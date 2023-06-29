# Comparing `tmp/aws-cdk.integ-tests-alpha-2.85.0a0.tar.gz` & `tmp/aws-cdk.integ-tests-alpha-2.86.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src913890871/src/packages/@aws-cdk/integ-tests-alpha/dist/python/aws-cdk.integ-tests-alpha-2.85.0a0.tar", last modified: Wed Jun 21 13:32:08 2023, max compression
+gzip compressed data, was "/codebuild/output/src3755887465/src/packages/@aws-cdk/integ-tests-alpha/dist/python/aws-cdk.integ-tests-alpha-2.86.0a0.tar", last modified: Thu Jun 29 08:23:32 2023, max compression
```

## Comparing `aws-cdk.integ-tests-alpha-2.85.0a0.tar` & `aws-cdk.integ-tests-alpha-2.86.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    16501 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15508 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1862 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk/integ_tests_alpha/
--rw-r--r--   0 root         (0) root         (0)   227828 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk/integ_tests_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk/integ_tests_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      441 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk/integ_tests_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   147040 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk/integ_tests_alpha/_jsii/integ-tests-alpha@2.85.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:32:00.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk/integ_tests_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk.integ_tests_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16501 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk.integ_tests_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk.integ_tests_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk.integ_tests_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk.integ_tests_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-21 13:32:08.000000 aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk.integ_tests_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:32.000000 aws-cdk.integ-tests-alpha-2.86.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-06-29 08:23:25.000000 aws-cdk.integ-tests-alpha-2.86.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-29 08:23:25.000000 aws-cdk.integ-tests-alpha-2.86.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-29 08:23:25.000000 aws-cdk.integ-tests-alpha-2.86.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    17167 2023-06-29 08:23:32.000000 aws-cdk.integ-tests-alpha-2.86.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16174 2023-06-29 08:23:25.000000 aws-cdk.integ-tests-alpha-2.86.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-29 08:23:25.000000 aws-cdk.integ-tests-alpha-2.86.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 08:23:32.000000 aws-cdk.integ-tests-alpha-2.86.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1862 2023-06-29 08:23:25.000000 aws-cdk.integ-tests-alpha-2.86.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:32.000000 aws-cdk.integ-tests-alpha-2.86.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:32.000000 aws-cdk.integ-tests-alpha-2.86.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:32.000000 aws-cdk.integ-tests-alpha-2.86.0a0/src/aws_cdk/integ_tests_alpha/
+-rw-r--r--   0 root         (0) root         (0)   258346 2023-06-29 08:23:25.000000 aws-cdk.integ-tests-alpha-2.86.0a0/src/aws_cdk/integ_tests_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:32.000000 aws-cdk.integ-tests-alpha-2.86.0a0/src/aws_cdk/integ_tests_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-06-29 08:23:25.000000 aws-cdk.integ-tests-alpha-2.86.0a0/src/aws_cdk/integ_tests_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   437875 2023-06-29 08:23:25.000000 aws-cdk.integ-tests-alpha-2.86.0a0/src/aws_cdk/integ_tests_alpha/_jsii/integ-tests-alpha@2.86.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 08:23:25.000000 aws-cdk.integ-tests-alpha-2.86.0a0/src/aws_cdk/integ_tests_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:32.000000 aws-cdk.integ-tests-alpha-2.86.0a0/src/aws_cdk.integ_tests_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17167 2023-06-29 08:23:32.000000 aws-cdk.integ-tests-alpha-2.86.0a0/src/aws_cdk.integ_tests_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-29 08:23:32.000000 aws-cdk.integ-tests-alpha-2.86.0a0/src/aws_cdk.integ_tests_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 08:23:32.000000 aws-cdk.integ-tests-alpha-2.86.0a0/src/aws_cdk.integ_tests_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-29 08:23:32.000000 aws-cdk.integ-tests-alpha-2.86.0a0/src/aws_cdk.integ_tests_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-29 08:23:32.000000 aws-cdk.integ-tests-alpha-2.86.0a0/src/aws_cdk.integ_tests_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.integ-tests-alpha-2.85.0a0/LICENSE` & `aws-cdk.integ-tests-alpha-2.86.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.integ-tests-alpha-2.85.0a0/PKG-INFO` & `aws-cdk.integ-tests-alpha-2.86.0a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.integ-tests-alpha
-Version: 2.85.0a0
+Version: 2.86.0a0
 Summary: CDK Integration Testing Constructs
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -254,20 +254,53 @@
     ExpectedResult.object_like({"foo": "bar"}),
     ActualResult.from_custom_resource(my_custom_resource, "data"))
 ```
 
 In the above example an assertion is created that will trigger a user defined `CustomResource`
 and assert that the `data` attribute is equal to `{ foo: 'bar' }`.
 
-### AwsApiCall
+### API Calls
 
 A common method to retrieve the "actual" results to compare with what is expected is to make an
-AWS API call to receive some data. This library does this by utilizing CloudFormation custom resources
+API call to receive some data. This library does this by utilizing CloudFormation custom resources
 which means that CloudFormation will call out to a Lambda Function which will
-use the AWS JavaScript SDK to make the API call.
+make the API call.
+
+#### HttpApiCall
+
+Using the `HttpApiCall` will use the
+[node-fetch](https://github.com/node-fetch/node-fetch) JavaScript library to
+make the HTTP call.
+
+This can be done by using the class directory (in the case of a normal deployment):
+
+```python
+# stack: Stack
+
+
+HttpApiCall(stack, "MyAsssertion",
+    url="https://example-api.com/abc"
+)
+```
+
+Or by using the `httpApiCall` method on `DeployAssert` (when writing integration tests):
+
+```python
+# app: App
+# stack: Stack
+
+integ = IntegTest(app, "Integ",
+    test_cases=[stack]
+)
+integ.assertions.http_api_call("https://example-api.com/abc")
+```
+
+#### AwsApiCall
+
+Using the `AwsApiCall` construct will use the AWS JavaScript SDK to make the API call.
 
 This can be done by using the class directory (in the case of a normal deployment):
 
 ```python
 # stack: Stack
