# Comparing `tmp/wechaty-grpc-1.5.dev2.tar.gz` & `tmp/wechaty-grpc-1.5.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wechaty-grpc-1.5.dev2.tar", last modified: Wed Apr 20 14:29:28 2022, max compression
+gzip compressed data, was "wechaty-grpc-1.5.dev4.tar", last modified: Thu Jun 29 08:12:16 2023, max compression
```

## Comparing `wechaty-grpc-1.5.dev2.tar` & `wechaty-grpc-1.5.dev4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.838808 wechaty-grpc-1.5.dev2/
--rw-r--r--   0 runner    (1001) docker     (121)    15021 2022-04-20 14:29:28.838808 wechaty-grpc-1.5.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-20 14:29:28.838808 wechaty-grpc-1.5.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-04-20 14:27:59.000000 wechaty-grpc-1.5.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.834808 wechaty-grpc-1.5.dev2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.834808 wechaty-grpc-1.5.dev2/src/wechaty_grpc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.000000 wechaty-grpc-1.5.dev2/src/wechaty_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.834808 wechaty-grpc-1.5.dev2/src/wechaty_grpc/google/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.000000 wechaty-grpc-1.5.dev2/src/wechaty_grpc/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.834808 wechaty-grpc-1.5.dev2/src/wechaty_grpc/google/api/
--rw-r--r--   0 runner    (1001) docker     (121)    14621 2022-04-20 14:29:28.000000 wechaty-grpc-1.5.dev2/src/wechaty_grpc/google/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.834808 wechaty-grpc-1.5.dev2/src/wechaty_grpc/grpc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.000000 wechaty-grpc-1.5.dev2/src/wechaty_grpc/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.838808 wechaty-grpc-1.5.dev2/src/wechaty_grpc/grpc/gateway/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.000000 wechaty-grpc-1.5.dev2/src/wechaty_grpc/grpc/gateway/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.838808 wechaty-grpc-1.5.dev2/src/wechaty_grpc/grpc/gateway/protoc_gen_openapiv2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.000000 wechaty-grpc-1.5.dev2/src/wechaty_grpc/grpc/gateway/protoc_gen_openapiv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.838808 wechaty-grpc-1.5.dev2/src/wechaty_grpc/grpc/gateway/protoc_gen_openapiv2/options/
--rw-r--r--   0 runner    (1001) docker     (121)    26732 2022-04-20 14:29:28.000000 wechaty-grpc-1.5.dev2/src/wechaty_grpc/grpc/gateway/protoc_gen_openapiv2/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.838808 wechaty-grpc-1.5.dev2/src/wechaty_grpc/wechaty/
--rw-r--r--   0 runner    (1001) docker     (121)    74685 2022-04-20 14:29:28.000000 wechaty-grpc-1.5.dev2/src/wechaty_grpc/wechaty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.838808 wechaty-grpc-1.5.dev2/src/wechaty_grpc/wechaty/puppet/
--rw-r--r--   0 runner    (1001) docker     (121)    40441 2022-04-20 14:29:28.000000 wechaty-grpc-1.5.dev2/src/wechaty_grpc/wechaty/puppet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:29:28.834808 wechaty-grpc-1.5.dev2/src/wechaty_grpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15021 2022-04-20 14:29:28.000000 wechaty-grpc-1.5.dev2/src/wechaty_grpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-04-20 14:29:28.000000 wechaty-grpc-1.5.dev2/src/wechaty_grpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 14:29:28.000000 wechaty-grpc-1.5.dev2/src/wechaty_grpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-04-20 14:29:28.000000 wechaty-grpc-1.5.dev2/src/wechaty_grpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-20 14:29:28.000000 wechaty-grpc-1.5.dev2/src/wechaty_grpc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:16.582760 wechaty-grpc-1.5.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-06-29 08:12:16.582760 wechaty-grpc-1.5.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:12:16.582760 wechaty-grpc-1.5.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-29 08:10:49.000000 wechaty-grpc-1.5.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:16.578760 wechaty-grpc-1.5.dev4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:16.582760 wechaty-grpc-1.5.dev4/src/wechaty_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:14.000000 wechaty-grpc-1.5.dev4/src/wechaty_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:16.582760 wechaty-grpc-1.5.dev4/src/wechaty_grpc/google/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:14.000000 wechaty-grpc-1.5.dev4/src/wechaty_grpc/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:16.582760 wechaty-grpc-1.5.dev4/src/wechaty_grpc/google/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-06-29 08:12:14.000000 wechaty-grpc-1.5.dev4/src/wechaty_grpc/google/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:16.582760 wechaty-grpc-1.5.dev4/src/wechaty_grpc/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:14.000000 wechaty-grpc-1.5.dev4/src/wechaty_grpc/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:16.582760 wechaty-grpc-1.5.dev4/src/wechaty_grpc/grpc/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:14.000000 wechaty-grpc-1.5.dev4/src/wechaty_grpc/grpc/gateway/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:16.582760 wechaty-grpc-1.5.dev4/src/wechaty_grpc/grpc/gateway/protoc_gen_openapiv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:14.000000 wechaty-grpc-1.5.dev4/src/wechaty_grpc/grpc/gateway/protoc_gen_openapiv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:16.582760 wechaty-grpc-1.5.dev4/src/wechaty_grpc/grpc/gateway/protoc_gen_openapiv2/options/
+-rw-r--r--   0 runner    (1001) docker     (123)    32279 2023-06-29 08:12:14.000000 wechaty-grpc-1.5.dev4/src/wechaty_grpc/grpc/gateway/protoc_gen_openapiv2/options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:16.582760 wechaty-grpc-1.5.dev4/src/wechaty_grpc/wechaty/
+-rw-r--r--   0 runner    (1001) docker     (123)    87750 2023-06-29 08:12:14.000000 wechaty-grpc-1.5.dev4/src/wechaty_grpc/wechaty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:16.582760 wechaty-grpc-1.5.dev4/src/wechaty_grpc/wechaty/puppet/
+-rw-r--r--   0 runner    (1001) docker     (123)    41958 2023-06-29 08:12:14.000000 wechaty-grpc-1.5.dev4/src/wechaty_grpc/wechaty/puppet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:12:16.582760 wechaty-grpc-1.5.dev4/src/wechaty_grpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-06-29 08:12:16.000000 wechaty-grpc-1.5.dev4/src/wechaty_grpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-29 08:12:16.000000 wechaty-grpc-1.5.dev4/src/wechaty_grpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:12:16.000000 wechaty-grpc-1.5.dev4/src/wechaty_grpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 08:12:16.000000 wechaty-grpc-1.5.dev4/src/wechaty_grpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 08:12:16.000000 wechaty-grpc-1.5.dev4/src/wechaty_grpc.egg-info/top_level.txt
```

### Comparing `wechaty-grpc-1.5.dev2/PKG-INFO` & `wechaty-grpc-1.5.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wechaty-grpc
-Version: 1.5.dev2
+Version: 1.5.dev4
 Summary: Wechaty Puppet Service gRPC API
 Home-page: https://github.com/wechaty/grpc
 Author: Huan LI (李卓桓)
 Author-email: zixia@zixia.net
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
@@ -138,15 +138,15 @@
 
 **Maintainer:**
 
 - [@diaozxin007](https://github.com/diaozxin007) - Zhengxin DIAO (刁政欣)
 
 ### PHP
 
-[github.com/wechaty/php-grpc](https://github.comwechaty/php-grpc)
+[github.com/wechaty/php-grpc](https://github.com/wechaty/php-grpc)
 
 **Maintainer:**
 
 - [@zhangchunsheng](https://github.com/zhangchunsheng) - Chunsheng ZHANG (张春生)
 
 ### CSharp
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wechaty-grpc Version: 1.5.dev2 Summary: Wechaty
+Metadata-Version: 2.1 Name: wechaty-grpc Version: 1.5.dev4 Summary: Wechaty
 Puppet Service gRPC API Home-page: https://github.com/wechaty/grpc Author: Huan
 LI (æåæ¡) Author-email: zixia@zixia.net License: Apache-2.0 Platform:
 UNKNOWN Classifier: Programming Language :: Python :: 3.7 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown
                      [docs/images/wechaty-grpc-logo.svg]
                           ****** Wechaty gRPC ******
@@ -71,15 +71,15 @@
 Jingjing WU (å´äº¬äº¬) ### Go [github.com/wechaty/go-grpc](https://github.com/
 wechaty/go-grpc) **Maintainer:** - [@dchaofei](https://github.com/dchaofei) -
 Chaofei DING (ä¸è¶é£) ### Java [https://mvnrepository.com/artifact/
 io.github.wechaty/grpc](https://mvnrepository.com/artifact/io.github.wechaty/
 grpc) **Maven:** ```xml  io.github.wechaty 0.11.25 grpc  ``` **Gradle:**
 ```groovy compile 'io.github.wechaty:grpc:0.11.25' ``` **Maintainer:** -
 [@diaozxin007](https://github.com/diaozxin007) - Zhengxin DIAO (åæ¿æ¬£) ###
-PHP [github.com/wechaty/php-grpc](https://github.comwechaty/php-grpc)
+PHP [github.com/wechaty/php-grpc](https://github.com/wechaty/php-grpc)
 **Maintainer:** - [@zhangchunsheng](https://github.com/zhangchunsheng) -
 Chunsheng ZHANG (å¼ æ¥ç) ### CSharp [Wechaty.Grpc @ Nuget](https://
 www.nuget.org/packages/Wechaty.Grpc) **Maintainer:** - [@Darren](https://
 github.com/jesn) - Darren (éæ³¢) ## Development ### Debug - [GUI Client for
 GRPC Services](https://github.com/uw-labs/bloomrpc) - BloomRPC aims to give the
 simplest and efficient developer experience for exploring and querying your
 GRPC services. (Inspired by Postman and GraphQL Playground) - [A gRPC CLI
```

### Comparing `wechaty-grpc-1.5.dev2/setup.py` & `wechaty-grpc-1.5.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `wechaty-grpc-1.5.dev2/src/wechaty_grpc/google/api/__init__.py` & `wechaty-grpc-1.5.dev4/src/wechaty_grpc/google/api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: google/api/annotations.proto, google/api/http.proto
 # plugin: python-betterproto
+# This file has been @generated
+
 from dataclasses import dataclass
 from typing import List
 
 import betterproto
-from betterproto.grpc.grpclib_server import ServiceBase
 
 
 @dataclass(eq=False, repr=False)
 class Http(betterproto.Message):
     """
     Defines the HTTP configuration for an API service. It contains a list of
     [HttpRule][google.api.HttpRule], each specifying the mapping of an RPC
     method to one or more HTTP REST API methods.
     """
 
-    # A list of HTTP configuration rules that apply to individual API methods.
-    # **NOTE:** All service configuration rules follow "last one wins" order.
     rules: List["HttpRule"] = betterproto.message_field(1)
-    # When set to true, URL path parameters will be fully URI-decoded except in
-    # cases of single segment matches in reserved expansion, where "%2F" will be
-    # left encoded. The default behavior is to not decode RFC 6570 reserved
-    # characters in multi segment matches.
+    """
+    A list of HTTP configuration rules that apply to individual API methods.
+    **NOTE:** All service configuration rules follow "last one wins" order.
+    """
+
     fully_decode_reserved_expansion: bool = betterproto.bool_field(2)
+    """
+    When set to true, URL path parameters will be fully URI-decoded except in
+    cases of single segment matches in reserved expansion, where "%2F" will be
+    left encoded. The default behavior is to not decode RFC 6570 reserved
+    characters in multi segment matches.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class HttpRule(betterproto.Message):
     """
     # gRPC Transcoding gRPC Transcoding is a feature for mapping between a gRPC
     method and one or more HTTP REST endpoints. It allows developers to build a
@@ -106,23 +112,23 @@
     user_id = 2;     } This enables the following two alternative HTTP JSON to
     RPC mappings: HTTP | gRPC -----|----- `GET /v1/messages/123456` |
     `GetMessage(message_id: "123456")` `GET /v1/users/me/messages/123456` |
     `GetMessage(user_id: "me" message_id: "123456")` ## Rules for HTTP mapping
     1. Leaf request fields (recursive expansion nested messages in the request
     message) are classified into three categories:    - Fields referred by the
     path template. They are passed via the URL path.    - Fields referred by
-    the [HttpRule.body][google.api.HttpRule.body]. They are passed via the HTTP
-    request body.    - All other fields are passed via the URL query
+    the [HttpRule.body][google.api.HttpRule.body]. They    are passed via the
+    HTTP      request body.    - All other fields are passed via the URL query
     parameters, and the      parameter name is the field path in the request
     message. A repeated      field can be represented as multiple query
     parameters under the same      name.  2. If
-    [HttpRule.body][google.api.HttpRule.body] is "*", there is no URL query
+    [HttpRule.body][google.api.HttpRule.body] is "*", there is no URL  query
     parameter, all fields     are passed via URL path and HTTP request body.
     3. If [HttpRule.body][google.api.HttpRule.body] is omitted, there is no
-    HTTP request body, all     fields are passed via URL path and URL query
+    HTTP  request body, all     fields are passed via URL path and URL query
     parameters. ### Path template syntax     Template = "/" Segments [ Verb ] ;
     Segments = Segment { "/" Segment } ;     Segment  = "*" | "**" | LITERAL |
     Variable ;     Variable = "{" FieldPath [ "=" Segments ] "}" ;
     FieldPath = IDENT { "." IDENT } ;     Verb     = ":" LITERAL ; The syntax
     `*` matches a single URL path segment. The syntax `**` matches zero or more
     URL path segments, which must be the last part of the URL path except the
     `Verb`. The syntax `Variable` matches part of the URL path as specified by
@@ -175,50 +181,74 @@
     must not be mapped to URL query parameters, because no client library can
     support such complicated mapping. If an API needs to use a JSON array for
     request or response body, it can map the request or response body to a
     repeated field. However, some gRPC Transcoding implementations may not
     support this feature.
     """
 
-    # Selects a method to which this rule applies. Refer to
-    # [selector][google.api.DocumentationRule.selector] for syntax details.
     selector: str = betterproto.string_field(1)
-    # Maps to HTTP GET. Used for listing and getting information about resources.
+    """
+    Selects a method to which this rule applies. Refer to
+    [selector][google.api.DocumentationRule.selector] for syntax details.
+    """
+
     get: str = betterproto.string_field(2, group="pattern")
-    # Maps to HTTP PUT. Used for replacing a resource.
+    """
+    Maps to HTTP GET. Used for listing and getting information about resources.
+    """
+
     put: str = betterproto.string_field(3, group="pattern")
-    # Maps to HTTP POST. Used for creating a resource or performing an action.
+    """Maps to HTTP PUT. Used for replacing a resource."""
+
     post: str = betterproto.string_field(4, group="pattern")
-    # Maps to HTTP DELETE. Used for deleting a resource.
+    """
+    Maps to HTTP POST. Used for creating a resource or performing an action.
+    """
+
     delete: str = betterproto.string_field(5, group="pattern")
-    # Maps to HTTP PATCH. Used for updating a resource.
+    """Maps to HTTP DELETE. Used for deleting a resource."""
+
     patch: str = betterproto.string_field(6, group="pattern")
-    # The custom pattern is used for specifying an HTTP method that is not
-    # included in the `pattern` field, such as HEAD, or "*" to leave the HTTP
-    # method unspecified for this rule. The wild-card rule is useful for services
-    # that provide content to Web (HTML) clients.
+    """Maps to HTTP PATCH. Used for updating a resource."""
+
     custom: "CustomHttpPattern" = betterproto.message_field(8, group="pattern")
-    # The name of the request field whose value is mapped to the HTTP request
-    # body, or `*` for mapping all request fields not captured by the path
-    # pattern to the HTTP body, or omitted for not having any HTTP request body.
-    # NOTE: the referred field must be present at the top-level of the request
-    # message type.
+    """
+    The custom pattern is used for specifying an HTTP method that is not
+    included in the `pattern` field, such as HEAD, or "*" to leave the HTTP
+    method unspecified for this rule. The wild-card rule is useful for services
+    that provide content to Web (HTML) clients.
+    """
+
     body: str = betterproto.string_field(7)
-    # Optional. The name of the response field whose value is mapped to the HTTP
-    # response body. When omitted, the entire response message will be used as
-    # the HTTP response body. NOTE: The referred field must be present at the
-    # top-level of the response message type.
+    """
+    The name of the request field whose value is mapped to the HTTP request
+    body, or `*` for mapping all request fields not captured by the path
+    pattern to the HTTP body, or omitted for not having any HTTP request body.
+    NOTE: the referred field must be present at the top-level of the request
+    message type.
+    """
+
     response_body: str = betterproto.string_field(12)
-    # Additional HTTP bindings for the selector. Nested bindings must not contain
-    # an `additional_bindings` field themselves (that is, the nesting may only be
-    # one level deep).
+    """
+    Optional. The name of the response field whose value is mapped to the HTTP
+    response body. When omitted, the entire response message will be used as
+    the HTTP response body. NOTE: The referred field must be present at the
+    top-level of the response message type.
+    """
+
     additional_bindings: List["HttpRule"] = betterproto.message_field(11)
+    """
+    Additional HTTP bindings for the selector. Nested bindings must not contain
+    an `additional_bindings` field themselves (that is, the nesting may only be
+    one level deep).
+    """
 
 
 @dataclass(eq=False, repr=False)
 class CustomHttpPattern(betterproto.Message):
     """A custom pattern is used for defining custom HTTP verb."""
 
-    # The name of this custom HTTP verb.
     kind: str = betterproto.string_field(1)
-    # The path matched by this custom verb.
+    """The name of this custom HTTP verb."""
+
     path: str = betterproto.string_field(2)
+    """The path matched by this custom verb."""
```

### Comparing `wechaty-grpc-1.5.dev2/src/wechaty_grpc/grpc/gateway/protoc_gen_openapiv2/options/__init__.py` & `wechaty-grpc-1.5.dev4/src/wechaty_grpc/grpc/gateway/protoc_gen_openapiv2/options/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: protoc-gen-openapiv2/options/annotations.proto, protoc-gen-openapiv2/options/openapiv2.proto
 # plugin: python-betterproto
+# This file has been @generated
+
 from dataclasses import dataclass
-from typing import Dict, List
+from typing import (
+    Dict,
+    List,
+)
 
 import betterproto
-from betterproto.grpc.grpclib_server import ServiceBase
+import betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
 
 class Scheme(betterproto.Enum):
     """
     Scheme describes the schemes supported by the OpenAPI Swagger and Operation
     objects.
     """
@@ -17,112 +22,180 @@
     UNKNOWN = 0
     HTTP = 1
     HTTPS = 2
     WS = 3
     WSS = 4
 
 
+class HeaderParameterType(betterproto.Enum):
+    """
+    `Type` is a a supported HTTP header type. See
+    https://swagger.io/specification/v2/#parameterType.
+    """
+
+    UNKNOWN = 0
+    STRING = 1
+    NUMBER = 2
+    INTEGER = 3
+    BOOLEAN = 4
+
+
 class JsonSchemaJsonSchemaSimpleTypes(betterproto.Enum):
     UNKNOWN = 0
     ARRAY = 1
     BOOLEAN = 2
     INTEGER = 3
     NULL = 4
     NUMBER = 5
     OBJECT = 6
     STRING = 7
 
 
 class SecuritySchemeType(betterproto.Enum):
+    """
+    The type of the security scheme. Valid values are "basic", "apiKey" or
+    "oauth2".
+    """
+
     TYPE_INVALID = 0
     TYPE_BASIC = 1
     TYPE_API_KEY = 2
     TYPE_OAUTH2 = 3
 
 
 class SecuritySchemeIn(betterproto.Enum):
+    """The location of the API key. Valid values are "query" or "header"."""
+
     IN_INVALID = 0
     IN_QUERY = 1
     IN_HEADER = 2
 
 
 class SecuritySchemeFlow(betterproto.Enum):
+    """
+    The flow used by the OAuth2 security scheme. Valid values are "implicit",
+    "password", "application" or "accessCode".
+    """
+
     FLOW_INVALID = 0
     FLOW_IMPLICIT = 1
     FLOW_PASSWORD = 2
     FLOW_APPLICATION = 3
     FLOW_ACCESS_CODE = 4
 
 
 @dataclass(eq=False, repr=False)
 class Swagger(betterproto.Message):
     """
     `Swagger` is a representation of OpenAPI v2 specification's Swagger object.
     See: https://github.com/OAI/OpenAPI-
     Specification/blob/3.0.0/versions/2.0.md#swaggerObject Example:  option
     (grpc.gateway.protoc_gen_openapiv2.options.openapiv2_swagger) = {    info:
-    {      title: "Echo API";      version: "1.0";      description: ";
+    {      title: "Echo API";      version: "1.0";      description: "";
     contact: {        name: "gRPC-Gateway project";        url:
     "https://github.com/grpc-ecosystem/grpc-gateway";        email:
     "none@example.com";      };      license: {        name: "BSD 3-Clause
     License";        url: "https://github.com/grpc-ecosystem/grpc-
-    gateway/blob/master/LICENSE.txt";      };    };    schemes: HTTPS;
+    gateway/blob/main/LICENSE.txt";      };    };    schemes: HTTPS;
     consumes: "application/json";    produces: "application/json";  };
     """
 
-    # Specifies the OpenAPI Specification version being used. It can be used by
-    # the OpenAPI UI and other clients to interpret the API listing. The value
-    # MUST be "2.0".
     swagger: str = betterproto.string_field(1)
-    # Provides metadata about the API. The metadata can be used by the clients if
-    # needed.
+    """
+    Specifies the OpenAPI Specification version being used. It can be used by
+    the OpenAPI UI and other clients to interpret the API listing. The value
+    MUST be "2.0".
+    """
+
     info: "Info" = betterproto.message_field(2)
-    # The host (name or ip) serving the API. This MUST be the host only and does
-    # not include the scheme nor sub-paths. It MAY include a port. If the host is
-    # not included, the host serving the documentation is to be used (including
-    # the port). The host does not support path templating.
+    """
+    Provides metadata about the API. The metadata can be used by the clients if
+    needed.
+    """
+
     host: str = betterproto.string_field(3)
-    # The base path on which the API is served, which is relative to the host. If
-    # it is not included, the API is served directly under the host. The value
-    # MUST start with a leading slash (/). The basePath does not support path
-    # templating. Note that using `base_path` does not change the endpoint paths
-    # that are generated in the resulting OpenAPI file. If you wish to use
-    # `base_path` with relatively generated OpenAPI paths, the `base_path` prefix
-    # must be manually removed from your `google.api.http` paths and your code
-    # changed to serve the API from the `base_path`.
+    """
+    The host (name or ip) serving the API. This MUST be the host only and does
+    not include the scheme nor sub-paths. It MAY include a port. If the host is
+    not included, the host serving the documentation is to be used (including
+    the port). The host does not support path templating.
+    """
+
     base_path: str = betterproto.string_field(4)
-    # The transfer protocol of the API. Values MUST be from the list: "http",
-    # "https", "ws", "wss". If the schemes is not included, the default scheme to
-    # be used is the one used to access the OpenAPI definition itself.
+    """
+    The base path on which the API is served, which is relative to the host. If
+    it is not included, the API is served directly under the host. The value
+    MUST start with a leading slash (/). The basePath does not support path
+    templating. Note that using `base_path` does not change the endpoint paths
+    that are generated in the resulting OpenAPI file. If you wish to use
+    `base_path` with relatively generated OpenAPI paths, the `base_path` prefix
+    must be manually removed from your `google.api.http` paths and your code
+    changed to serve the API from the `base_path`.
+    """
+
     schemes: List["Scheme"] = betterproto.enum_field(5)
-    # A list of MIME types the APIs can consume. This is global to all APIs but
-    # can be overridden on specific API calls. Value MUST be as described under
-    # Mime Types.
+    """
+    The transfer protocol of the API. Values MUST be from the list: "http",
+    "https", "ws", "wss". If the schemes is not included, the default scheme to
+    be used is the one used to access the OpenAPI definition itself.
+    """
+
     consumes: List[str] = betterproto.string_field(6)
-    # A list of MIME types the APIs can produce. This is global to all APIs but
-    # can be overridden on specific API calls. Value MUST be as described under
-    # Mime Types.
+    """
+    A list of MIME types the APIs can consume. This is global to all APIs but
+    can be overridden on specific API calls. Value MUST be as described under
+    Mime Types.
+    """
+
     produces: List[str] = betterproto.string_field(7)
-    # An object to hold responses that can be used across operations. This
-    # property does not define global responses for all operations.
+    """
+    A list of MIME types the APIs can produce. This is global to all APIs but
+    can be overridden on specific API calls. Value MUST be as described under
+    Mime Types.
+    """
+
     responses: Dict[str, "Response"] = betterproto.map_field(
         10, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
     )
-    # Security scheme definitions that can be used across the specification.
+    """
+    An object to hold responses that can be used across operations. This
+    property does not define global responses for all operations.
+    """
+
     security_definitions: "SecurityDefinitions" = betterproto.message_field(11)
-    # A declaration of which security schemes are applied for the API as a whole.
-    # The list of values describes alternative security schemes that can be used
-    # (that is, there is a logical OR between the security requirements).
-    # Individual operations can override this definition.
+    """
+    Security scheme definitions that can be used across the specification.
+    """
+
     security: List["SecurityRequirement"] = betterproto.message_field(12)
-    # Additional external documentation.
+    """
+    A declaration of which security schemes are applied for the API as a whole.
+    The list of values describes alternative security schemes that can be used
+    (that is, there is a logical OR between the security requirements).
+    Individual operations can override this definition.
+    """
+
+    tags: List["Tag"] = betterproto.message_field(13)
+    """
+    A list of tags for API documentation control. Tags can be used for logical
+    grouping of operations by resources or any other qualifier.
+    """
+
     external_docs: "ExternalDocumentation" = betterproto.message_field(14)
+    """Additional external documentation."""
+
     extensions: Dict[
         str, "betterproto_lib_google_protobuf.Value"
     ] = betterproto.map_field(15, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE)
+    """
+    Custom properties that start with "x-" such as "x-foo" used to describe
+    extra functionality that is not covered by the standard OpenAPI
+    Specification. See: https://swagger.io/docs/specification/2-0/swagger-
+    extensions/
+    """
 
 
 @dataclass(eq=False, repr=False)
 class Operation(betterproto.Message):
     """
     `Operation` is a representation of OpenAPI v2 specification's Operation
     object. See: https://github.com/OAI/OpenAPI-
@@ -131,236 +204,393 @@
     option (google.api.http) = {        get: "/v1/example/echo/{id}"      };
     option (grpc.gateway.protoc_gen_openapiv2.options.openapiv2_operation) = {
     summary: "Get a message.";        operation_id: "getMessage";        tags:
     "echo";        responses: {          key: "200"            value: {
     description: "OK";          }        }      };    }  }
     """
 
-    # A list of tags for API documentation control. Tags can be used for logical
-    # grouping of operations by resources or any other qualifier.
     tags: List[str] = betterproto.string_field(1)
-    # A short summary of what the operation does. For maximum readability in the
-    # swagger-ui, this field SHOULD be less than 120 characters.
+    """
+    A list of tags for API documentation control. Tags can be used for logical
+    grouping of operations by resources or any other qualifier.
+    """
+
     summary: str = betterproto.string_field(2)
-    # A verbose explanation of the operation behavior. GFM syntax can be used for
-    # rich text representation.
+    """
+    A short summary of what the operation does. For maximum readability in the
+    swagger-ui, this field SHOULD be less than 120 characters.
+    """
+
     description: str = betterproto.string_field(3)
-    # Additional external documentation for this operation.
+    """
+    A verbose explanation of the operation behavior. GFM syntax can be used for
+    rich text representation.
+    """
+
     external_docs: "ExternalDocumentation" = betterproto.message_field(4)
-    # Unique string used to identify the operation. The id MUST be unique among
-    # all operations described in the API. Tools and libraries MAY use the
-    # operationId to uniquely identify an operation, therefore, it is recommended
-    # to follow common programming naming conventions.
+    """Additional external documentation for this operation."""
+
     operation_id: str = betterproto.string_field(5)
-    # A list of MIME types the operation can consume. This overrides the consumes
-    # definition at the OpenAPI Object. An empty value MAY be used to clear the
-    # global definition. Value MUST be as described under Mime Types.
+    """
+    Unique string used to identify the operation. The id MUST be unique among
+    all operations described in the API. Tools and libraries MAY use the
+    operationId to uniquely identify an operation, therefore, it is recommended
+    to follow common programming naming conventions.
+    """
+
     consumes: List[str] = betterproto.string_field(6)
-    # A list of MIME types the operation can produce. This overrides the produces
-    # definition at the OpenAPI Object. An empty value MAY be used to clear the
-    # global definition. Value MUST be as described under Mime Types.
+    """
+    A list of MIME types the operation can consume. This overrides the consumes
+    definition at the OpenAPI Object. An empty value MAY be used to clear the
+    global definition. Value MUST be as described under Mime Types.
+    """
+
     produces: List[str] = betterproto.string_field(7)
-    # The list of possible responses as they are returned from executing this
-    # operation.
+    """
+    A list of MIME types the operation can produce. This overrides the produces
+    definition at the OpenAPI Object. An empty value MAY be used to clear the
+    global definition. Value MUST be as described under Mime Types.
+    """
+
     responses: Dict[str, "Response"] = betterproto.map_field(
         9, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
     )
-    # The transfer protocol for the operation. Values MUST be from the list:
-    # "http", "https", "ws", "wss". The value overrides the OpenAPI Object
-    # schemes definition.
+    """
+    The list of possible responses as they are returned from executing this
+    operation.
+    """
+
     schemes: List["Scheme"] = betterproto.enum_field(10)
-    # Declares this operation to be deprecated. Usage of the declared operation
-    # should be refrained. Default value is false.
+    """
+    The transfer protocol for the operation. Values MUST be from the list:
+    "http", "https", "ws", "wss". The value overrides the OpenAPI Object
+    schemes definition.
+    """
+
     deprecated: bool = betterproto.bool_field(11)
-    # A declaration of which security schemes are applied for this operation. The
-    # list of values describes alternative security schemes that can be used
-    # (that is, there is a logical OR between the security requirements). This
-    # definition overrides any declared top-level security. To remove a top-level
-    # security declaration, an empty array can be used.
+    """
+    Declares this operation to be deprecated. Usage of the declared operation
+    should be refrained. Default value is false.
+    """
+
     security: List["SecurityRequirement"] = betterproto.message_field(12)
+    """
+    A declaration of which security schemes are applied for this operation. The
+    list of values describes alternative security schemes that can be used
+    (that is, there is a logical OR between the security requirements). This
+    definition overrides any declared top-level security. To remove a top-level
+    security declaration, an empty array can be used.
+    """
+
     extensions: Dict[
         str, "betterproto_lib_google_protobuf.Value"
     ] = betterproto.map_field(13, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE)
+    """
+    Custom properties that start with "x-" such as "x-foo" used to describe
+    extra functionality that is not covered by the standard OpenAPI
+    Specification. See: https://swagger.io/docs/specification/2-0/swagger-
+    extensions/
+    """
+
+    parameters: "Parameters" = betterproto.message_field(14)
+    """
+    Custom parameters such as HTTP request headers. See:
+    https://swagger.io/docs/specification/2-0/describing-parameters/ and
+    https://swagger.io/specification/v2/#parameter-object.
+    """
+
+
+@dataclass(eq=False, repr=False)
+class Parameters(betterproto.Message):
+    """
+    `Parameters` is a representation of OpenAPI v2 specification's parameters
+    object. Note: This technically breaks compatibility with the OpenAPI 2
+    definition structure as we only allow header parameters to be set here
+    since we do not want users specifying custom non-header parameters beyond
+    those inferred from the Protobuf schema. See:
+    https://swagger.io/specification/v2/#parameter-object
+    """
+
+    headers: List["HeaderParameter"] = betterproto.message_field(1)
+    """
+    `Headers` is one or more HTTP header parameter. See:
+    https://swagger.io/docs/specification/2-0/describing-parameters/#header-
+    parameters
+    """
+
+
+@dataclass(eq=False, repr=False)
+class HeaderParameter(betterproto.Message):
+    """
+    `HeaderParameter` a HTTP header parameter. See:
+    https://swagger.io/specification/v2/#parameter-object
+    """
+
+    name: str = betterproto.string_field(1)
+    """`Name` is the header name."""
+
+    description: str = betterproto.string_field(2)
+    """`Description` is a short description of the header."""
+
+    type: "HeaderParameterType" = betterproto.enum_field(3)
+    """
+    `Type` is the type of the object. The value MUST be one of "string",
+    "number", "integer", or "boolean". The "array" type is not supported. See:
+    https://swagger.io/specification/v2/#parameterType.
+    """
+
+    format: str = betterproto.string_field(4)
+    """`Format` The extending format for the previously mentioned type."""
+
+    required: bool = betterproto.bool_field(5)
+    """`Required` indicates if the header is optional"""
 
 
 @dataclass(eq=False, repr=False)
 class Header(betterproto.Message):
     """
     `Header` is a representation of OpenAPI v2 specification's Header object.
     See: https://github.com/OAI/OpenAPI-
     Specification/blob/3.0.0/versions/2.0.md#headerObject
     """
 
-    # `Description` is a short description of the header.
     description: str = betterproto.string_field(1)
-    # The type of the object. The value MUST be one of "string", "number",
-    # "integer", or "boolean". The "array" type is not supported.
+    """`Description` is a short description of the header."""
+
     type: str = betterproto.string_field(2)
-    # `Format` The extending format for the previously mentioned type.
+    """
+    The type of the object. The value MUST be one of "string", "number",
+    "integer", or "boolean". The "array" type is not supported.
+    """
+
     format: str = betterproto.string_field(3)
-    # `Default` Declares the value of the header that the server will use if none
-    # is provided. See: https://tools.ietf.org/html/draft-fge-json-schema-
-    # validation-00#section-6.2. Unlike JSON Schema this value MUST conform to
-    # the defined type for the header.
+    """`Format` The extending format for the previously mentioned type."""
+
     default: str = betterproto.string_field(6)
-    # 'Pattern' See https://tools.ietf.org/html/draft-fge-json-schema-
-    # validation-00#section-5.2.3.
+    """
+    `Default` Declares the value of the header that the server will use if none
+    is provided. See: https://tools.ietf.org/html/draft-fge-json-schema-
+    validation-00#section-6.2. Unlike JSON Schema this value MUST conform to
+    the defined type for the header.
+    """
+
     pattern: str = betterproto.string_field(13)
+    """
+    'Pattern' See https://tools.ietf.org/html/draft-fge-json-schema-
+    validation-00#section-5.2.3.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class Response(betterproto.Message):
     """
     `Response` is a representation of OpenAPI v2 specification's Response
     object. See: https://github.com/OAI/OpenAPI-
     Specification/blob/3.0.0/versions/2.0.md#responseObject
     """
 
-    # `Description` is a short description of the response. GFM syntax can be
-    # used for rich text representation.
     description: str = betterproto.string_field(1)
-    # `Schema` optionally defines the structure of the response. If `Schema` is
-    # not provided, it means there is no content to the response.
+    """
+    `Description` is a short description of the response. GFM syntax can be
+    used for rich text representation.
+    """
+
     schema: "Schema" = betterproto.message_field(2)
-    # `Headers` A list of headers that are sent with the response. `Header` name
-    # is expected to be a string in the canonical format of the MIME header key
-    # See: https://golang.org/pkg/net/textproto/#CanonicalMIMEHeaderKey
+    """
+    `Schema` optionally defines the structure of the response. If `Schema` is
+    not provided, it means there is no content to the response.
+    """
+
     headers: Dict[str, "Header"] = betterproto.map_field(
         3, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
     )
-    # `Examples` gives per-mimetype response examples. See:
-    # https://github.com/OAI/OpenAPI-
-    # Specification/blob/3.0.0/versions/2.0.md#example-object
+    """
+    `Headers` A list of headers that are sent with the response. `Header` name
+    is expected to be a string in the canonical format of the MIME header key
+    See: https://golang.org/pkg/net/textproto/#CanonicalMIMEHeaderKey
+    """
+
     examples: Dict[str, str] = betterproto.map_field(
         4, betterproto.TYPE_STRING, betterproto.TYPE_STRING
     )
+    """
+    `Examples` gives per-mimetype response examples. See:
+    https://github.com/OAI/OpenAPI-
+    Specification/blob/3.0.0/versions/2.0.md#example-object
+    """
+
     extensions: Dict[
         str, "betterproto_lib_google_protobuf.Value"
     ] = betterproto.map_field(5, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE)
+    """
+    Custom properties that start with "x-" such as "x-foo" used to describe
+    extra functionality that is not covered by the standard OpenAPI
+    Specification. See: https://swagger.io/docs/specification/2-0/swagger-
+    extensions/
+    """
 
 
 @dataclass(eq=False, repr=False)
 class Info(betterproto.Message):
     """
     `Info` is a representation of OpenAPI v2 specification's Info object. See:
     https://github.com/OAI/OpenAPI-
     Specification/blob/3.0.0/versions/2.0.md#infoObject Example:  option
     (grpc.gateway.protoc_gen_openapiv2.options.openapiv2_swagger) = {    info:
-    {      title: "Echo API";      version: "1.0";      description: ";
+    {      title: "Echo API";      version: "1.0";      description: "";
     contact: {        name: "gRPC-Gateway project";        url:
     "https://github.com/grpc-ecosystem/grpc-gateway";        email:
     "none@example.com";      };      license: {        name: "BSD 3-Clause
     License";        url: "https://github.com/grpc-ecosystem/grpc-
-    gateway/blob/master/LICENSE.txt";      };    };    ...  };
+    gateway/blob/main/LICENSE.txt";      };    };    ...  };
     """
 
-    # The title of the application.
     title: str = betterproto.string_field(1)
-    # A short description of the application. GFM syntax can be used for rich
-    # text representation.
+    """The title of the application."""
+
     description: str = betterproto.string_field(2)
-    # The Terms of Service for the API.
+    """
+    A short description of the application. GFM syntax can be used for rich
+    text representation.
+    """
+
     terms_of_service: str = betterproto.string_field(3)
-    # The contact information for the exposed API.
+    """The Terms of Service for the API."""
+
     contact: "Contact" = betterproto.message_field(4)
-    # The license information for the exposed API.
+    """The contact information for the exposed API."""
+
     license: "License" = betterproto.message_field(5)
-    # Provides the version of the application API (not to be confused with the
-    # specification version).
+    """The license information for the exposed API."""
+
     version: str = betterproto.string_field(6)
+    """
+    Provides the version of the application API (not to be confused with the
+    specification version).
+    """
+
     extensions: Dict[
         str, "betterproto_lib_google_protobuf.Value"
     ] = betterproto.map_field(7, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE)
+    """
+    Custom properties that start with "x-" such as "x-foo" used to describe
+    extra functionality that is not covered by the standard OpenAPI
+    Specification. See: https://swagger.io/docs/specification/2-0/swagger-
+    extensions/
+    """
 
 
 @dataclass(eq=False, repr=False)
 class Contact(betterproto.Message):
     """
     `Contact` is a representation of OpenAPI v2 specification's Contact object.
     See: https://github.com/OAI/OpenAPI-
     Specification/blob/3.0.0/versions/2.0.md#contactObject Example:  option
     (grpc.gateway.protoc_gen_openapiv2.options.openapiv2_swagger) = {    info:
     {      ...      contact: {        name: "gRPC-Gateway project";        url:
     "https://github.com/grpc-ecosystem/grpc-gateway";        email:
     "none@example.com";      };      ...    };    ...  };
     """
 
-    # The identifying name of the contact person/organization.
     name: str = betterproto.string_field(1)
-    # The URL pointing to the contact information. MUST be in the format of a
-    # URL.
+    """The identifying name of the contact person/organization."""
+
     url: str = betterproto.string_field(2)
-    # The email address of the contact person/organization. MUST be in the format
-    # of an email address.
+    """
+    The URL pointing to the contact information. MUST be in the format of a
+    URL.
+    """
+
     email: str = betterproto.string_field(3)
+    """
+    The email address of the contact person/organization. MUST be in the format
+    of an email address.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class License(betterproto.Message):
     """
     `License` is a representation of OpenAPI v2 specification's License object.
     See: https://github.com/OAI/OpenAPI-
     Specification/blob/3.0.0/versions/2.0.md#licenseObject Example:  option
     (grpc.gateway.protoc_gen_openapiv2.options.openapiv2_swagger) = {    info:
     {      ...      license: {        name: "BSD 3-Clause License";        url:
-    "https://github.com/grpc-ecosystem/grpc-gateway/blob/master/LICENSE.txt";
+    "https://github.com/grpc-ecosystem/grpc-gateway/blob/main/LICENSE.txt";
     };      ...    };    ...  };
     """
 
-    # The license name used for the API.
     name: str = betterproto.string_field(1)
-    # A URL to the license used for the API. MUST be in the format of a URL.
+    """The license name used for the API."""
+
     url: str = betterproto.string_field(2)
+    """
+    A URL to the license used for the API. MUST be in the format of a URL.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class ExternalDocumentation(betterproto.Message):
     """
     `ExternalDocumentation` is a representation of OpenAPI v2 specification's
     ExternalDocumentation object. See: https://github.com/OAI/OpenAPI-
     Specification/blob/3.0.0/versions/2.0.md#externalDocumentationObject
     Example:  option
     (grpc.gateway.protoc_gen_openapiv2.options.openapiv2_swagger) = {    ...
     external_docs: {      description: "More about gRPC-Gateway";      url:
     "https://github.com/grpc-ecosystem/grpc-gateway";    }    ...  };
     """
 
-    # A short description of the target documentation. GFM syntax can be used for
-    # rich text representation.
     description: str = betterproto.string_field(1)
-    # The URL for the target documentation. Value MUST be in the format of a URL.
+    """
+    A short description of the target documentation. GFM syntax can be used for
+    rich text representation.
+    """
+
     url: str = betterproto.string_field(2)
+    """
+    The URL for the target documentation. Value MUST be in the format of a URL.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class Schema(betterproto.Message):
     """
     `Schema` is a representation of OpenAPI v2 specification's Schema object.
     See: https://github.com/OAI/OpenAPI-
     Specification/blob/3.0.0/versions/2.0.md#schemaObject
     """
 
     json_schema: "JsonSchema" = betterproto.message_field(1)
-    # Adds support for polymorphism. The discriminator is the schema property
-    # name that is used to differentiate between other schema that inherit this
-    # schema. The property name used MUST be defined at this schema and it MUST
-    # be in the required property list. When used, the value MUST be the name of
-    # this schema or any schema that inherits it.
     discriminator: str = betterproto.string_field(2)
-    # Relevant only for Schema "properties" definitions. Declares the property as
-    # "read only". This means that it MAY be sent as part of a response but MUST
-    # NOT be sent as part of the request. Properties marked as readOnly being
-    # true SHOULD NOT be in the required list of the defined schema. Default
-    # value is false.
+    """
+    Adds support for polymorphism. The discriminator is the schema property
+    name that is used to differentiate between other schema that inherit this
+    schema. The property name used MUST be defined at this schema and it MUST
+    be in the required property list. When used, the value MUST be the name of
+    this schema or any schema that inherits it.
+    """
+
     read_only: bool = betterproto.bool_field(3)
-    # Additional external documentation for this schema.
+    """
+    Relevant only for Schema "properties" definitions. Declares the property as
+    "read only". This means that it MAY be sent as part of a response but MUST
+    NOT be sent as part of the request. Properties marked as readOnly being
+    true SHOULD NOT be in the required list of the defined schema. Default
+    value is false.
+    """
+
     external_docs: "ExternalDocumentation" = betterproto.message_field(5)
-    # A free-form property to include an example of an instance for this schema
-    # in JSON. This is copied verbatim to the output.
+    """Additional external documentation for this schema."""
+
     example: str = betterproto.string_field(6)
+    """
+    A free-form property to include an example of an instance for this schema
+    in JSON. This is copied verbatim to the output.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class JsonSchema(betterproto.Message):
     """
     `JSONSchema` represents properties from JSON Schema taken, and as used, in
     the OpenAPI v2 spec. This includes changes made by OpenAPI v2. See:
@@ -373,152 +603,232 @@
     json_schema: {        title: "SimpleMessage"        description: "A simple
     message."        required: ["id"]      }    };    // Id represents the
     message identifier.    string id = 1; [
     (grpc.gateway.protoc_gen_openapiv2.options.openapiv2_field) = {
     description: "The unique identifier of the simple message."        }];  }
     """
 
-    # Ref is used to define an external reference to include in the message. This
-    # could be a fully qualified proto message reference, and that type must be
-    # imported into the protofile. If no message is identified, the Ref will be
-    # used verbatim in the output. For example:  `ref:
-    # ".google.protobuf.Timestamp"`.
     ref: str = betterproto.string_field(3)
-    # The title of the schema.
+    """
+    Ref is used to define an external reference to include in the message. This
+    could be a fully qualified proto message reference, and that type must be
+    imported into the protofile. If no message is identified, the Ref will be
+    used verbatim in the output. For example:  `ref:
+    ".google.protobuf.Timestamp"`.
+    """
+
     title: str = betterproto.string_field(5)
-    # A short description of the schema.
+    """The title of the schema."""
+
     description: str = betterproto.string_field(6)
+    """A short description of the schema."""
+
     default: str = betterproto.string_field(7)
     read_only: bool = betterproto.bool_field(8)
-    # A free-form property to include a JSON example of this field. This is
-    # copied verbatim to the output swagger.json. Quotes must be escaped. This
-    # property is the same for 2.0 and 3.0.0 https://github.com/OAI/OpenAPI-
-    # Specification/blob/3.0.0/versions/3.0.0.md#schemaObject
-    # https://github.com/OAI/OpenAPI-
-    # Specification/blob/3.0.0/versions/2.0.md#schemaObject
     example: str = betterproto.string_field(9)
+    """
+    A free-form property to include a JSON example of this field. This is
+    copied verbatim to the output swagger.json. Quotes must be escaped. This
+    property is the same for 2.0 and 3.0.0 https://github.com/OAI/OpenAPI-
+    Specification/blob/3.0.0/versions/3.0.0.md#schemaObject
+    https://github.com/OAI/OpenAPI-
+    Specification/blob/3.0.0/versions/2.0.md#schemaObject
+    """
+
     multiple_of: float = betterproto.double_field(10)
-    # Maximum represents an inclusive upper limit for a numeric instance. The
-    # value of MUST be a number,
     maximum: float = betterproto.double_field(11)
+    """
+    Maximum represents an inclusive upper limit for a numeric instance. The
+    value of MUST be a number,
+    """
+
     exclusive_maximum: bool = betterproto.bool_field(12)
-    # minimum represents an inclusive lower limit for a numeric instance. The
-    # value of MUST be a number,
     minimum: float = betterproto.double_field(13)
+    """
+    minimum represents an inclusive lower limit for a numeric instance. The
+    value of MUST be a number,
+    """
+
     exclusive_minimum: bool = betterproto.bool_field(14)
     max_length: int = betterproto.uint64_field(15)
     min_length: int = betterproto.uint64_field(16)
     pattern: str = betterproto.string_field(17)
     max_items: int = betterproto.uint64_field(20)
     min_items: int = betterproto.uint64_field(21)
     unique_items: bool = betterproto.bool_field(22)
     max_properties: int = betterproto.uint64_field(24)
     min_properties: int = betterproto.uint64_field(25)
     required: List[str] = betterproto.string_field(26)
-    # Items in 'array' must be unique.
     array: List[str] = betterproto.string_field(34)
+    """Items in 'array' must be unique."""
+
     type: List["JsonSchemaJsonSchemaSimpleTypes"] = betterproto.enum_field(35)
-    # `Format`
     format: str = betterproto.string_field(36)
-    # Items in `enum` must be unique https://tools.ietf.org/html/draft-fge-json-
-    # schema-validation-00#section-5.5.1
+    """`Format`"""
+
     enum: List[str] = betterproto.string_field(46)
-    # Additional field level properties used when generating the OpenAPI v2 file.
+    """
+    Items in `enum` must be unique https://tools.ietf.org/html/draft-fge-json-
+    schema-validation-00#section-5.5.1
+    """
+
     field_configuration: "JsonSchemaFieldConfiguration" = betterproto.message_field(
         1001
     )
+    """
+    Additional field level properties used when generating the OpenAPI v2 file.
+    """
+
     extensions: Dict[
         str, "betterproto_lib_google_protobuf.Value"
     ] = betterproto.map_field(48, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE)
+    """
+    Custom properties that start with "x-" such as "x-foo" used to describe
+    extra functionality that is not covered by the standard OpenAPI
+    Specification. See: https://swagger.io/docs/specification/2-0/swagger-
+    extensions/
+    """
 
 
 @dataclass(eq=False, repr=False)
 class JsonSchemaFieldConfiguration(betterproto.Message):
     """
     'FieldConfiguration' provides additional field level properties used when
     generating the OpenAPI v2 file. These properties are not defined by
     OpenAPIv2, but they are used to control the generation.
     """
 
-    # Alternative parameter name when used as path parameter. If set, this will
-    # be used as the complete parameter name when this field is used as a path
-    # parameter. Use this to avoid having auto generated path parameter names for
-    # overlapping paths.
     path_param_name: str = betterproto.string_field(47)
+    """
+    Alternative parameter name when used as path parameter. If set, this will
+    be used as the complete parameter name when this field is used as a path
+    parameter. Use this to avoid having auto generated path parameter names for
+    overlapping paths.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class Tag(betterproto.Message):
     """
     `Tag` is a representation of OpenAPI v2 specification's Tag object. See:
     https://github.com/OAI/OpenAPI-
     Specification/blob/3.0.0/versions/2.0.md#tagObject
     """
 
-    # A short description for the tag. GFM syntax can be used for rich text
-    # representation.
+    name: str = betterproto.string_field(1)
+    """
+    The name of the tag. Use it to allow override of the name of a global Tag
+    object, then use that name to reference the tag throughout the OpenAPI
+    file.
+    """
+
     description: str = betterproto.string_field(2)
-    # Additional external documentation for this tag.
+    """
+    A short description for the tag. GFM syntax can be used for rich text
+    representation.
+    """
+
     external_docs: "ExternalDocumentation" = betterproto.message_field(3)
+    """Additional external documentation for this tag."""
+
+    extensions: Dict[
+        str, "betterproto_lib_google_protobuf.Value"
+    ] = betterproto.map_field(4, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE)
+    """
+    Custom properties that start with "x-" such as "x-foo" used to describe
+    extra functionality that is not covered by the standard OpenAPI
+    Specification. See: https://swagger.io/docs/specification/2-0/swagger-
+    extensions/
+    """
 
 
 @dataclass(eq=False, repr=False)
 class SecurityDefinitions(betterproto.Message):
     """
     `SecurityDefinitions` is a representation of OpenAPI v2 specification's
     Security Definitions object. See: https://github.com/OAI/OpenAPI-
     Specification/blob/3.0.0/versions/2.0.md#securityDefinitionsObject A
     declaration of the security schemes available to be used in the
     specification. This does not enforce the security schemes on the operations
     and only serves to provide the relevant details for each scheme.
     """
 
-    # A single security scheme definition, mapping a "name" to the scheme it
-    # defines.
     security: Dict[str, "SecurityScheme"] = betterproto.map_field(
         1, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
     )
+    """
+    A single security scheme definition, mapping a "name" to the scheme it
+    defines.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class SecurityScheme(betterproto.Message):
     """
     `SecurityScheme` is a representation of OpenAPI v2 specification's Security
     Scheme object. See: https://github.com/OAI/OpenAPI-
     Specification/blob/3.0.0/versions/2.0.md#securitySchemeObject Allows the
     definition of a security scheme that can be used by the operations.
     Supported schemes are basic authentication, an API key (either as a header
     or as a query parameter) and OAuth2's common flows (implicit, password,
     application and access code).
     """
 
-    # The type of the security scheme. Valid values are "basic", "apiKey" or
-    # "oauth2".
     type: "SecuritySchemeType" = betterproto.enum_field(1)
-    # A short description for security scheme.
+    """
+    The type of the security scheme. Valid values are "basic", "apiKey" or
+    "oauth2".
+    """
+
     description: str = betterproto.string_field(2)
-    # The name of the header or query parameter to be used. Valid for apiKey.
+    """A short description for security scheme."""
+
     name: str = betterproto.string_field(3)
-    # The location of the API key. Valid values are "query" or "header". Valid
-    # for apiKey.
+    """
+    The name of the header or query parameter to be used. Valid for apiKey.
+    """
+
     in_: "SecuritySchemeIn" = betterproto.enum_field(4)
-    # The flow used by the OAuth2 security scheme. Valid values are "implicit",
-    # "password", "application" or "accessCode". Valid for oauth2.
+    """
+    The location of the API key. Valid values are "query" or "header". Valid
+    for apiKey.
+    """
+
     flow: "SecuritySchemeFlow" = betterproto.enum_field(5)
-    # The authorization URL to be used for this flow. This SHOULD be in the form
-    # of a URL. Valid for oauth2/implicit and oauth2/accessCode.
+    """
+    The flow used by the OAuth2 security scheme. Valid values are "implicit",
+    "password", "application" or "accessCode". Valid for oauth2.
+    """
+
     authorization_url: str = betterproto.string_field(6)
-    # The token URL to be used for this flow. This SHOULD be in the form of a
-    # URL. Valid for oauth2/password, oauth2/application and oauth2/accessCode.
+    """
+    The authorization URL to be used for this flow. This SHOULD be in the form
+    of a URL. Valid for oauth2/implicit and oauth2/accessCode.
+    """
+
     token_url: str = betterproto.string_field(7)
-    # The available scopes for the OAuth2 security scheme. Valid for oauth2.
+    """
+    The token URL to be used for this flow. This SHOULD be in the form of a
+    URL. Valid for oauth2/password, oauth2/application and oauth2/accessCode.
+    """
+
     scopes: "Scopes" = betterproto.message_field(8)
+    """
+    The available scopes for the OAuth2 security scheme. Valid for oauth2.
+    """
+
     extensions: Dict[
         str, "betterproto_lib_google_protobuf.Value"
     ] = betterproto.map_field(9, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE)
+    """
+    Custom properties that start with "x-" such as "x-foo" used to describe
+    extra functionality that is not covered by the standard OpenAPI
+    Specification. See: https://swagger.io/docs/specification/2-0/swagger-
+    extensions/
+    """
 
 
 @dataclass(eq=False, repr=False)
 class SecurityRequirement(betterproto.Message):
     """
     `SecurityRequirement` is a representation of OpenAPI v2 specification's
     Security Requirement object. See: https://github.com/OAI/OpenAPI-
@@ -526,21 +836,23 @@
     the required security schemes to execute this operation. The object can
     have multiple security schemes declared in it which are all required (that
     is, there is a logical AND between the schemes). The name used for each
     property MUST correspond to a security scheme declared in the Security
     Definitions.
     """
 
-    # Each name must correspond to a security scheme which is declared in the
-    # Security Definitions. If the security scheme is of type "oauth2", then the
-    # value is a list of scope names required for the execution. For other
-    # security scheme types, the array MUST be empty.
     security_requirement: Dict[
         str, "SecurityRequirementSecurityRequirementValue"
     ] = betterproto.map_field(1, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE)
+    """
+    Each name must correspond to a security scheme which is declared in the
+    Security Definitions. If the security scheme is of type "oauth2", then the
+    value is a list of scope names required for the execution. For other
+    security scheme types, the array MUST be empty.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class SecurityRequirementSecurityRequirementValue(betterproto.Message):
     """
     If the security scheme is of type "oauth2", then the value is a list of
     scope names required for the execution. For other security scheme types,
@@ -555,15 +867,14 @@
     """
     `Scopes` is a representation of OpenAPI v2 specification's Scopes object.
     See: https://github.com/OAI/OpenAPI-
     Specification/blob/3.0.0/versions/2.0.md#scopesObject Lists the available
     scopes for an OAuth2 security scheme.
     """
 
-    # Maps between a name of a scope to a short description of it (as the value
-    # of the property).
     scope: Dict[str, str] = betterproto.map_field(
         1, betterproto.TYPE_STRING, betterproto.TYPE_STRING
     )
-
-
-import betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
+    """
+    Maps between a name of a scope to a short description of it (as the value
+    of the property).
+    """
```

### Comparing `wechaty-grpc-1.5.dev2/src/wechaty_grpc/wechaty/puppet/__init__.py` & `wechaty-grpc-1.5.dev4/src/wechaty_grpc/wechaty/puppet/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: wechaty/deprecated/file-box.proto, wechaty/puppet/base.proto, wechaty/puppet/contact.proto, wechaty/puppet/download-upload.proto, wechaty/puppet/event.proto, wechaty/puppet/friendship.proto, wechaty/puppet/image.proto, wechaty/puppet/location.proto, wechaty/puppet/message.proto, wechaty/puppet/mini-program.proto, wechaty/puppet/referrer.proto, wechaty/puppet/room-invitation.proto, wechaty/puppet/room-member.proto, wechaty/puppet/room.proto, wechaty/puppet/tag.proto, wechaty/puppet/url-link.proto
+# sources: wechaty/deprecated/file-box.proto, wechaty/puppet/base.proto, wechaty/puppet/contact.proto, wechaty/puppet/conversation.proto, wechaty/puppet/download-upload.proto, wechaty/puppet/event.proto, wechaty/puppet/friendship.proto, wechaty/puppet/image.proto, wechaty/puppet/location.proto, wechaty/puppet/message.proto, wechaty/puppet/mini-program.proto, wechaty/puppet/referrer.proto, wechaty/puppet/room-invitation.proto, wechaty/puppet/room-member.proto, wechaty/puppet/room.proto, wechaty/puppet/tag.proto, wechaty/puppet/url-link.proto
 # plugin: python-betterproto
+# This file has been @generated
 import warnings
 from dataclasses import dataclass
 from datetime import datetime
-from typing import List, Optional
+from typing import (
+    List,
+    Optional,
+)
 
 import betterproto
-from betterproto.grpc.grpclib_server import ServiceBase
 
 
 class ImageType(betterproto.Enum):
     IMAGE_TYPE_UNSPECIFIED = 0
     IMAGE_TYPE_THUMBNAIL = 1
     IMAGE_TYPE_HD = 2
     IMAGE_TYPE_ARTWORK = 3
@@ -53,14 +56,15 @@
     EVENT_TYPE_ROOM_TOPIC = 21
     EVENT_TYPE_SCAN = 22
     EVENT_TYPE_READY = 23
     EVENT_TYPE_RESET = 24
     EVENT_TYPE_LOGIN = 25
     EVENT_TYPE_LOGOUT = 26
     EVENT_TYPE_DIRTY = 27
+    EVENT_TYPE_ROOM_ANNOUNCE = 32
 
 
 class FriendshipType(betterproto.Enum):
     FRIENDSHIP_TYPE_UNSPECIFIED = 0
     FRIENDSHIP_TYPE_CONFIRM = 1
     FRIENDSHIP_TYPE_RECEIVE = 2
     FRIENDSHIP_TYPE_VERIFY = 3
@@ -93,20 +97,24 @@
     MESSAGE_TYPE_CHAT_HISTORY = 8
     MESSAGE_TYPE_LOCATION = 9
     MESSAGE_TYPE_MINI_PROGRAM = 10
     MESSAGE_TYPE_TRANSFER = 11
     MESSAGE_TYPE_RED_ENVELOPE = 12
     MESSAGE_TYPE_RECALLED = 13
     MESSAGE_TYPE_URL = 14
+    MESSAGE_TYPE_GROUP_NOTE = 15
+    MESSAGE_TYPE_POST = 16
+    MESSAGE_TYPE_SYSTEM = 18
 
 
 @dataclass(eq=False, repr=False)
 class FileBoxChunk(betterproto.Message):
-    # oneof payload {
     data: Optional[bytes] = betterproto.bytes_field(1, optional=True, group="_data")
+    """oneof payload {"""
+
     name: Optional[str] = betterproto.string_field(2, optional=True, group="_name")
 
 
 @dataclass(eq=False, repr=False)
 class MessageImageStreamRequest(betterproto.Message):
     id: str = betterproto.string_field(1)
     type: "ImageType" = betterproto.enum_field(2)
@@ -125,36 +133,40 @@
 @dataclass(eq=False, repr=False)
 class MessageFileStreamResponse(betterproto.Message):
     file_box_chunk: "FileBoxChunk" = betterproto.message_field(1)
 
 
 @dataclass(eq=False, repr=False)
 class MessageSendFileStreamRequest(betterproto.Message):
-    # oneof payload {
     conversation_id: Optional[str] = betterproto.string_field(
         1, optional=True, group="_conversation_id"
     )
+    """oneof payload {"""
+
     file_box_chunk: Optional["FileBoxChunk"] = betterproto.message_field(
         2, optional=True, group="_file_box_chunk"
     )
 
 
 @dataclass(eq=False, repr=False)
 class MessageSendFileStreamResponse(betterproto.Message):
-    # * @deprecated:  Huan(202109): Wrapper types must not be used going forward.
-    # https://cloud.google.com/apis/design/design_patterns#optional_primitive_fie
-    # lds
     id_string_value_deprecated: Optional[str] = betterproto.message_field(
         1, wraps=betterproto.TYPE_STRING
     )
+    """
+    * @deprecated:  Huan(202109): Wrapper types must not be used going forward.
+    https://cloud.google.com/apis/design/design_patterns#optional_primitive_fie
+    lds
+    """
+
     id: str = betterproto.string_field(2)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.id_string_value_deprecated:
+        if self.is_set("id_string_value_deprecated"):
             warnings.warn(
                 "MessageSendFileStreamResponse.id_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -243,22 +255,25 @@
     address: str = betterproto.string_field(6)
     alias: str = betterproto.string_field(7)
     city: str = betterproto.string_field(8)
     friend: bool = betterproto.bool_field(9)
     province: str = betterproto.string_field(10)
     signature: str = betterproto.string_field(11)
     star: bool = betterproto.bool_field(12)
-    # * Huan(202203): in gRPC, we can freely rename the field name as long as the
-    # number keep consistent.  so we can just rename `weixin` to `handle` here.
-    # (Huan(20220329): use `weixin` for now, until we upgrade to v2.0  the
-    # `wechaty-grpc@1.0.0` will use the latest v1.x automatically when running
-    # `npm install`    which will causing a breaking change.  @link
-    # https://github.com/wechaty/getting-started/issues/254 TODO: rename `weixin`
-    # to `handle` in v2.0.0
     weixin: str = betterproto.string_field(13)
+    """
+    * Huan(202203): in gRPC, we can freely rename the field name as long as the
+    number keep consistent.  so we can just rename `weixin` to `handle` here.
+    (Huan(20220329): use `weixin` for now, until we upgrade to v2.0  the
+    `wechaty-grpc@1.0.0` will use the latest v1.x automatically when running
+    `npm install`    which will causing a breaking change.  @link
+    https://github.com/wechaty/getting-started/issues/254 TODO: rename `weixin`
+    to `handle` in v2.0.0
+    """
+
     corporation: str = betterproto.string_field(14)
     title: str = betterproto.string_field(15)
     description: str = betterproto.string_field(16)
     coworker: bool = betterproto.bool_field(17)
     phones: List[str] = betterproto.string_field(18)
 
 
@@ -291,23 +306,24 @@
 class ContactSelfSignatureResponse(betterproto.Message):
     pass
 
 
 @dataclass(eq=False, repr=False)
 class ContactAliasRequest(betterproto.Message):
     id: str = betterproto.string_field(1)
-    # nullable
     alias_string_value_deprecated: Optional[str] = betterproto.message_field(
         2, wraps=betterproto.TYPE_STRING
     )
+    """nullable"""
+
     alias: Optional[str] = betterproto.string_field(3, optional=True, group="_alias")
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.alias_string_value_deprecated:
+        if self.is_set("alias_string_value_deprecated"):
             warnings.warn(
                 "ContactAliasRequest.alias_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -315,15 +331,15 @@
     alias_string_value_deprecated: Optional[str] = betterproto.message_field(
         1, wraps=betterproto.TYPE_STRING
     )
     alias: str = betterproto.string_field(2)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.alias_string_value_deprecated:
+        if self.is_set("alias_string_value_deprecated"):
             warnings.warn(
                 "ContactAliasResponse.alias_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -334,15 +350,15 @@
     )
     file_box: Optional[str] = betterproto.string_field(
         3, optional=True, group="_file_box"
     )
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.filebox_string_value_deprecated:
+        if self.is_set("filebox_string_value_deprecated"):
             warnings.warn(
                 "ContactAvatarRequest.filebox_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -350,15 +366,15 @@
     filebox_string_value_deprecated: Optional[str] = betterproto.message_field(
         1, wraps=betterproto.TYPE_STRING
     )
     file_box: str = betterproto.string_field(2)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.filebox_string_value_deprecated:
+        if self.is_set("filebox_string_value_deprecated"):
             warnings.warn(
                 "ContactAvatarResponse.filebox_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -378,15 +394,15 @@
     corporation_remark_string_value_deprecated: Optional[
         str
     ] = betterproto.message_field(2, wraps=betterproto.TYPE_STRING)
     corporation_remark: str = betterproto.string_field(3)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.corporation_remark_string_value_deprecated:
+        if self.is_set("corporation_remark_string_value_deprecated"):
             warnings.warn(
                 "ContactCorporationRemarkRequest.corporation_remark_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -400,15 +416,15 @@
     description_string_value_deprecated: Optional[str] = betterproto.message_field(
         2, wraps=betterproto.TYPE_STRING
     )
     description: str = betterproto.string_field(3)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.description_string_value_deprecated:
+        if self.is_set("description_string_value_deprecated"):
             warnings.warn(
                 "ContactDescriptionRequest.description_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -440,16 +456,16 @@
 class EventRequest(betterproto.Message):
     pass
 
 
 @dataclass(eq=False, repr=False)
 class EventResponse(betterproto.Message):
     type: "EventType" = betterproto.enum_field(1)
-    # TODO: Huan(202002) consider to use a PB Map?
     payload: str = betterproto.string_field(2)
+    """TODO: Huan(202002) consider to use a PB Map?"""
 
 
 @dataclass(eq=False, repr=False)
 class Referrer(betterproto.Message):
     """
     * "Referrer" and "Referral" refers to different things. "Referrer" is
     something or somebody who refers. "Referral" is the act of referring.  -
@@ -460,24 +476,27 @@
     contact_id: str = betterproto.string_field(1)
     room_id: str = betterproto.string_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class FriendshipPayloadRequest(betterproto.Message):
     id: str = betterproto.string_field(1)
-    # * Huan(202003):  What's the reason we need belowing payload?  We should
-    # remove it if possible.
     payload_string_value_deprecated: Optional[str] = betterproto.message_field(
         2, wraps=betterproto.TYPE_STRING
     )
+    """
+    * Huan(202003):  What's the reason we need belowing payload?  We should
+    remove it if possible.
+    """
+
     payload: str = betterproto.string_field(3)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.payload_string_value_deprecated:
+        if self.is_set("payload_string_value_deprecated"):
             warnings.warn(
                 "FriendshipPayloadRequest.payload_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -494,23 +513,24 @@
 @dataclass(eq=False, repr=False)
 class FriendshipSearchPhoneRequest(betterproto.Message):
     phone: str = betterproto.string_field(1)
 
 
 @dataclass(eq=False, repr=False)
 class FriendshipSearchPhoneResponse(betterproto.Message):
-    # nullable
     contact_id_string_value_deprecated: Optional[str] = betterproto.message_field(
         1, wraps=betterproto.TYPE_STRING
     )
+    """nullable"""
+
     contact_id: str = betterproto.string_field(2)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.contact_id_string_value_deprecated:
+        if self.is_set("contact_id_string_value_deprecated"):
             warnings.warn(
                 "FriendshipSearchPhoneResponse.contact_id_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -519,35 +539,38 @@
     * Huan(202003): we just rename the payload message because gRPC only care
     about the message structure  (and as long as we keep consistent with the
     old structure).  @link https://github.com/wechaty/grpc/pull/173 Rename:  1.
     `FriendshipSearchWeixinRequest`    -> `FriendshipSearchHandleRequest`  2.
     `FriendshipSearchWeixinReqsponse`  -> `FriendshipSearchHandleResponse`
     """
 
-    # * Huan(202203): in gRPC, we can freely rename the field name as long as the
-    # number keep consistent.  so we can just rename `weixin` to `handle` here.
-    # (Huan(20220329): use `weixin` for now, until we upgrade to v2.0  the
-    # `wechaty-grpc@1.0.0` will use the latest v1.x automatically when running
-    # `npm install`    which will causing a breaking change.  @link
-    # https://github.com/wechaty/getting-started/issues/254 TODO: rename `weixin`
-    # to `handle` in v2.0.0
     weixin: str = betterproto.string_field(1)
+    """
+    * Huan(202203): in gRPC, we can freely rename the field name as long as the
+    number keep consistent.  so we can just rename `weixin` to `handle` here.
+    (Huan(20220329): use `weixin` for now, until we upgrade to v2.0  the
+    `wechaty-grpc@1.0.0` will use the latest v1.x automatically when running
+    `npm install`    which will causing a breaking change.  @link
+    https://github.com/wechaty/getting-started/issues/254 TODO: rename `weixin`
+    to `handle` in v2.0.0
+    """
 
 
 @dataclass(eq=False, repr=False)
 class FriendshipSearchHandleResponse(betterproto.Message):
-    # nullable
     contact_id_string_value_deprecated: Optional[str] = betterproto.message_field(
         1, wraps=betterproto.TYPE_STRING
     )
+    """nullable"""
+
     contact_id: str = betterproto.string_field(2)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.contact_id_string_value_deprecated:
+        if self.is_set("contact_id_string_value_deprecated"):
             warnings.warn(
                 "FriendshipSearchHandleResponse.contact_id_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -560,20 +583,20 @@
     source_contact_id_string_value_deprecated: Optional[
         str
     ] = betterproto.message_field(4, wraps=betterproto.TYPE_STRING)
     referrer: "Referrer" = betterproto.message_field(5)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.source_room_id_string_value_deprecated:
+        if self.is_set("source_room_id_string_value_deprecated"):
             warnings.warn(
                 "FriendshipAddRequest.source_room_id_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
-        if self.source_contact_id_string_value_deprecated:
+        if self.is_set("source_contact_id_string_value_deprecated"):
             warnings.warn(
                 "FriendshipAddRequest.source_contact_id_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -627,27 +650,30 @@
 
 
 @dataclass(eq=False, repr=False)
 class MessagePayloadResponse(betterproto.Message):
     id: str = betterproto.string_field(1)
     filename: str = betterproto.string_field(2)
     text: str = betterproto.string_field(3)
-    # * @deprecated will be removed after Dec 31, 2022  Huan(202109): use
-    # receive_time(10) instead
     timestamp_deprecated: int = betterproto.uint64_field(4)
+    """
+    * @deprecated will be removed after Dec 31, 2022  Huan(202109): use
+    receive_time(10) instead
+    """
+
     type: "MessageType" = betterproto.enum_field(5)
     talker_id: str = betterproto.string_field(6)
     room_id: str = betterproto.string_field(7)
     listener_id: str = betterproto.string_field(8)
     mention_ids: List[str] = betterproto.string_field(9)
     receive_time: datetime = betterproto.message_field(10)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.timestamp_deprecated:
+        if self.is_set("timestamp_deprecated"):
             warnings.warn(
                 "MessagePayloadResponse.timestamp_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -684,192 +710,221 @@
 @dataclass(eq=False, repr=False)
 class MessageMiniProgramRequest(betterproto.Message):
     id: str = betterproto.string_field(1)
 
 
 @dataclass(eq=False, repr=False)
 class MessageMiniProgramResponse(betterproto.Message):
-    # * Huan(202110): We should use payload instead of JSON.stringify string  The
-    # compatible code will be removed after Dec 31, 2022
     mini_program_deprecated: str = betterproto.string_field(1)
+    """
+    * Huan(202110): We should use payload instead of JSON.stringify string  The
+    compatible code will be removed after Dec 31, 2022
+    """
+
     mini_program: "MiniProgramPayload" = betterproto.message_field(2)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.mini_program_deprecated:
+        if self.is_set("mini_program_deprecated"):
             warnings.warn(
                 "MessageMiniProgramResponse.mini_program_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
 class MessageUrlRequest(betterproto.Message):
     id: str = betterproto.string_field(1)
 
 
 @dataclass(eq=False, repr=False)
 class MessageUrlResponse(betterproto.Message):
-    # * Huan(202110): We should use payload instead of JSON.stringify string  The
-    # compatible code will be removed after Dec 31, 2022
     url_link_deprecated: str = betterproto.string_field(1)
+    """
+    * Huan(202110): We should use payload instead of JSON.stringify string  The
+    compatible code will be removed after Dec 31, 2022
+    """
+
     url_link: "UrlLinkPayload" = betterproto.message_field(2)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.url_link_deprecated:
+        if self.is_set("url_link_deprecated"):
             warnings.warn(
                 "MessageUrlResponse.url_link_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
 class MessageSendContactRequest(betterproto.Message):
     conversation_id: str = betterproto.string_field(1)
     contact_id: str = betterproto.string_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class MessageSendContactResponse(betterproto.Message):
-    # * @deprecated:  Huan(202109): Wrapper types must not be used going forward.
-    # https://cloud.google.com/apis/design/design_patterns#optional_primitive_fie
-    # lds
     id_string_value_deprecated: Optional[str] = betterproto.message_field(
         1, wraps=betterproto.TYPE_STRING
     )
+    """
+    * @deprecated:  Huan(202109): Wrapper types must not be used going forward.
+    https://cloud.google.com/apis/design/design_patterns#optional_primitive_fie
+    lds
+    """
+
     id: str = betterproto.string_field(2)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.id_string_value_deprecated:
+        if self.is_set("id_string_value_deprecated"):
             warnings.warn(
                 "MessageSendContactResponse.id_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
 class MessageSendFileRequest(betterproto.Message):
     conversation_id: str = betterproto.string_field(1)
     file_box: str = betterproto.string_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class MessageSendFileResponse(betterproto.Message):
-    # * @deprecated:  Huan(202109): Wrapper types must not be used going forward.
-    # https://cloud.google.com/apis/design/design_patterns#optional_primitive_fie
-    # lds
     id_string_value_deprecated: Optional[str] = betterproto.message_field(
         1, wraps=betterproto.TYPE_STRING
     )
+    """
+    * @deprecated:  Huan(202109): Wrapper types must not be used going forward.
+    https://cloud.google.com/apis/design/design_patterns#optional_primitive_fie
+    lds
+    """
+
     id: str = betterproto.string_field(2)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.id_string_value_deprecated:
+        if self.is_set("id_string_value_deprecated"):
             warnings.warn(
                 "MessageSendFileResponse.id_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
 class MessageSendTextRequest(betterproto.Message):
     conversation_id: str = betterproto.string_field(1)
     text: str = betterproto.string_field(2)
-    # Huan(202011) FIXME: Issue #99 https://github.com/wechaty/grpc/issues/99
     mentional_ids: List[str] = betterproto.string_field(3)
+    """
+    Huan(202011) FIXME: Issue #99 https://github.com/wechaty/grpc/issues/99
+    """
 
 
 @dataclass(eq=False, repr=False)
 class MessageSendTextResponse(betterproto.Message):
-    # * @deprecated:  Huan(202109): Wrapper types must not be used going forward.
-    # https://cloud.google.com/apis/design/design_patterns#optional_primitive_fie
-    # lds
     id_string_value_deprecated: Optional[str] = betterproto.message_field(
         1, wraps=betterproto.TYPE_STRING
     )
+    """
+    * @deprecated:  Huan(202109): Wrapper types must not be used going forward.
+    https://cloud.google.com/apis/design/design_patterns#optional_primitive_fie
+    lds
+    """
+
     id: str = betterproto.string_field(2)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.id_string_value_deprecated:
+        if self.is_set("id_string_value_deprecated"):
             warnings.warn(
                 "MessageSendTextResponse.id_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
 class MessageSendMiniProgramRequest(betterproto.Message):
     conversation_id: str = betterproto.string_field(1)
-    # * Huan(202110): We should use payload instead of JSON.stringify string  The
-    # compatible code will be removed after Dec 31, 2022
     mini_program_deprecated: str = betterproto.string_field(2)
+    """
+    * Huan(202110): We should use payload instead of JSON.stringify string  The
+    compatible code will be removed after Dec 31, 2022
+    """
+
     mini_program: "MiniProgramPayload" = betterproto.message_field(3)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.mini_program_deprecated:
+        if self.is_set("mini_program_deprecated"):
             warnings.warn(
                 "MessageSendMiniProgramRequest.mini_program_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
 class MessageSendMiniProgramResponse(betterproto.Message):
-    # * @deprecated:  Huan(202109): Wrapper types must not be used going forward.
-    # https://cloud.google.com/apis/design/design_patterns#optional_primitive_fie
-    # lds
     id_string_value_deprecated: Optional[str] = betterproto.message_field(
         1, wraps=betterproto.TYPE_STRING
     )
+    """
+    * @deprecated:  Huan(202109): Wrapper types must not be used going forward.
+    https://cloud.google.com/apis/design/design_patterns#optional_primitive_fie
+    lds
+    """
+
     id: str = betterproto.string_field(2)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.id_string_value_deprecated:
+        if self.is_set("id_string_value_deprecated"):
             warnings.warn(
                 "MessageSendMiniProgramResponse.id_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
 class MessageSendUrlRequest(betterproto.Message):
     conversation_id: str = betterproto.string_field(1)
-    # * Huan(202110): We should use payload instead of JSON.stringify string  The
-    # compatible code will be removed after Dec 31, 2022
     url_link_deprecated: str = betterproto.string_field(2)
+    """
+    * Huan(202110): We should use payload instead of JSON.stringify string  The
+    compatible code will be removed after Dec 31, 2022
+    """
+
     url_link: "UrlLinkPayload" = betterproto.message_field(3)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.url_link_deprecated:
+        if self.is_set("url_link_deprecated"):
             warnings.warn(
                 "MessageSendUrlRequest.url_link_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
 class MessageSendUrlResponse(betterproto.Message):
-    # * @deprecated:  Huan(202109): Wrapper types must not be used going forward.
-    # https://cloud.google.com/apis/design/design_patterns#optional_primitive_fie
-    # lds
     id_string_value_deprecated: Optional[str] = betterproto.message_field(
         1, wraps=betterproto.TYPE_STRING
     )
+    """
+    * @deprecated:  Huan(202109): Wrapper types must not be used going forward.
+    https://cloud.google.com/apis/design/design_patterns#optional_primitive_fie
+    lds
+    """
+
     id: str = betterproto.string_field(2)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.id_string_value_deprecated:
+        if self.is_set("id_string_value_deprecated"):
             warnings.warn(
                 "MessageSendUrlResponse.id_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -886,25 +941,28 @@
 class MessageForwardRequest(betterproto.Message):
     message_id: str = betterproto.string_field(1)
     conversation_id: str = betterproto.string_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class MessageForwardResponse(betterproto.Message):
-    # * @deprecated: use payload instead.  Huan(202109): Wrapper types must not
-    # be used going forward.    https://cloud.google.com/apis/design/design_patte
-    # rns#optional_primitive_fields
     id_string_value_deprecated: Optional[str] = betterproto.message_field(
         1, wraps=betterproto.TYPE_STRING
     )
+    """
+    * @deprecated: use payload instead.  Huan(202109): Wrapper types must not
+    be used going forward.    https://cloud.google.com/apis/design/design_patte
+    rns#optional_primitive_fields
+    """
+
     id: str = betterproto.string_field(2)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.id_string_value_deprecated:
+        if self.is_set("id_string_value_deprecated"):
             warnings.warn(
                 "MessageForwardResponse.id_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -921,63 +979,71 @@
 class MessageSendLocationRequest(betterproto.Message):
     conversation_id: str = betterproto.string_field(1)
     location: "LocationPayload" = betterproto.message_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class MessageSendLocationResponse(betterproto.Message):
-    # * Huan(202110): we will not use wrappers any more by following the Google
-    # Style Guide:  If not using optional would add complexity or ambiguity, then
-    # use optional primitive fields,  Wrapper types must not be used going
-    # forward.  — Optional Primitive Fields
-    # (https://cloud.google.com/apis/design/design_patterns.md#optional-
-    # primitive-fields)
     id: str = betterproto.string_field(1)
+    """
+    * Huan(202110): we will not use wrappers any more by following the Google
+    Style Guide:  If not using optional would add complexity or ambiguity, then
+    use optional primitive fields,  Wrapper types must not be used going
+    forward.  — Optional Primitive Fields
+    (https://cloud.google.com/apis/design/design_patterns.md#optional-
+    primitive-fields)
+    """
 
 
 @dataclass(eq=False, repr=False)
 class RoomInvitationPayloadRequest(betterproto.Message):
     id: str = betterproto.string_field(1)
-    # * Huan(202002): `payload` should be removed.  The puppet server should take
-    # the responsibilities  for storing the unaccepted friend-request payload.
-    # @deprecated: use payload instead.  Huan(202109): Wrapper types must not be
-    # used going forward.    https://cloud.google.com/apis/design/design_patterns
-    # #optional_primitive_fields
     payload_string_value_deprecated: Optional[str] = betterproto.message_field(
         2, wraps=betterproto.TYPE_STRING
     )
+    """
+    * Huan(202002): `payload` should be removed.  The puppet server should take
+    the responsibilities  for storing the unaccepted friend-request payload.
+    @deprecated: use payload instead.  Huan(202109): Wrapper types must not be
+    used going forward.    https://cloud.google.com/apis/design/design_patterns
+    #optional_primitive_fields
+    """
+
     payload: str = betterproto.string_field(3)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.payload_string_value_deprecated:
+        if self.is_set("payload_string_value_deprecated"):
             warnings.warn(
                 "RoomInvitationPayloadRequest.payload_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
 class RoomInvitationPayloadResponse(betterproto.Message):
     id: str = betterproto.string_field(1)
     inviter_id: str = betterproto.string_field(2)
     topic: str = betterproto.string_field(3)
     member_count: int = betterproto.int32_field(4)
     member_ids: List[str] = betterproto.string_field(5)
-    # * @deprecated will be removed after Dec 31, 2022  Huan(202109): use
-    # receive_time(10) instead
     timestamp_uint64_deprecated: int = betterproto.uint64_field(6)
+    """
+    * @deprecated will be removed after Dec 31, 2022  Huan(202109): use
+    receive_time(10) instead
+    """
+
     avatar: str = betterproto.string_field(7)
     invitation: str = betterproto.string_field(8)
     receiver_id: str = betterproto.string_field(9)
     receive_time: datetime = betterproto.message_field(10)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.timestamp_uint64_deprecated:
+        if self.is_set("timestamp_uint64_deprecated"):
             warnings.warn(
                 "RoomInvitationPayloadResponse.timestamp_uint64_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -1042,14 +1108,20 @@
 
 
 @dataclass(eq=False, repr=False)
 class RoomAddRequest(betterproto.Message):
     id: str = betterproto.string_field(1)
     contact_id: str = betterproto.string_field(2)
     invite_only: bool = betterproto.bool_field(3)
+    contact_ids: List[str] = betterproto.string_field(4)
+
+    def __post_init__(self) -> None:
+        super().__post_init__()
+        if self.is_set("contact_id"):
+            warnings.warn("RoomAddRequest.contact_id is deprecated", DeprecationWarning)
 
 
 @dataclass(eq=False, repr=False)
 class RoomAddResponse(betterproto.Message):
     pass
 
 
@@ -1074,14 +1146,20 @@
     id: str = betterproto.string_field(1)
 
 
 @dataclass(eq=False, repr=False)
 class RoomDelRequest(betterproto.Message):
     id: str = betterproto.string_field(1)
     contact_id: str = betterproto.string_field(2)
+    contact_ids: List[str] = betterproto.string_field(3)
+
+    def __post_init__(self) -> None:
+        super().__post_init__()
+        if self.is_set("contact_id"):
+            warnings.warn("RoomDelRequest.contact_id is deprecated", DeprecationWarning)
 
 
 @dataclass(eq=False, repr=False)
 class RoomDelResponse(betterproto.Message):
     pass
 
 
@@ -1101,15 +1179,15 @@
     topic_string_value_deprecated: Optional[str] = betterproto.message_field(
         2, wraps=betterproto.TYPE_STRING
     )
     topic: Optional[str] = betterproto.string_field(3, optional=True, group="_topic")
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.topic_string_value_deprecated:
+        if self.is_set("topic_string_value_deprecated"):
             warnings.warn(
                 "RoomTopicRequest.topic_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -1117,15 +1195,15 @@
     topic_string_value_deprecated: Optional[str] = betterproto.message_field(
         1, wraps=betterproto.TYPE_STRING
     )
     topic: str = betterproto.string_field(2)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.topic_string_value_deprecated:
+        if self.is_set("topic_string_value_deprecated"):
             warnings.warn(
                 "RoomTopicResponse.topic_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -1144,15 +1222,15 @@
     text_string_value_deprecated: Optional[str] = betterproto.message_field(
         2, wraps=betterproto.TYPE_STRING
     )
     text: Optional[str] = betterproto.string_field(3, optional=True, group="_text")
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.text_string_value_deprecated:
+        if self.is_set("text_string_value_deprecated"):
             warnings.warn(
                 "RoomAnnounceRequest.text_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -1160,15 +1238,15 @@
     text_string_value_deprecated: Optional[str] = betterproto.message_field(
         1, wraps=betterproto.TYPE_STRING
     )
     text: str = betterproto.string_field(2)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.text_string_value_deprecated:
+        if self.is_set("text_string_value_deprecated"):
             warnings.warn(
                 "RoomAnnounceResponse.text_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
@@ -1201,27 +1279,41 @@
 @dataclass(eq=False, repr=False)
 class TagContactDeleteResponse(betterproto.Message):
     pass
 
 
 @dataclass(eq=False, repr=False)
 class TagContactListRequest(betterproto.Message):
-    # @deprecated:  Huan(202109): Wrapper types must not be used going forward.
-    # https://cloud.google.com/apis/design/design_patterns#optional_primitive_fie
-    # lds
     contact_id_string_value_deprecated: Optional[str] = betterproto.message_field(
         1, wraps=betterproto.TYPE_STRING
     )
+    """
+    @deprecated:  Huan(202109): Wrapper types must not be used going forward.
+    https://cloud.google.com/apis/design/design_patterns#optional_primitive_fie
+    lds
+    """
+
     contact_id: str = betterproto.string_field(2)
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.contact_id_string_value_deprecated:
+        if self.is_set("contact_id_string_value_deprecated"):
             warnings.warn(
                 "TagContactListRequest.contact_id_string_value_deprecated is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
 class TagContactListResponse(betterproto.Message):
     ids: List[str] = betterproto.string_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class ConversationReadRequest(betterproto.Message):
+    conversation_id: str = betterproto.string_field(1)
+    has_read: bool = betterproto.bool_field(2)
+
+
+@dataclass(eq=False, repr=False)
+class ConversationReadResponse(betterproto.Message):
+    has_read: bool = betterproto.bool_field(1)
```

### Comparing `wechaty-grpc-1.5.dev2/src/wechaty_grpc.egg-info/PKG-INFO` & `wechaty-grpc-1.5.dev4/src/wechaty_grpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wechaty-grpc
-Version: 1.5.dev2
+Version: 1.5.dev4
 Summary: Wechaty Puppet Service gRPC API
 Home-page: https://github.com/wechaty/grpc
 Author: Huan LI (李卓桓)
 Author-email: zixia@zixia.net
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
@@ -138,15 +138,15 @@
 
 **Maintainer:**
 
 - [@diaozxin007](https://github.com/diaozxin007) - Zhengxin DIAO (刁政欣)
 
 ### PHP
 
-[github.com/wechaty/php-grpc](https://github.comwechaty/php-grpc)
+[github.com/wechaty/php-grpc](https://github.com/wechaty/php-grpc)
 
 **Maintainer:**
 
 - [@zhangchunsheng](https://github.com/zhangchunsheng) - Chunsheng ZHANG (张春生)
 
 ### CSharp
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wechaty-grpc Version: 1.5.dev2 Summary: Wechaty
+Metadata-Version: 2.1 Name: wechaty-grpc Version: 1.5.dev4 Summary: Wechaty
 Puppet Service gRPC API Home-page: https://github.com/wechaty/grpc Author: Huan
 LI (æåæ¡) Author-email: zixia@zixia.net License: Apache-2.0 Platform:
 UNKNOWN Classifier: Programming Language :: Python :: 3.7 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown
                      [docs/images/wechaty-grpc-logo.svg]
                           ****** Wechaty gRPC ******
@@ -71,15 +71,15 @@
 Jingjing WU (å´äº¬äº¬) ### Go [github.com/wechaty/go-grpc](https://github.com/
 wechaty/go-grpc) **Maintainer:** - [@dchaofei](https://github.com/dchaofei) -
 Chaofei DING (ä¸è¶é£) ### Java [https://mvnrepository.com/artifact/
 io.github.wechaty/grpc](https://mvnrepository.com/artifact/io.github.wechaty/
 grpc) **Maven:** ```xml  io.github.wechaty 0.11.25 grpc  ``` **Gradle:**
 ```groovy compile 'io.github.wechaty:grpc:0.11.25' ``` **Maintainer:** -
 [@diaozxin007](https://github.com/diaozxin007) - Zhengxin DIAO (åæ¿æ¬£) ###
-PHP [github.com/wechaty/php-grpc](https://github.comwechaty/php-grpc)
+PHP [github.com/wechaty/php-grpc](https://github.com/wechaty/php-grpc)
 **Maintainer:** - [@zhangchunsheng](https://github.com/zhangchunsheng) -
 Chunsheng ZHANG (å¼ æ¥ç) ### CSharp [Wechaty.Grpc @ Nuget](https://
 www.nuget.org/packages/Wechaty.Grpc) **Maintainer:** - [@Darren](https://
 github.com/jesn) - Darren (éæ³¢) ## Development ### Debug - [GUI Client for
 GRPC Services](https://github.com/uw-labs/bloomrpc) - BloomRPC aims to give the
 simplest and efficient developer experience for exploring and querying your
 GRPC services. (Inspired by Postman and GraphQL Playground) - [A gRPC CLI
```

### Comparing `wechaty-grpc-1.5.dev2/src/wechaty_grpc.egg-info/SOURCES.txt` & `wechaty-grpc-1.5.dev4/src/wechaty_grpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