```

### Comparing `aws-cdk.integ-tests-alpha-2.85.0a0/README.md` & `aws-cdk.integ-tests-alpha-2.86.0a0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -227,20 +227,53 @@
     ExpectedResult.object_like({"foo": "bar"}),
     ActualResult.from_custom_resource(my_custom_resource, "data"))
 ```
 
 In the above example an assertion is created that will trigger a user defined `CustomResource`
 and assert that the `data` attribute is equal to `{ foo: 'bar' }`.
 
-### AwsApiCall
+### API Calls
 
 A common method to retrieve the "actual" results to compare with what is expected is to make an
-AWS API call to receive some data. This library does this by utilizing CloudFormation custom resources
+API call to receive some data. This library does this by utilizing CloudFormation custom resources
 which means that CloudFormation will call out to a Lambda Function which will
-use the AWS JavaScript SDK to make the API call.
+make the API call.
+
+#### HttpApiCall
+
+Using the `HttpApiCall` will use the
+[node-fetch](https://github.com/node-fetch/node-fetch) JavaScript library to
+make the HTTP call.
+
+This can be done by using the class directory (in the case of a normal deployment):
+
+```python
+# stack: Stack
+
+
+HttpApiCall(stack, "MyAsssertion",
+    url="https://example-api.com/abc"
+)
+```
+
+Or by using the `httpApiCall` method on `DeployAssert` (when writing integration tests):
+
+```python
+# app: App
+# stack: Stack
+
+integ = IntegTest(app, "Integ",
+    test_cases=[stack]
+)
+integ.assertions.http_api_call("https://example-api.com/abc")
+```
+
+#### AwsApiCall
+
+Using the `AwsApiCall` construct will use the AWS JavaScript SDK to make the API call.
 
 This can be done by using the class directory (in the case of a normal deployment):
 
 ```python
 # stack: Stack
```

### Comparing `aws-cdk.integ-tests-alpha-2.85.0a0/setup.py` & `aws-cdk.integ-tests-alpha-2.86.0a0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.integ-tests-alpha",
-    "version": "2.85.0.a0",
+    "version": "2.86.0.a0",
     "description": "CDK Integration Testing Constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_cdk.integ_tests_alpha",
         "aws_cdk.integ_tests_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.integ_tests_alpha._jsii": [
-            "integ-tests-alpha@2.85.0-alpha.0.jsii.tgz"
+            "integ-tests-alpha@2.86.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.integ_tests_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.85.0",
+        "aws-cdk-lib==2.86.0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk/integ_tests_alpha/__init__.py` & `aws-cdk.integ-tests-alpha-2.86.0a0/src/aws_cdk/integ_tests_alpha/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -228,20 +228,53 @@
     ExpectedResult.object_like({"foo": "bar"}),
     ActualResult.from_custom_resource(my_custom_resource, "data"))
 ```
 
 In the above example an assertion is created that will trigger a user defined `CustomResource`
 and assert that the `data` attribute is equal to `{ foo: 'bar' }`.
 
-### AwsApiCall
+### API Calls
 
 A common method to retrieve the "actual" results to compare with what is expected is to make an
-AWS API call to receive some data. This library does this by utilizing CloudFormation custom resources
+API call to receive some data. This library does this by utilizing CloudFormation custom resources
 which means that CloudFormation will call out to a Lambda Function which will
-use the AWS JavaScript SDK to make the API call.
+make the API call.
+
+#### HttpApiCall
+
+Using the `HttpApiCall` will use the
+[node-fetch](https://github.com/node-fetch/node-fetch) JavaScript library to
+make the HTTP call.
+
+This can be done by using the class directory (in the case of a normal deployment):
+
+```python
+# stack: Stack
+
+
+HttpApiCall(stack, "MyAsssertion",
+    url="https://example-api.com/abc"
+)
+```
+
+Or by using the `httpApiCall` method on `DeployAssert` (when writing integration tests):
+
+```python
+# app: App
+# stack: Stack
+
+integ = IntegTest(app, "Integ",
+    test_cases=[stack]
+)
+integ.assertions.http_api_call("https://example-api.com/abc")
+```
+
+#### AwsApiCall
+
+Using the `AwsApiCall` construct will use the AWS JavaScript SDK to make the API call.
 
 This can be done by using the class directory (in the case of a normal deployment):
 
 ```python
 # stack: Stack
 
 
@@ -1824,14 +1857,488 @@
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "result", value)
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the abstract class
 typing.cast(typing.Any, ExpectedResult).__jsii_proxy_class__ = lambda : _ExpectedResultProxy
 
 
+@jsii.data_type(
+    jsii_type="@aws-cdk/integ-tests-alpha.FetchOptions",
+    jsii_struct_bases=[],
+    name_mapping={
+        "body": "body",
+        "headers": "headers",
+        "method": "method",
+        "port": "port",
+    },
+)
+class FetchOptions:
+    def __init__(
+        self,
+        *,
+        body: typing.Optional[builtins.str] = None,
+        headers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        method: typing.Optional[builtins.str] = None,
+        port: typing.Optional[jsii.Number] = None,
+    ) -> None:
+        '''(experimental) Options to pass to the JavaScript fetch api.
+
+        :param body: (experimental) Request body. Default: - no body
+        :param headers: (experimental) Optional request headers. Default: no headers
+        :param method: (experimental) HTTP method. Default: GET
+        :param port: (experimental) Optional port. Default: default port for protocol
+
+        :stability: experimental
+        :exampleMetadata: fixture=_generated
+
+        Example::
+
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.integ_tests_alpha as integ_tests_alpha
+            
+            fetch_options = integ_tests_alpha.FetchOptions(
+                body="body",
+                headers={
+                    "headers_key": "headers"
+                },
+                method="method",
+                port=123
+            )
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__e2e88c6f6439b0e809ba451cf7d5fdcb3370b99a16f4d97c6d1c6ff524a91f56)
+            check_type(argname="argument body", value=body, expected_type=type_hints["body"])
+            check_type(argname="argument headers", value=headers, expected_type=type_hints["headers"])
+            check_type(argname="argument method", value=method, expected_type=type_hints["method"])
+            check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if body is not None:
+            self._values["body"] = body
+        if headers is not None:
+            self._values["headers"] = headers
+        if method is not None:
+            self._values["method"] = method
+        if port is not None:
+            self._values["port"] = port
+
+    @builtins.property
+    def body(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Request body.
+
+        :default: - no body
+
+        :stability: experimental
+        '''
+        result = self._values.get("body")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def headers(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
+        '''(experimental) Optional request headers.
+
+        :default: no headers
+
+        :stability: experimental
+        '''
+        result = self._values.get("headers")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
+
+    @builtins.property
+    def method(self) -> typing.Optional[builtins.str]:
+        '''(experimental) HTTP method.
+
+        :default: GET
+
+        :stability: experimental
+        '''
+        result = self._values.get("method")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def port(self) -> typing.Optional[jsii.Number]:
+        '''(experimental) Optional port.
+
+        :default: default port for protocol
+
+        :stability: experimental
+        '''
+        result = self._values.get("port")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "FetchOptions(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="@aws-cdk/integ-tests-alpha.HttpRequest",
+    jsii_struct_bases=[],
+    name_mapping={"parameters": "parameters"},
+)
+class HttpRequest:
+    def __init__(
+        self,
+        *,
+        parameters: typing.Union["HttpRequestParameters", typing.Dict[builtins.str, typing.Any]],
+    ) -> None:
+        '''(experimental) Request to the HttpCall resource.
+
+        :param parameters: (experimental) Parameters from the custom resource.
+
+        :stability: experimental
+        :exampleMetadata: fixture=_generated
+
+        Example::
+
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.integ_tests_alpha as integ_tests_alpha
+            
+            http_request = integ_tests_alpha.HttpRequest(
+                parameters=integ_tests_alpha.HttpRequestParameters(
+                    url="url",
+            
+                    # the properties below are optional
+                    fetch_options=integ_tests_alpha.FetchOptions(
+                        body="body",
+                        headers={
+                            "headers_key": "headers"
+                        },
+                        method="method",
+                        port=123
+                    )
+                )
+            )
+        '''
+        if isinstance(parameters, dict):
+            parameters = HttpRequestParameters(**parameters)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__7e43070ab7c42531f81da281a2f078d3aaa5c2747ce7ed529dd5083e0ecf1f15)
+            check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "parameters": parameters,
+        }
+
+    @builtins.property
+    def parameters(self) -> "HttpRequestParameters":
+        '''(experimental) Parameters from the custom resource.
+
+        :stability: experimental
+        '''
+        result = self._values.get("parameters")
+        assert result is not None, "Required property 'parameters' is missing"
+        return typing.cast("HttpRequestParameters", result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "HttpRequest(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="@aws-cdk/integ-tests-alpha.HttpRequestParameters",
+    jsii_struct_bases=[],
+    name_mapping={"url": "url", "fetch_options": "fetchOptions"},
+)
+class HttpRequestParameters:
+    def __init__(
+        self,
+        *,
+        url: builtins.str,
+        fetch_options: typing.Optional[typing.Union[FetchOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    ) -> None:
+        '''
+        :param url: (experimental) The url to fetch.
+        :param fetch_options: (experimental) Options for fetch.
+
+        :stability: experimental
+        :exampleMetadata: fixture=_generated
+
+        Example::
+
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.integ_tests_alpha as integ_tests_alpha
+            
+            http_request_parameters = integ_tests_alpha.HttpRequestParameters(
+                url="url",
+            
+                # the properties below are optional
+                fetch_options=integ_tests_alpha.FetchOptions(
+                    body="body",
+                    headers={
+                        "headers_key": "headers"
+                    },
+                    method="method",
+                    port=123
+                )
+            )
+        '''
+        if isinstance(fetch_options, dict):
+            fetch_options = FetchOptions(**fetch_options)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__93af9c54916c56a6f8f854ed0b3f9f13208556a5bdfc783196525c8d6ac46dab)
+            check_type(argname="argument url", value=url, expected_type=type_hints["url"])
+            check_type(argname="argument fetch_options", value=fetch_options, expected_type=type_hints["fetch_options"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "url": url,
+        }
+        if fetch_options is not None:
+            self._values["fetch_options"] = fetch_options
+
+    @builtins.property
+    def url(self) -> builtins.str:
+        '''(experimental) The url to fetch.
+
+        :stability: experimental
+        '''
+        result = self._values.get("url")
+        assert result is not None, "Required property 'url' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def fetch_options(self) -> typing.Optional[FetchOptions]:
+        '''(experimental) Options for fetch.
+
+        :stability: experimental
+        '''
+        result = self._values.get("fetch_options")
+        return typing.cast(typing.Optional[FetchOptions], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "HttpRequestParameters(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="@aws-cdk/integ-tests-alpha.HttpResponse",
+    jsii_struct_bases=[],
+    name_mapping={
+        "headers": "headers",
+        "ok": "ok",
+        "response_json": "responseJson",
+        "status": "status",
+        "status_text": "statusText",
+    },
+)
+class HttpResponse:
+    def __init__(
+        self,
+        *,
+        headers: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+        ok: typing.Optional[builtins.bool] = None,
+        response_json: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+        status: typing.Optional[jsii.Number] = None,
+        status_text: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''(experimental) Response from fetch.
+
+        :param headers: (experimental) Headers associated with the response.
+        :param ok: (experimental) Indicates whether the response was successful. status range 200-299
+        :param response_json: (experimental) The response as JSON.
+        :param status: (experimental) Status code of the response.
+        :param status_text: (experimental) The status message corresponding to the status code.
+
+        :stability: experimental
+        :exampleMetadata: fixture=_generated
+
+        Example::
+
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.integ_tests_alpha as integ_tests_alpha
+            
+            # headers: Any
+            # response_json: Any
+            
+            http_response = integ_tests_alpha.HttpResponse(
+                headers={
+                    "headers_key": headers
+                },
+                ok=False,
+                response_json={
+                    "response_json_key": response_json
+                },
+                status=123,
+                status_text="statusText"
+            )
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__391c496ab114dbafa2050e50cd71e9603e3723e49e2d262950bd96589530e06a)
+            check_type(argname="argument headers", value=headers, expected_type=type_hints["headers"])
+            check_type(argname="argument ok", value=ok, expected_type=type_hints["ok"])
+            check_type(argname="argument response_json", value=response_json, expected_type=type_hints["response_json"])
+            check_type(argname="argument status", value=status, expected_type=type_hints["status"])
+            check_type(argname="argument status_text", value=status_text, expected_type=type_hints["status_text"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if headers is not None:
+            self._values["headers"] = headers
+        if ok is not None:
+            self._values["ok"] = ok
+        if response_json is not None:
+            self._values["response_json"] = response_json
+        if status is not None:
+            self._values["status"] = status
+        if status_text is not None:
+            self._values["status_text"] = status_text
+
+    @builtins.property
+    def headers(self) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
+        '''(experimental) Headers associated with the response.
+
+        :stability: experimental
+        '''
+        result = self._values.get("headers")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
+
+    @builtins.property
+    def ok(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Indicates whether the response was successful.
+
+        status range 200-299
+
+        :stability: experimental
+        '''
+        result = self._values.get("ok")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def response_json(
+        self,
+    ) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
+        '''(experimental) The response as JSON.
+
+        :stability: experimental
+        '''
+        result = self._values.get("response_json")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
+
+    @builtins.property
+    def status(self) -> typing.Optional[jsii.Number]:
+        '''(experimental) Status code of the response.
+
+        :stability: experimental
+        '''
+        result = self._values.get("status")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def status_text(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The status message corresponding to the status code.
+
+        :stability: experimental
+        '''
+        result = self._values.get("status_text")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "HttpResponse(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="@aws-cdk/integ-tests-alpha.HttpResponseWrapper",
+    jsii_struct_bases=[],
+    name_mapping={"api_call_response": "apiCallResponse"},
+)
+class HttpResponseWrapper:
+    def __init__(
+        self,
+        *,
+        api_call_response: typing.Union[HttpResponse, typing.Dict[builtins.str, typing.Any]],
+    ) -> None:
+        '''(experimental) Response from the HttpCall resource.
+
+        :param api_call_response: (experimental) The Response from the fetch request.
+
+        :stability: experimental
+        :exampleMetadata: fixture=_generated
+
+        Example::
+
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.integ_tests_alpha as integ_tests_alpha
+            
+            # headers: Any
+            # response_json: Any
+            
+            http_response_wrapper = integ_tests_alpha.HttpResponseWrapper(
+                api_call_response=integ_tests_alpha.HttpResponse(
+                    headers={
+                        "headers_key": headers
+                    },
+                    ok=False,
+                    response_json={
+                        "response_json_key": response_json
+                    },
+                    status=123,
+                    status_text="statusText"
+                )
+            )
+        '''
+        if isinstance(api_call_response, dict):
+            api_call_response = HttpResponse(**api_call_response)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__fa97df0d1c119f8060810ef7873d7cbafff7b4b83e883dff6b5be3ec2fbbd17b)
+            check_type(argname="argument api_call_response", value=api_call_response, expected_type=type_hints["api_call_response"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "api_call_response": api_call_response,
+        }
+
+    @builtins.property
+    def api_call_response(self) -> HttpResponse:
+        '''(experimental) The Response from the fetch request.
+
+        :stability: experimental
+        '''
+        result = self._values.get("api_call_response")
+        assert result is not None, "Required property 'api_call_response' is missing"
+        return typing.cast(HttpResponse, result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "HttpResponseWrapper(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 @jsii.interface(jsii_type="@aws-cdk/integ-tests-alpha.IApiCall")
 class IApiCall(_constructs_77d1e7e8.IConstruct, typing_extensions.Protocol):
     '''(experimental) Represents an ApiCall.
 
     :stability: experimental
     '''
 
@@ -2265,14 +2772,46 @@
             
             integ.assertions.expect("invoke",
                 ExpectedResult.object_like({"Payload": "OK"}),
                 ActualResult.from_aws_api_call(api_call, "Body"))
         '''
         ...
 
+    @jsii.member(jsii_name="httpApiCall")
+    def http_api_call(
+        self,
+        url: builtins.str,
+        *,
+        body: typing.Optional[builtins.str] = None,
+        headers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        method: typing.Optional[builtins.str] = None,
+        port: typing.Optional[jsii.Number] = None,
+    ) -> IApiCall:
+        '''(experimental) Make an HTTP call to the provided endpoint.
+
+        :param url: -
+        :param body: (experimental) Request body. Default: - no body
+        :param headers: (experimental) Optional request headers. Default: no headers
+        :param method: (experimental) HTTP method. Default: GET
+        :param port: (experimental) Optional port. Default: default port for protocol
+
+        :stability: experimental
+
+        Example::
+
+            # app: App
+            # integ: IntegTest
+            
+            call = integ.assertions.http_api_call("https://example.com/test")
+            call.expect(ExpectedResult.object_like({
+                "Message": "Hello World!"
+            }))
+        '''
+        ...
+
     @jsii.member(jsii_name="invokeFunction")
     def invoke_function(
         self,
         *,
         function_name: builtins.str,
         invocation_type: typing.Optional["InvocationType"] = None,
         log_type: typing.Optional["LogType"] = None,
@@ -2385,14 +2924,51 @@
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bc5691b1933125f6e27b8109881a6206c07bcdea66d6a2a61d313cd6f7b30ce8)
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument expected", value=expected, expected_type=type_hints["expected"])
             check_type(argname="argument actual", value=actual, expected_type=type_hints["actual"])
         return typing.cast(None, jsii.invoke(self, "expect", [id, expected, actual]))
 
+    @jsii.member(jsii_name="httpApiCall")
+    def http_api_call(
+        self,
+        url: builtins.str,
+        *,
+        body: typing.Optional[builtins.str] = None,
+        headers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        method: typing.Optional[builtins.str] = None,
+        port: typing.Optional[jsii.Number] = None,
+    ) -> IApiCall:
+        '''(experimental) Make an HTTP call to the provided endpoint.
+
+        :param url: -
+        :param body: (experimental) Request body. Default: - no body
+        :param headers: (experimental) Optional request headers. Default: no headers
+        :param method: (experimental) HTTP method. Default: GET
+        :param port: (experimental) Optional port. Default: default port for protocol
+
+        :stability: experimental
+
+        Example::
+
+            # app: App
+            # integ: IntegTest
+            
+            call = integ.assertions.http_api_call("https://example.com/test")
+            call.expect(ExpectedResult.object_like({
+                "Message": "Hello World!"
+            }))
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9053497bae85d950ab08f20afee06c8e7c3e89c63f987e0320dba88e432ddff5)
+            check_type(argname="argument url", value=url, expected_type=type_hints["url"])
+        options = FetchOptions(body=body, headers=headers, method=method, port=port)
+
+        return typing.cast(IApiCall, jsii.invoke(self, "httpApiCall", [url, options]))
+
     @jsii.member(jsii_name="invokeFunction")
     def invoke_function(
         self,
         *,
         function_name: builtins.str,
         invocation_type: typing.Optional["InvocationType"] = None,
         log_type: typing.Optional["LogType"] = None,
@@ -2443,30 +3019,23 @@
     instance of this class.
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
-        # lambda_function: lambda.IFunction
+        # my_custom_resource: CustomResource
+        # stack: Stack
         # app: App
         
         
-        stack = Stack(app, "cdk-integ-lambda-bundling")
-        
-        integ = IntegTest(app, "IntegTest",
-            test_cases=[stack]
-        )
-        
-        invoke = integ.assertions.invoke_function(
-            function_name=lambda_function.function_name
-        )
-        invoke.expect(ExpectedResult.object_like({
-            "Payload": "200"
-        }))
+        integ = IntegTest(app, "Integ", test_cases=[stack])
+        integ.assertions.expect("CustomAssertion",
+            ExpectedResult.object_like({"foo": "bar"}),
+            ActualResult.from_custom_resource(my_custom_resource, "data"))
     '''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
@@ -3554,30 +4123,23 @@
         :param enable_lookups: (experimental) Enable lookups for this test. If lookups are enabled then ``stackUpdateWorkflow`` must be set to false. Lookups should only be enabled when you are explicitly testing lookups. Default: false
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
-            # lambda_function: lambda.IFunction
+            # my_custom_resource: CustomResource
+            # stack: Stack
             # app: App
             
             
-            stack = Stack(app, "cdk-integ-lambda-bundling")
-            
-            integ = IntegTest(app, "IntegTest",
-                test_cases=[stack]
-            )
-            
-            invoke = integ.assertions.invoke_function(
-                function_name=lambda_function.function_name
-            )
-            invoke.expect(ExpectedResult.object_like({
-                "Payload": "200"
-            }))
+            integ = IntegTest(app, "Integ", test_cases=[stack])
+            integ.assertions.expect("CustomAssertion",
+                ExpectedResult.object_like({"foo": "bar"}),
+                ActualResult.from_custom_resource(my_custom_resource, "data"))
         '''
         if isinstance(cdk_command_options, dict):
             cdk_command_options = _aws_cdk_cloud_assembly_schema_ceddda9d.CdkCommands(**cdk_command_options)
         if isinstance(hooks, dict):
             hooks = _aws_cdk_cloud_assembly_schema_ceddda9d.Hooks(**hooks)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7a2013546a0269b479331ed4cdfd706a8b20bf18d5f45e074d56ae77eb9b6dd4)
@@ -4902,14 +5464,202 @@
     def waiter_provider(self, value: typing.Optional[AssertionsProvider]) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0e978f2b80fc7ca4cf867ebf9e4673daf1582477274721902259a31caf906a43)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "waiterProvider", value)
 
 
+class HttpApiCall(
+    ApiCallBase,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@aws-cdk/integ-tests-alpha.HttpApiCall",
+):
+    '''(experimental) Construct that creates a custom resource that will perform an HTTP API Call.
+
+    :stability: experimental
+    :exampleMetadata: infused
+
+    Example::
+
+        # stack: Stack
+        
+        
+        HttpApiCall(stack, "MyAsssertion",
+            url="https://example-api.com/abc"
+        )
+    '''
+
+    def __init__(
+        self,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        *,
+        url: builtins.str,
+        fetch_options: typing.Optional[typing.Union[FetchOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    ) -> None:
+        '''
+        :param scope: -
+        :param id: -
+        :param url: (experimental) The url to fetch.
+        :param fetch_options: (experimental) Options for fetch.
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__0209121e751279aa416df5a16ee8548cf444948c1d390c4c88c07eb8c6b1c58a)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = HttpCallProps(url=url, fetch_options=fetch_options)
+
+        jsii.create(self.__class__, self, [scope, id, props])
+
+    @jsii.member(jsii_name="assertAtPath")
+    def assert_at_path(
+        self,
+        _path: builtins.str,
+        _expected: ExpectedResult,
+    ) -> IApiCall:
+        '''(experimental) Assert that the ExpectedResult is equal to the result of the AwsApiCall at the given path.
+
+        Providing a path will filter the output of the initial API call.
+
+        For example the SQS.receiveMessage api response would look
+        like:
+
+        If you wanted to assert the value of ``Body`` you could do
+
+        :param _path: -
+        :param _expected: -
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__eb5f6f39838f44a897965a4772b5b6db17ad826ce021bb98080a9af10f1207c9)
+            check_type(argname="argument _path", value=_path, expected_type=type_hints["_path"])
+            check_type(argname="argument _expected", value=_expected, expected_type=type_hints["_expected"])
+        return typing.cast(IApiCall, jsii.invoke(self, "assertAtPath", [_path, _expected]))
+
+    @jsii.member(jsii_name="waitForAssertions")
+    def wait_for_assertions(
+        self,
+        *,
+        backoff_rate: typing.Optional[jsii.Number] = None,
+        interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        total_timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+    ) -> IApiCall:
+        '''(experimental) Wait for the IApiCall to return the expected response.
+
+        If no expected response is specified then it will wait for
+        the IApiCall to return a success
+
+        :param backoff_rate: (experimental) Backoff between attempts. This is the multiplier by which the retry interval increases after each retry attempt. By default there is no backoff. Each retry will wait the amount of time specified by ``interval``. Default: 1 (no backoff)
+        :param interval: (experimental) The interval (number of seconds) to wait between attempts. Default: Duration.seconds(5)
+        :param total_timeout: (experimental) The total time that the state machine will wait for a successful response. Default: Duration.minutes(30)
+
+        :stability: experimental
+        '''
+        options = WaiterStateMachineOptions(
+            backoff_rate=backoff_rate, interval=interval, total_timeout=total_timeout
+        )
+
+        return typing.cast(IApiCall, jsii.invoke(self, "waitForAssertions", [options]))
+
+    @builtins.property
+    @jsii.member(jsii_name="apiCallResource")
+    def _api_call_resource(self) -> _aws_cdk_ceddda9d.CustomResource:
+        '''
+        :stability: experimental
+        '''
+        return typing.cast(_aws_cdk_ceddda9d.CustomResource, jsii.get(self, "apiCallResource"))
+
+    @builtins.property
+    @jsii.member(jsii_name="provider")
+    def provider(self) -> AssertionsProvider:
+        '''(experimental) access the AssertionsProvider.
+
+        This can be used to add additional IAM policies
+        the the provider role policy
+
+        :stability: experimental
+        '''
+        return typing.cast(AssertionsProvider, jsii.get(self, "provider"))
+
+
+@jsii.data_type(
+    jsii_type="@aws-cdk/integ-tests-alpha.HttpCallProps",
+    jsii_struct_bases=[HttpRequestParameters],
+    name_mapping={"url": "url", "fetch_options": "fetchOptions"},
+)
+class HttpCallProps(HttpRequestParameters):
+    def __init__(
+        self,
+        *,
+        url: builtins.str,
+        fetch_options: typing.Optional[typing.Union[FetchOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    ) -> None:
+        '''(experimental) Options for creating an HttpApiCall provider.
+
+        :param url: (experimental) The url to fetch.
+        :param fetch_options: (experimental) Options for fetch.
+
+        :stability: experimental
+        :exampleMetadata: infused
+
+        Example::
+
+            # stack: Stack
+            
+            
+            HttpApiCall(stack, "MyAsssertion",
+                url="https://example-api.com/abc"
+            )
+        '''
+        if isinstance(fetch_options, dict):
+            fetch_options = FetchOptions(**fetch_options)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__1f4a71f13aa64d1306c572e9f98559d007cead2ee1c483183f46e1dad96274fd)
+            check_type(argname="argument url", value=url, expected_type=type_hints["url"])
+            check_type(argname="argument fetch_options", value=fetch_options, expected_type=type_hints["fetch_options"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "url": url,
+        }
+        if fetch_options is not None:
+            self._values["fetch_options"] = fetch_options
+
+    @builtins.property
+    def url(self) -> builtins.str:
+        '''(experimental) The url to fetch.
+
+        :stability: experimental
+        '''
+        result = self._values.get("url")
+        assert result is not None, "Required property 'url' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def fetch_options(self) -> typing.Optional[FetchOptions]:
+        '''(experimental) Options for fetch.
+
+        :stability: experimental
+        '''
+        result = self._values.get("fetch_options")
+        return typing.cast(typing.Optional[FetchOptions], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "HttpCallProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class LambdaInvokeFunction(
     AwsApiCall,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/integ-tests-alpha.LambdaInvokeFunction",
 ):
     '''(experimental) An AWS Lambda Invoke function API call.
 
@@ -4983,14 +5733,21 @@
     "AwsApiCallOptions",
     "AwsApiCallProps",
     "AwsApiCallRequest",
     "AwsApiCallResult",
     "EqualsAssertion",
     "EqualsAssertionProps",
     "ExpectedResult",
+    "FetchOptions",
+    "HttpApiCall",
+    "HttpCallProps",
+    "HttpRequest",
+    "HttpRequestParameters",
+    "HttpResponse",
+    "HttpResponseWrapper",
     "IApiCall",
     "IDeployAssert",
     "IntegTest",
     "IntegTestCase",
     "IntegTestCaseProps",
     "IntegTestCaseStack",
     "IntegTestCaseStackProps",
@@ -5174,14 +5931,57 @@
 
 def _typecheckingstub__e33010e7c2f43ad7b078d998ca478ef09e6cf76bc2eadeb12407d48e7f8d56d3(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__e2e88c6f6439b0e809ba451cf7d5fdcb3370b99a16f4d97c6d1c6ff524a91f56(
+    *,
+    body: typing.Optional[builtins.str] = None,
+    headers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    method: typing.Optional[builtins.str] = None,
+    port: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7e43070ab7c42531f81da281a2f078d3aaa5c2747ce7ed529dd5083e0ecf1f15(
+    *,
+    parameters: typing.Union[HttpRequestParameters, typing.Dict[builtins.str, typing.Any]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__93af9c54916c56a6f8f854ed0b3f9f13208556a5bdfc783196525c8d6ac46dab(
+    *,
+    url: builtins.str,
+    fetch_options: typing.Optional[typing.Union[FetchOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__391c496ab114dbafa2050e50cd71e9603e3723e49e2d262950bd96589530e06a(
+    *,
+    headers: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+    ok: typing.Optional[builtins.bool] = None,
+    response_json: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+    status: typing.Optional[jsii.Number] = None,
+    status_text: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__fa97df0d1c119f8060810ef7873d7cbafff7b4b83e883dff6b5be3ec2fbbd17b(
+    *,
+    api_call_response: typing.Union[HttpResponse, typing.Dict[builtins.str, typing.Any]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__f411c9c6ce09258efafb36af27db400c2f261d107ee630843a9353825628ab2a(
     path: builtins.str,
     expected: ExpectedResult,
 ) -> None:
     """Type checking stubs"""
     pass
 
@@ -5222,14 +6022,25 @@
     id: builtins.str,
     expected: ExpectedResult,
     actual: ActualResult,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__9053497bae85d950ab08f20afee06c8e7c3e89c63f987e0320dba88e432ddff5(
+    url: builtins.str,
+    *,
+    body: typing.Optional[builtins.str] = None,
+    headers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    method: typing.Optional[builtins.str] = None,
+    port: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__12fb8761c88b4fc9579f6a32db4edfe539963bdb489338e7e428d98f41281684(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     test_cases: typing.Sequence[_aws_cdk_ceddda9d.Stack],
     assertion_stack: typing.Optional[_aws_cdk_ceddda9d.Stack] = None,
     enable_lookups: typing.Optional[builtins.bool] = None,
@@ -5495,14 +6306,39 @@
 
 def _typecheckingstub__0e978f2b80fc7ca4cf867ebf9e4673daf1582477274721902259a31caf906a43(
     value: typing.Optional[AssertionsProvider],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__0209121e751279aa416df5a16ee8548cf444948c1d390c4c88c07eb8c6b1c58a(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    url: builtins.str,
+    fetch_options: typing.Optional[typing.Union[FetchOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__eb5f6f39838f44a897965a4772b5b6db17ad826ce021bb98080a9af10f1207c9(
+    _path: builtins.str,
+    _expected: ExpectedResult,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__1f4a71f13aa64d1306c572e9f98559d007cead2ee1c483183f46e1dad96274fd(
+    *,
+    url: builtins.str,
+    fetch_options: typing.Optional[typing.Union[FetchOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__fc846004ad65c16a9a1322c4c518ae25ebd02b2bc7803230f5bb11a2884f1de0(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     function_name: builtins.str,
     invocation_type: typing.Optional[InvocationType] = None,
     log_type: typing.Optional[LogType] = None,
```

### Comparing `aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk.integ_tests_alpha.egg-info/PKG-INFO` & `aws-cdk.integ-tests-alpha-2.86.0a0/src/aws_cdk.integ_tests_alpha.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.integ-tests-alpha
-Version: 2.85.0a0
+Version: 2.86.0a0
 Summary: CDK Integration Testing Constructs
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -254,20 +254,53 @@
     ExpectedResult.object_like({"foo": "bar"}),
     ActualResult.from_custom_resource(my_custom_resource, "data"))
 ```
 
 In the above example an assertion is created that will trigger a user defined `CustomResource`
 and assert that the `data` attribute is equal to `{ foo: 'bar' }`.
 
-### AwsApiCall
+### API Calls
 
 A common method to retrieve the "actual" results to compare with what is expected is to make an
-AWS API call to receive some data. This library does this by utilizing CloudFormation custom resources
+API call to receive some data. This library does this by utilizing CloudFormation custom resources
 which means that CloudFormation will call out to a Lambda Function which will
-use the AWS JavaScript SDK to make the API call.
+make the API call.
+
+#### HttpApiCall
+
+Using the `HttpApiCall` will use the
+[node-fetch](https://github.com/node-fetch/node-fetch) JavaScript library to
+make the HTTP call.
+
+This can be done by using the class directory (in the case of a normal deployment):
+
+```python
+# stack: Stack
+
+
+HttpApiCall(stack, "MyAsssertion",
+    url="https://example-api.com/abc"
+)
+```
+
+Or by using the `httpApiCall` method on `DeployAssert` (when writing integration tests):
+
+```python
+# app: App
+# stack: Stack
+
+integ = IntegTest(app, "Integ",
+    test_cases=[stack]
+)
+integ.assertions.http_api_call("https://example-api.com/abc")
+```
+
+#### AwsApiCall
+
+Using the `AwsApiCall` construct will use the AWS JavaScript SDK to make the API call.
 
 This can be done by using the class directory (in the case of a normal deployment):
 
 ```python
 # stack: Stack
```

### Comparing `aws-cdk.integ-tests-alpha-2.85.0a0/src/aws_cdk.integ_tests_alpha.egg-info/SOURCES.txt` & `aws-cdk.integ-tests-alpha-2.86.0a0/src/aws_cdk.integ_tests_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.integ_tests_alpha.egg-info/SOURCES.txt
 src/aws_cdk.integ_tests_alpha.egg-info/dependency_links.txt
 src/aws_cdk.integ_tests_alpha.egg-info/requires.txt
 src/aws_cdk.integ_tests_alpha.egg-info/top_level.txt
 src/aws_cdk/integ_tests_alpha/__init__.py
 src/aws_cdk/integ_tests_alpha/py.typed
 src/aws_cdk/integ_tests_alpha/_jsii/__init__.py
-src/aws_cdk/integ_tests_alpha/_jsii/integ-tests-alpha@2.85.0-alpha.0.jsii.tgz
+src/aws_cdk/integ_tests_alpha/_jsii/integ-tests-alpha@2.86.0-alpha.0.jsii.tgz
```

