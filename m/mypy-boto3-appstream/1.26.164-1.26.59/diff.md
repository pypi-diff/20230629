# Comparing `tmp/mypy-boto3-appstream-1.26.164.tar.gz` & `tmp/mypy-boto3-appstream-1.26.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appstream-1.26.164.tar", last modified: Thu Jun 29 20:25:42 2023, max compression
+gzip compressed data, was "mypy-boto3-appstream-1.26.59.tar", last modified: Fri Jan 27 20:32:50 2023, max compression
```

## Comparing `mypy-boto3-appstream-1.26.164.tar` & `mypy-boto3-appstream-1.26.59.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:25:42.248377 mypy-boto3-appstream-1.26.164/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-29 20:24:26.000000 mypy-boto3-appstream-1.26.164/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23433 2023-06-29 20:25:42.240377 mypy-boto3-appstream-1.26.164/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21936 2023-06-29 20:24:26.000000 mypy-boto3-appstream-1.26.164/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:25:42.240377 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-29 20:24:26.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-29 20:24:26.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-29 20:24:26.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57916 2023-06-29 20:24:27.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57822 2023-06-29 20:24:27.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-06-29 20:24:27.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-06-29 20:24:27.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-06-29 20:24:27.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-06-29 20:24:27.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:24:26.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69593 2023-06-29 20:24:29.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69496 2023-06-29 20:24:29.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 20:24:26.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-29 20:24:27.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-29 20:24:27.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:25:42.240377 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23433 2023-06-29 20:25:42.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-29 20:25:42.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:25:42.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:25:42.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-29 20:25:42.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 20:25:42.000000 mypy-boto3-appstream-1.26.164/mypy_boto3_appstream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 20:25:42.248377 mypy-boto3-appstream-1.26.164/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-29 20:24:26.000000 mypy-boto3-appstream-1.26.164/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.588096 mypy-boto3-appstream-1.26.59/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22207 2023-01-27 20:32:50.588096 mypy-boto3-appstream-1.26.59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20712 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.588096 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51155 2023-01-27 20:32:01.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51071 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13985 2023-01-27 20:32:01.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-01-27 20:32:01.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-01-27 20:32:01.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-01-27 20:32:01.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60863 2023-01-27 20:32:02.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60776 2023-01-27 20:32:02.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-01-27 20:32:01.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-01-27 20:32:01.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.588096 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22207 2023-01-27 20:32:50.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-01-27 20:32:50.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:50.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:50.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-27 20:32:50.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-27 20:32:50.000000 mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 20:32:50.588096 mypy-boto3-appstream-1.26.59/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-01-27 20:32:00.000000 mypy-boto3-appstream-1.26.59/setup.py
```

### Comparing `mypy-boto3-appstream-1.26.164/LICENSE` & `mypy-boto3-appstream-1.26.59/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-appstream-1.26.164/PKG-INFO` & `mypy-boto3-appstream-1.26.59/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appstream
-Version: 1.26.164
-Summary: Type annotations for boto3.AppStream 1.26.164 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.59
+Summary: Type annotations for boto3.AppStream 1.26.59 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-appstream"></a>
 
 # mypy-boto3-appstream
 
 [![PyPI - mypy-boto3-appstream](https://img.shields.io/pypi/v/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appstream?color=blue)](https://pypistats.org/packages/mypy-boto3-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppStream 1.26.164](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[boto3.AppStream 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,19 +349,14 @@
 `mypy_boto3_appstream.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_appstream.literals import (
     AccessEndpointTypeType,
     ActionType,
-    AppBlockBuilderAttributeType,
-    AppBlockBuilderPlatformTypeType,
-    AppBlockBuilderStateChangeReasonCodeType,
-    AppBlockBuilderStateType,
-    AppBlockStateType,
     AppVisibilityType,
     ApplicationAttributeType,
     AuthenticationTypeType,
     CertificateBasedAuthStatusType,
     DescribeDirectoryConfigsPaginatorName,
     DescribeFleetsPaginatorName,
     DescribeImageBuildersPaginatorName,
@@ -379,15 +374,14 @@
     ImageBuilderStateChangeReasonCodeType,
     ImageBuilderStateType,
     ImageStateChangeReasonCodeType,
     ImageStateType,
     ListAssociatedFleetsPaginatorName,
     ListAssociatedStacksPaginatorName,
     MessageActionType,
-    PackagingTypeType,
     PermissionType,
     PlatformTypeType,
     PreferredProtocolType,
     SessionConnectionStateType,
     SessionStateType,
     StackAttributeType,
     StackErrorCodeType,
@@ -416,57 +410,48 @@
 
 `mypy_boto3_appstream.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appstream.type_defs import (
     AccessEndpointTypeDef,
-    AppBlockBuilderAppBlockAssociationTypeDef,
-    AppBlockBuilderStateChangeReasonTypeDef,
-    ResourceErrorTypeDef,
-    VpcConfigTypeDef,
-    ErrorDetailsTypeDef,
     S3LocationTypeDef,
     ApplicationFleetAssociationTypeDef,
     ApplicationSettingsResponseTypeDef,
     ApplicationSettingsTypeDef,
-    AssociateAppBlockBuilderAppBlockRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AssociateApplicationFleetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AssociateApplicationToEntitlementRequestRequestTypeDef,
     AssociateFleetRequestRequestTypeDef,
     UserStackAssociationTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityStatusTypeDef,
     ComputeCapacityTypeDef,
     CopyImageRequestRequestTypeDef,
-    CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
+    VpcConfigTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UserSettingTypeDef,
     CreateStreamingURLRequestRequestTypeDef,
     CreateUpdatedImageRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
-    DeleteAppBlockBuilderRequestRequestTypeDef,
     DeleteAppBlockRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteDirectoryConfigRequestRequestTypeDef,
     DeleteEntitlementRequestRequestTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteImageBuilderRequestRequestTypeDef,
     DeleteImagePermissionsRequestRequestTypeDef,
     DeleteImageRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
-    DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef,
-    DescribeAppBlockBuildersRequestRequestTypeDef,
     DescribeAppBlocksRequestRequestTypeDef,
     DescribeApplicationFleetAssociationsRequestRequestTypeDef,
     DescribeApplicationsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeDirectoryConfigsRequestRequestTypeDef,
     DescribeEntitlementsRequestRequestTypeDef,
     WaiterConfigTypeDef,
@@ -477,55 +462,47 @@
     DescribeSessionsRequestRequestTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeUsageReportSubscriptionsRequestRequestTypeDef,
     DescribeUserStackAssociationsRequestRequestTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UserTypeDef,
     DisableUserRequestRequestTypeDef,
-    DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     DisassociateApplicationFleetRequestRequestTypeDef,
     DisassociateApplicationFromEntitlementRequestRequestTypeDef,
     DisassociateFleetRequestRequestTypeDef,
     EnableUserRequestRequestTypeDef,
     EntitledApplicationTypeDef,
     ExpireSessionRequestRequestTypeDef,
     FleetErrorTypeDef,
     ImageBuilderStateChangeReasonTypeDef,
     NetworkAccessConfigurationTypeDef,
+    ResourceErrorTypeDef,
     ImagePermissionsTypeDef,
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
     ListAssociatedStacksRequestRequestTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     StackErrorTypeDef,
-    StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
-    StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AppBlockBuilderTypeDef,
-    CreateAppBlockBuilderRequestRequestTypeDef,
-    UpdateAppBlockBuilderRequestRequestTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     ScriptDetailsTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    AssociateAppBlockBuilderAppBlockResultTypeDef,
     AssociateApplicationFleetResultTypeDef,
     CopyImageResponseTypeDef,
-    CreateAppBlockBuilderStreamingURLResultTypeDef,
     CreateImageBuilderStreamingURLResultTypeDef,
     CreateStreamingURLResultTypeDef,
     CreateUsageReportSubscriptionResultTypeDef,
-    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
     ListAssociatedFleetsResultTypeDef,
     ListAssociatedStacksResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     BatchAssociateUserStackRequestRequestTypeDef,
     BatchDisassociateUserStackRequestRequestTypeDef,
     DescribeUserStackAssociationsResultTypeDef,
@@ -552,25 +529,20 @@
     ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
     ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
     DescribeFleetsRequestFleetStartedWaitTypeDef,
     DescribeFleetsRequestFleetStoppedWaitTypeDef,
     DescribeUsersResultTypeDef,
     ListEntitledApplicationsResultTypeDef,
     FleetTypeDef,
-    ImageBuilderTypeDef,
     SessionTypeDef,
+    ImageBuilderTypeDef,
     SharedImagePermissionsTypeDef,
     UpdateImagePermissionsRequestRequestTypeDef,
     UsageReportSubscriptionTypeDef,
     StackTypeDef,
-    CreateAppBlockBuilderResultTypeDef,
-    DescribeAppBlockBuildersResultTypeDef,
-    StartAppBlockBuilderResultTypeDef,
-    StopAppBlockBuilderResultTypeDef,
-    UpdateAppBlockBuilderResultTypeDef,
     CreateApplicationResultTypeDef,
     DescribeApplicationsResultTypeDef,
     ImageTypeDef,
     UpdateApplicationResultTypeDef,
     AppBlockTypeDef,
     CreateAppBlockRequestRequestTypeDef,
     BatchAssociateUserStackResultTypeDef,
@@ -580,20 +552,20 @@
     UpdateDirectoryConfigResultTypeDef,
     CreateEntitlementResultTypeDef,
     DescribeEntitlementsResultTypeDef,
     UpdateEntitlementResultTypeDef,
     CreateFleetResultTypeDef,
     DescribeFleetsResultTypeDef,
     UpdateFleetResultTypeDef,
+    DescribeSessionsResultTypeDef,
     CreateImageBuilderResultTypeDef,
     DeleteImageBuilderResultTypeDef,
     DescribeImageBuildersResultTypeDef,
     StartImageBuilderResultTypeDef,
     StopImageBuilderResultTypeDef,
-    DescribeSessionsResultTypeDef,
     DescribeImagePermissionsResultTypeDef,
     DescribeUsageReportSubscriptionsResultTypeDef,
     CreateStackResultTypeDef,
     DescribeStacksResultTypeDef,
     UpdateStackResultTypeDef,
     CreateUpdatedImageResultTypeDef,
     DeleteImageResultTypeDef,
@@ -610,42 +582,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-appstream-1.26.164/README.md` & `mypy-boto3-appstream-1.26.59/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-appstream"></a>
 
 # mypy-boto3-appstream
 
 [![PyPI - mypy-boto3-appstream](https://img.shields.io/pypi/v/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appstream?color=blue)](https://pypistats.org/packages/mypy-boto3-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppStream 1.26.164](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[boto3.AppStream 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,19 +317,14 @@
 `mypy_boto3_appstream.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_appstream.literals import (
     AccessEndpointTypeType,
     ActionType,
-    AppBlockBuilderAttributeType,
-    AppBlockBuilderPlatformTypeType,
-    AppBlockBuilderStateChangeReasonCodeType,
-    AppBlockBuilderStateType,
-    AppBlockStateType,
     AppVisibilityType,
     ApplicationAttributeType,
     AuthenticationTypeType,
     CertificateBasedAuthStatusType,
     DescribeDirectoryConfigsPaginatorName,
     DescribeFleetsPaginatorName,
     DescribeImageBuildersPaginatorName,
@@ -347,15 +342,14 @@
     ImageBuilderStateChangeReasonCodeType,
     ImageBuilderStateType,
     ImageStateChangeReasonCodeType,
     ImageStateType,
     ListAssociatedFleetsPaginatorName,
     ListAssociatedStacksPaginatorName,
     MessageActionType,
-    PackagingTypeType,
     PermissionType,
     PlatformTypeType,
     PreferredProtocolType,
     SessionConnectionStateType,
     SessionStateType,
     StackAttributeType,
     StackErrorCodeType,
@@ -384,57 +378,48 @@
 
 `mypy_boto3_appstream.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appstream.type_defs import (
     AccessEndpointTypeDef,
-    AppBlockBuilderAppBlockAssociationTypeDef,
-    AppBlockBuilderStateChangeReasonTypeDef,
-    ResourceErrorTypeDef,
-    VpcConfigTypeDef,
-    ErrorDetailsTypeDef,
     S3LocationTypeDef,
     ApplicationFleetAssociationTypeDef,
     ApplicationSettingsResponseTypeDef,
     ApplicationSettingsTypeDef,
-    AssociateAppBlockBuilderAppBlockRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AssociateApplicationFleetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AssociateApplicationToEntitlementRequestRequestTypeDef,
     AssociateFleetRequestRequestTypeDef,
     UserStackAssociationTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityStatusTypeDef,
     ComputeCapacityTypeDef,
     CopyImageRequestRequestTypeDef,
-    CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
+    VpcConfigTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UserSettingTypeDef,
     CreateStreamingURLRequestRequestTypeDef,
     CreateUpdatedImageRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
-    DeleteAppBlockBuilderRequestRequestTypeDef,
     DeleteAppBlockRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteDirectoryConfigRequestRequestTypeDef,
     DeleteEntitlementRequestRequestTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteImageBuilderRequestRequestTypeDef,
     DeleteImagePermissionsRequestRequestTypeDef,
     DeleteImageRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
-    DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef,
-    DescribeAppBlockBuildersRequestRequestTypeDef,
     DescribeAppBlocksRequestRequestTypeDef,
     DescribeApplicationFleetAssociationsRequestRequestTypeDef,
     DescribeApplicationsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeDirectoryConfigsRequestRequestTypeDef,
     DescribeEntitlementsRequestRequestTypeDef,
     WaiterConfigTypeDef,
@@ -445,55 +430,47 @@
     DescribeSessionsRequestRequestTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeUsageReportSubscriptionsRequestRequestTypeDef,
     DescribeUserStackAssociationsRequestRequestTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UserTypeDef,
     DisableUserRequestRequestTypeDef,
-    DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     DisassociateApplicationFleetRequestRequestTypeDef,
     DisassociateApplicationFromEntitlementRequestRequestTypeDef,
     DisassociateFleetRequestRequestTypeDef,
     EnableUserRequestRequestTypeDef,
     EntitledApplicationTypeDef,
     ExpireSessionRequestRequestTypeDef,
     FleetErrorTypeDef,
     ImageBuilderStateChangeReasonTypeDef,
     NetworkAccessConfigurationTypeDef,
+    ResourceErrorTypeDef,
     ImagePermissionsTypeDef,
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
     ListAssociatedStacksRequestRequestTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     StackErrorTypeDef,
-    StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
-    StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AppBlockBuilderTypeDef,
-    CreateAppBlockBuilderRequestRequestTypeDef,
-    UpdateAppBlockBuilderRequestRequestTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     ScriptDetailsTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    AssociateAppBlockBuilderAppBlockResultTypeDef,
     AssociateApplicationFleetResultTypeDef,
     CopyImageResponseTypeDef,
-    CreateAppBlockBuilderStreamingURLResultTypeDef,
     CreateImageBuilderStreamingURLResultTypeDef,
     CreateStreamingURLResultTypeDef,
     CreateUsageReportSubscriptionResultTypeDef,
-    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
     ListAssociatedFleetsResultTypeDef,
     ListAssociatedStacksResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     BatchAssociateUserStackRequestRequestTypeDef,
     BatchDisassociateUserStackRequestRequestTypeDef,
     DescribeUserStackAssociationsResultTypeDef,
@@ -520,25 +497,20 @@
     ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
     ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
     DescribeFleetsRequestFleetStartedWaitTypeDef,
     DescribeFleetsRequestFleetStoppedWaitTypeDef,
     DescribeUsersResultTypeDef,
     ListEntitledApplicationsResultTypeDef,
     FleetTypeDef,
-    ImageBuilderTypeDef,
     SessionTypeDef,
+    ImageBuilderTypeDef,
     SharedImagePermissionsTypeDef,
     UpdateImagePermissionsRequestRequestTypeDef,
     UsageReportSubscriptionTypeDef,
     StackTypeDef,
-    CreateAppBlockBuilderResultTypeDef,
-    DescribeAppBlockBuildersResultTypeDef,
-    StartAppBlockBuilderResultTypeDef,
-    StopAppBlockBuilderResultTypeDef,
-    UpdateAppBlockBuilderResultTypeDef,
     CreateApplicationResultTypeDef,
     DescribeApplicationsResultTypeDef,
     ImageTypeDef,
     UpdateApplicationResultTypeDef,
     AppBlockTypeDef,
     CreateAppBlockRequestRequestTypeDef,
     BatchAssociateUserStackResultTypeDef,
@@ -548,20 +520,20 @@
     UpdateDirectoryConfigResultTypeDef,
     CreateEntitlementResultTypeDef,
     DescribeEntitlementsResultTypeDef,
     UpdateEntitlementResultTypeDef,
     CreateFleetResultTypeDef,
     DescribeFleetsResultTypeDef,
     UpdateFleetResultTypeDef,
+    DescribeSessionsResultTypeDef,
     CreateImageBuilderResultTypeDef,
     DeleteImageBuilderResultTypeDef,
     DescribeImageBuildersResultTypeDef,
     StartImageBuilderResultTypeDef,
     StopImageBuilderResultTypeDef,
-    DescribeSessionsResultTypeDef,
     DescribeImagePermissionsResultTypeDef,
     DescribeUsageReportSubscriptionsResultTypeDef,
     CreateStackResultTypeDef,
     DescribeStacksResultTypeDef,
     UpdateStackResultTypeDef,
     CreateUpdatedImageResultTypeDef,
     DeleteImageResultTypeDef,
@@ -578,42 +550,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/__init__.py` & `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/__init__.pyi` & `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/__main__.py` & `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppStream 1.26.164\nVersion:         1.26.164\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.AppStream 1.26.59\nVersion:         1.26.59\nBuilder version:"
+        " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.164")
+    print("1.26.59")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/client.py` & `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,22 +15,20 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
-    AppBlockBuilderAttributeType,
     ApplicationAttributeType,
     AppVisibilityType,
     AuthenticationTypeType,
     FleetAttributeType,
     FleetTypeType,
     MessageActionType,
-    PackagingTypeType,
     PlatformTypeType,
     StackAttributeType,
     StreamViewType,
     VisibilityTypeType,
 )
 from .paginator import (
     DescribeDirectoryConfigsPaginator,
@@ -43,38 +41,33 @@
     DescribeUserStackAssociationsPaginator,
     ListAssociatedFleetsPaginator,
     ListAssociatedStacksPaginator,
 )
 from .type_defs import (
     AccessEndpointTypeDef,
     ApplicationSettingsTypeDef,
-    AssociateAppBlockBuilderAppBlockResultTypeDef,
     AssociateApplicationFleetResultTypeDef,
     BatchAssociateUserStackResultTypeDef,
     BatchDisassociateUserStackResultTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityTypeDef,
     CopyImageResponseTypeDef,
-    CreateAppBlockBuilderResultTypeDef,
-    CreateAppBlockBuilderStreamingURLResultTypeDef,
     CreateAppBlockResultTypeDef,
     CreateApplicationResultTypeDef,
     CreateDirectoryConfigResultTypeDef,
     CreateEntitlementResultTypeDef,
     CreateFleetResultTypeDef,
     CreateImageBuilderResultTypeDef,
     CreateImageBuilderStreamingURLResultTypeDef,
     CreateStackResultTypeDef,
     CreateStreamingURLResultTypeDef,
     CreateUpdatedImageResultTypeDef,
     CreateUsageReportSubscriptionResultTypeDef,
     DeleteImageBuilderResultTypeDef,
     DeleteImageResultTypeDef,
-    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
-    DescribeAppBlockBuildersResultTypeDef,
     DescribeAppBlocksResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
     DescribeApplicationsResultTypeDef,
     DescribeDirectoryConfigsResultTypeDef,
     DescribeEntitlementsResultTypeDef,
     DescribeFleetsResultTypeDef,
     DescribeImageBuildersResultTypeDef,
@@ -91,21 +84,18 @@
     ListAssociatedFleetsResultTypeDef,
     ListAssociatedStacksResultTypeDef,
     ListEntitledApplicationsResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     S3LocationTypeDef,
     ScriptDetailsTypeDef,
     ServiceAccountCredentialsTypeDef,
-    StartAppBlockBuilderResultTypeDef,
     StartImageBuilderResultTypeDef,
-    StopAppBlockBuilderResultTypeDef,
     StopImageBuilderResultTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
-    UpdateAppBlockBuilderResultTypeDef,
     UpdateApplicationResultTypeDef,
     UpdateDirectoryConfigResultTypeDef,
     UpdateEntitlementResultTypeDef,
     UpdateFleetResultTypeDef,
     UpdateStackResultTypeDef,
     UserSettingTypeDef,
     UserStackAssociationTypeDef,
@@ -161,24 +151,14 @@
         """
         AppStreamClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#exceptions)
         """
 
-    def associate_app_block_builder_app_block(
-        self, *, AppBlockArn: str, AppBlockBuilderName: str
-    ) -> AssociateAppBlockBuilderAppBlockResultTypeDef:
-        """
-        Associates the specified app block builder with the specified app block.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.associate_app_block_builder_app_block)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#associate_app_block_builder_app_block)
-        """
-
     def associate_application_fleet(
         self, *, FleetName: str, ApplicationArn: str
     ) -> AssociateApplicationFleetResultTypeDef:
         """
         Associates the specified application with the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.associate_application_fleet)
@@ -256,59 +236,26 @@
         """
 
     def create_app_block(
         self,
         *,
         Name: str,
         SourceS3Location: S3LocationTypeDef,
+        SetupScriptDetails: ScriptDetailsTypeDef,
         Description: str = ...,
         DisplayName: str = ...,
-        SetupScriptDetails: ScriptDetailsTypeDef = ...,
-        Tags: Mapping[str, str] = ...,
-        PostSetupScriptDetails: ScriptDetailsTypeDef = ...,
-        PackagingType: PackagingTypeType = ...
+        Tags: Mapping[str, str] = ...
     ) -> CreateAppBlockResultTypeDef:
         """
         Creates an app block.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#create_app_block)
         """
 
-    def create_app_block_builder(
-        self,
-        *,
-        Name: str,
-        Platform: Literal["WINDOWS_SERVER_2019"],
-        InstanceType: str,
-        VpcConfig: VpcConfigTypeDef,
-        Description: str = ...,
-        DisplayName: str = ...,
-        Tags: Mapping[str, str] = ...,
-        EnableDefaultInternetAccess: bool = ...,
-        IamRoleArn: str = ...,
-        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
-    ) -> CreateAppBlockBuilderResultTypeDef:
-        """
-        Creates an app block builder.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block_builder)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#create_app_block_builder)
-        """
-
-    def create_app_block_builder_streaming_url(
-        self, *, AppBlockBuilderName: str, Validity: int = ...
-    ) -> CreateAppBlockBuilderStreamingURLResultTypeDef:
-        """
-        Creates a URL to start a create app block builder streaming session.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block_builder_streaming_url)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#create_app_block_builder_streaming_url)
-        """
-
     def create_application(
         self,
         *,
         Name: str,
         IconS3Location: S3LocationTypeDef,
         LaunchPath: str,
         Platforms: Sequence[PlatformTypeType],
@@ -511,22 +458,14 @@
         """
         Deletes an app block.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_app_block)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#delete_app_block)
         """
 
-    def delete_app_block_builder(self, *, Name: str) -> Dict[str, Any]:
-        """
-        Deletes an app block builder.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_app_block_builder)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#delete_app_block_builder)
-        """
-
     def delete_application(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#delete_application)
         """
@@ -601,39 +540,14 @@
         """
         Deletes a user from the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#delete_user)
         """
 
-    def describe_app_block_builder_app_block_associations(
-        self,
-        *,
-        AppBlockArn: str = ...,
-        AppBlockBuilderName: str = ...,
-        MaxResults: int = ...,
-        NextToken: str = ...
-    ) -> DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef:
-        """
-        Retrieves a list that describes one or more app block builder associations.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_block_builder_app_block_associations)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#describe_app_block_builder_app_block_associations)
-        """
-
-    def describe_app_block_builders(
-        self, *, Names: Sequence[str] = ..., NextToken: str = ..., MaxResults: int = ...
-    ) -> DescribeAppBlockBuildersResultTypeDef:
-        """
-        Retrieves a list that describes one or more app block builders.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_block_builders)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#describe_app_block_builders)
-        """
-
     def describe_app_blocks(
         self, *, Arns: Sequence[str] = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeAppBlocksResultTypeDef:
         """
         Retrieves a list that describes one or more app blocks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_blocks)
@@ -816,24 +730,14 @@
         """
         Disables the specified user in the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disable_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#disable_user)
         """
 
-    def disassociate_app_block_builder_app_block(
-        self, *, AppBlockArn: str, AppBlockBuilderName: str
-    ) -> Dict[str, Any]:
-        """
-        Disassociates a specified app block builder from a specified app block.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disassociate_app_block_builder_app_block)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#disassociate_app_block_builder_app_block)
-        """
-
     def disassociate_application_fleet(
         self, *, FleetName: str, ApplicationArn: str
     ) -> Dict[str, Any]:
         """
         Disassociates the specified application from the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disassociate_application_fleet)
@@ -924,22 +828,14 @@
         """
         Retrieves a list of all tags for the specified AppStream 2.0 resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#list_tags_for_resource)
         """
 
-    def start_app_block_builder(self, *, Name: str) -> StartAppBlockBuilderResultTypeDef:
-        """
-        Starts an app block builder.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_app_block_builder)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#start_app_block_builder)
-        """
-
     def start_fleet(self, *, Name: str) -> Dict[str, Any]:
         """
         Starts the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#start_fleet)
         """
@@ -950,22 +846,14 @@
         """
         Starts the specified image builder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_image_builder)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#start_image_builder)
         """
 
-    def stop_app_block_builder(self, *, Name: str) -> StopAppBlockBuilderResultTypeDef:
-        """
-        Stops an app block builder.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.stop_app_block_builder)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#stop_app_block_builder)
-        """
-
     def stop_fleet(self, *, Name: str) -> Dict[str, Any]:
         """
         Stops the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.stop_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#stop_fleet)
         """
@@ -991,35 +879,14 @@
         Disassociates one or more specified tags from the specified AppStream 2.0
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#untag_resource)
         """
 
-    def update_app_block_builder(
-        self,
-        *,
-        Name: str,
-        Description: str = ...,
-        DisplayName: str = ...,
-        Platform: PlatformTypeType = ...,
-        InstanceType: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
-        EnableDefaultInternetAccess: bool = ...,
-        IamRoleArn: str = ...,
-        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
-        AttributesToDelete: Sequence[AppBlockBuilderAttributeType] = ...
-    ) -> UpdateAppBlockBuilderResultTypeDef:
-        """
-        Updates an app block builder.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_app_block_builder)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#update_app_block_builder)
-        """
-
     def update_application(
         self,
         *,
         Name: str,
         DisplayName: str = ...,
         Description: str = ...,
         IconS3Location: S3LocationTypeDef = ...,
```

### Comparing `mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/client.pyi` & `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/client.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -15,22 +15,20 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
-    AppBlockBuilderAttributeType,
     ApplicationAttributeType,
     AppVisibilityType,
     AuthenticationTypeType,
     FleetAttributeType,
     FleetTypeType,
     MessageActionType,
-    PackagingTypeType,
     PlatformTypeType,
     StackAttributeType,
     StreamViewType,
     VisibilityTypeType,
 )
 from .paginator import (
     DescribeDirectoryConfigsPaginator,
@@ -43,38 +41,33 @@
     DescribeUserStackAssociationsPaginator,
     ListAssociatedFleetsPaginator,
     ListAssociatedStacksPaginator,
 )
 from .type_defs import (
     AccessEndpointTypeDef,
     ApplicationSettingsTypeDef,
-    AssociateAppBlockBuilderAppBlockResultTypeDef,
     AssociateApplicationFleetResultTypeDef,
     BatchAssociateUserStackResultTypeDef,
     BatchDisassociateUserStackResultTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityTypeDef,
     CopyImageResponseTypeDef,
-    CreateAppBlockBuilderResultTypeDef,
-    CreateAppBlockBuilderStreamingURLResultTypeDef,
     CreateAppBlockResultTypeDef,
     CreateApplicationResultTypeDef,
     CreateDirectoryConfigResultTypeDef,
     CreateEntitlementResultTypeDef,
     CreateFleetResultTypeDef,
     CreateImageBuilderResultTypeDef,
     CreateImageBuilderStreamingURLResultTypeDef,
     CreateStackResultTypeDef,
     CreateStreamingURLResultTypeDef,
     CreateUpdatedImageResultTypeDef,
     CreateUsageReportSubscriptionResultTypeDef,
     DeleteImageBuilderResultTypeDef,
     DeleteImageResultTypeDef,
-    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
-    DescribeAppBlockBuildersResultTypeDef,
     DescribeAppBlocksResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
     DescribeApplicationsResultTypeDef,
     DescribeDirectoryConfigsResultTypeDef,
     DescribeEntitlementsResultTypeDef,
     DescribeFleetsResultTypeDef,
     DescribeImageBuildersResultTypeDef,
@@ -91,21 +84,18 @@
     ListAssociatedFleetsResultTypeDef,
     ListAssociatedStacksResultTypeDef,
     ListEntitledApplicationsResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     S3LocationTypeDef,
     ScriptDetailsTypeDef,
     ServiceAccountCredentialsTypeDef,
-    StartAppBlockBuilderResultTypeDef,
     StartImageBuilderResultTypeDef,
-    StopAppBlockBuilderResultTypeDef,
     StopImageBuilderResultTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
-    UpdateAppBlockBuilderResultTypeDef,
     UpdateApplicationResultTypeDef,
     UpdateDirectoryConfigResultTypeDef,
     UpdateEntitlementResultTypeDef,
     UpdateFleetResultTypeDef,
     UpdateStackResultTypeDef,
     UserSettingTypeDef,
     UserStackAssociationTypeDef,
@@ -156,23 +146,14 @@
     def exceptions(self) -> Exceptions:
         """
         AppStreamClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#exceptions)
         """
-    def associate_app_block_builder_app_block(
-        self, *, AppBlockArn: str, AppBlockBuilderName: str
-    ) -> AssociateAppBlockBuilderAppBlockResultTypeDef:
-        """
-        Associates the specified app block builder with the specified app block.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.associate_app_block_builder_app_block)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#associate_app_block_builder_app_block)
-        """
     def associate_application_fleet(
         self, *, FleetName: str, ApplicationArn: str
     ) -> AssociateApplicationFleetResultTypeDef:
         """
         Associates the specified application with the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.associate_application_fleet)
@@ -242,56 +223,25 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#copy_image)
         """
     def create_app_block(
         self,
         *,
         Name: str,
         SourceS3Location: S3LocationTypeDef,
+        SetupScriptDetails: ScriptDetailsTypeDef,
         Description: str = ...,
         DisplayName: str = ...,
-        SetupScriptDetails: ScriptDetailsTypeDef = ...,
-        Tags: Mapping[str, str] = ...,
-        PostSetupScriptDetails: ScriptDetailsTypeDef = ...,
-        PackagingType: PackagingTypeType = ...
+        Tags: Mapping[str, str] = ...
     ) -> CreateAppBlockResultTypeDef:
         """
         Creates an app block.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#create_app_block)
         """
-    def create_app_block_builder(
-        self,
-        *,
-        Name: str,
-        Platform: Literal["WINDOWS_SERVER_2019"],
-        InstanceType: str,
-        VpcConfig: VpcConfigTypeDef,
-        Description: str = ...,
-        DisplayName: str = ...,
-        Tags: Mapping[str, str] = ...,
-        EnableDefaultInternetAccess: bool = ...,
-        IamRoleArn: str = ...,
-        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
-    ) -> CreateAppBlockBuilderResultTypeDef:
-        """
-        Creates an app block builder.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block_builder)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#create_app_block_builder)
-        """
-    def create_app_block_builder_streaming_url(
-        self, *, AppBlockBuilderName: str, Validity: int = ...
-    ) -> CreateAppBlockBuilderStreamingURLResultTypeDef:
-        """
-        Creates a URL to start a create app block builder streaming session.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block_builder_streaming_url)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#create_app_block_builder_streaming_url)
-        """
     def create_application(
         self,
         *,
         Name: str,
         IconS3Location: S3LocationTypeDef,
         LaunchPath: str,
         Platforms: Sequence[PlatformTypeType],
@@ -482,21 +432,14 @@
     def delete_app_block(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes an app block.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_app_block)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#delete_app_block)
         """
-    def delete_app_block_builder(self, *, Name: str) -> Dict[str, Any]:
-        """
-        Deletes an app block builder.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_app_block_builder)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#delete_app_block_builder)
-        """
     def delete_application(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#delete_application)
         """
@@ -561,37 +504,14 @@
     ) -> Dict[str, Any]:
         """
         Deletes a user from the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#delete_user)
         """
-    def describe_app_block_builder_app_block_associations(
-        self,
-        *,
-        AppBlockArn: str = ...,
-        AppBlockBuilderName: str = ...,
-        MaxResults: int = ...,
-        NextToken: str = ...
-    ) -> DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef:
-        """
-        Retrieves a list that describes one or more app block builder associations.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_block_builder_app_block_associations)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#describe_app_block_builder_app_block_associations)
-        """
-    def describe_app_block_builders(
-        self, *, Names: Sequence[str] = ..., NextToken: str = ..., MaxResults: int = ...
-    ) -> DescribeAppBlockBuildersResultTypeDef:
-        """
-        Retrieves a list that describes one or more app block builders.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_block_builders)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#describe_app_block_builders)
-        """
     def describe_app_blocks(
         self, *, Arns: Sequence[str] = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeAppBlocksResultTypeDef:
         """
         Retrieves a list that describes one or more app blocks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_blocks)
@@ -759,23 +679,14 @@
     ) -> Dict[str, Any]:
         """
         Disables the specified user in the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disable_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#disable_user)
         """
-    def disassociate_app_block_builder_app_block(
-        self, *, AppBlockArn: str, AppBlockBuilderName: str
-    ) -> Dict[str, Any]:
-        """
-        Disassociates a specified app block builder from a specified app block.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disassociate_app_block_builder_app_block)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#disassociate_app_block_builder_app_block)
-        """
     def disassociate_application_fleet(
         self, *, FleetName: str, ApplicationArn: str
     ) -> Dict[str, Any]:
         """
         Disassociates the specified application from the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disassociate_application_fleet)
@@ -856,21 +767,14 @@
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Retrieves a list of all tags for the specified AppStream 2.0 resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#list_tags_for_resource)
         """
-    def start_app_block_builder(self, *, Name: str) -> StartAppBlockBuilderResultTypeDef:
-        """
-        Starts an app block builder.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_app_block_builder)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#start_app_block_builder)
-        """
     def start_fleet(self, *, Name: str) -> Dict[str, Any]:
         """
         Starts the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#start_fleet)
         """
@@ -879,21 +783,14 @@
     ) -> StartImageBuilderResultTypeDef:
         """
         Starts the specified image builder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_image_builder)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#start_image_builder)
         """
-    def stop_app_block_builder(self, *, Name: str) -> StopAppBlockBuilderResultTypeDef:
-        """
-        Stops an app block builder.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.stop_app_block_builder)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#stop_app_block_builder)
-        """
     def stop_fleet(self, *, Name: str) -> Dict[str, Any]:
         """
         Stops the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.stop_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#stop_fleet)
         """
@@ -915,34 +812,14 @@
         """
         Disassociates one or more specified tags from the specified AppStream 2.0
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#untag_resource)
         """
-    def update_app_block_builder(
-        self,
-        *,
-        Name: str,
-        Description: str = ...,
-        DisplayName: str = ...,
-        Platform: PlatformTypeType = ...,
-        InstanceType: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
-        EnableDefaultInternetAccess: bool = ...,
-        IamRoleArn: str = ...,
-        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
-        AttributesToDelete: Sequence[AppBlockBuilderAttributeType] = ...
-    ) -> UpdateAppBlockBuilderResultTypeDef:
-        """
-        Updates an app block builder.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_app_block_builder)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/client/#update_app_block_builder)
-        """
     def update_application(
         self,
         *,
         Name: str,
         DisplayName: str = ...,
         Description: str = ...,
         IconS3Location: S3LocationTypeDef = ...,
```

### Comparing `mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/literals.py` & `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -14,23 +14,17 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AccessEndpointTypeType",
     "ActionType",
-    "AppBlockBuilderAttributeType",
-    "AppBlockBuilderPlatformTypeType",
-    "AppBlockBuilderStateChangeReasonCodeType",
-    "AppBlockBuilderStateType",
-    "AppBlockStateType",
     "AppVisibilityType",
     "ApplicationAttributeType",
     "AuthenticationTypeType",
     "CertificateBasedAuthStatusType",
     "DescribeDirectoryConfigsPaginatorName",
     "DescribeFleetsPaginatorName",
     "DescribeImageBuildersPaginatorName",
@@ -48,15 +42,14 @@
     "ImageBuilderStateChangeReasonCodeType",
     "ImageBuilderStateType",
     "ImageStateChangeReasonCodeType",
     "ImageStateType",
     "ListAssociatedFleetsPaginatorName",
     "ListAssociatedStacksPaginatorName",
     "MessageActionType",
-    "PackagingTypeType",
     "PermissionType",
     "PlatformTypeType",
     "PreferredProtocolType",
     "SessionConnectionStateType",
     "SessionStateType",
     "StackAttributeType",
     "StackErrorCodeType",
@@ -70,32 +63,24 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AccessEndpointTypeType = Literal["STREAMING"]
 ActionType = Literal[
     "CLIPBOARD_COPY_FROM_LOCAL_DEVICE",
     "CLIPBOARD_COPY_TO_LOCAL_DEVICE",
     "DOMAIN_PASSWORD_SIGNIN",
     "DOMAIN_SMART_CARD_SIGNIN",
     "FILE_DOWNLOAD",
     "FILE_UPLOAD",
     "PRINTING_TO_LOCAL_DEVICE",
 ]
-AppBlockBuilderAttributeType = Literal[
-    "ACCESS_ENDPOINTS", "IAM_ROLE_ARN", "VPC_CONFIGURATION_SECURITY_GROUP_IDS"
-]
-AppBlockBuilderPlatformTypeType = Literal["WINDOWS_SERVER_2019"]
-AppBlockBuilderStateChangeReasonCodeType = Literal["INTERNAL_ERROR"]
-AppBlockBuilderStateType = Literal["RUNNING", "STARTING", "STOPPED", "STOPPING"]
-AppBlockStateType = Literal["ACTIVE", "INACTIVE"]
 AppVisibilityType = Literal["ALL", "ASSOCIATED"]
 ApplicationAttributeType = Literal["LAUNCH_PARAMETERS", "WORKING_DIRECTORY"]
 AuthenticationTypeType = Literal["API", "AWS_AD", "SAML", "USERPOOL"]
 CertificateBasedAuthStatusType = Literal[
     "DISABLED", "ENABLED", "ENABLED_NO_DIRECTORY_LOGIN_FALLBACK"
 ]
 DescribeDirectoryConfigsPaginatorName = Literal["describe_directory_configs"]
@@ -169,15 +154,14 @@
 ]
 ImageStateType = Literal[
     "AVAILABLE", "COPYING", "CREATING", "DELETING", "FAILED", "IMPORTING", "PENDING"
 ]
 ListAssociatedFleetsPaginatorName = Literal["list_associated_fleets"]
 ListAssociatedStacksPaginatorName = Literal["list_associated_stacks"]
 MessageActionType = Literal["RESEND", "SUPPRESS"]
-PackagingTypeType = Literal["APPSTREAM2", "CUSTOM"]
 PermissionType = Literal["DISABLED", "ENABLED"]
 PlatformTypeType = Literal["AMAZON_LINUX2", "WINDOWS", "WINDOWS_SERVER_2016", "WINDOWS_SERVER_2019"]
 PreferredProtocolType = Literal["TCP", "UDP"]
 SessionConnectionStateType = Literal["CONNECTED", "NOT_CONNECTED"]
 SessionStateType = Literal["ACTIVE", "EXPIRED", "PENDING"]
 StackAttributeType = Literal[
     "ACCESS_ENDPOINTS",
@@ -216,15 +200,14 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
-    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -256,23 +239,21 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
-    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -351,15 +332,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -370,15 +350,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -414,15 +393,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -441,19 +419,16 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
-    "payment-cryptography",
-    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -533,21 +508,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
-    "verifiedpermissions",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/literals.pyi` & `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,22 +14,18 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AccessEndpointTypeType",
     "ActionType",
-    "AppBlockBuilderAttributeType",
-    "AppBlockBuilderPlatformTypeType",
-    "AppBlockBuilderStateChangeReasonCodeType",
-    "AppBlockBuilderStateType",
-    "AppBlockStateType",
     "AppVisibilityType",
     "ApplicationAttributeType",
     "AuthenticationTypeType",
     "CertificateBasedAuthStatusType",
     "DescribeDirectoryConfigsPaginatorName",
     "DescribeFleetsPaginatorName",
     "DescribeImageBuildersPaginatorName",
@@ -47,15 +43,14 @@
     "ImageBuilderStateChangeReasonCodeType",
     "ImageBuilderStateType",
     "ImageStateChangeReasonCodeType",
     "ImageStateType",
     "ListAssociatedFleetsPaginatorName",
     "ListAssociatedStacksPaginatorName",
     "MessageActionType",
-    "PackagingTypeType",
     "PermissionType",
     "PlatformTypeType",
     "PreferredProtocolType",
     "SessionConnectionStateType",
     "SessionStateType",
     "StackAttributeType",
     "StackErrorCodeType",
@@ -69,31 +64,25 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AccessEndpointTypeType = Literal["STREAMING"]
 ActionType = Literal[
     "CLIPBOARD_COPY_FROM_LOCAL_DEVICE",
     "CLIPBOARD_COPY_TO_LOCAL_DEVICE",
     "DOMAIN_PASSWORD_SIGNIN",
     "DOMAIN_SMART_CARD_SIGNIN",
     "FILE_DOWNLOAD",
     "FILE_UPLOAD",
     "PRINTING_TO_LOCAL_DEVICE",
 ]
-AppBlockBuilderAttributeType = Literal[
-    "ACCESS_ENDPOINTS", "IAM_ROLE_ARN", "VPC_CONFIGURATION_SECURITY_GROUP_IDS"
-]
-AppBlockBuilderPlatformTypeType = Literal["WINDOWS_SERVER_2019"]
-AppBlockBuilderStateChangeReasonCodeType = Literal["INTERNAL_ERROR"]
-AppBlockBuilderStateType = Literal["RUNNING", "STARTING", "STOPPED", "STOPPING"]
-AppBlockStateType = Literal["ACTIVE", "INACTIVE"]
 AppVisibilityType = Literal["ALL", "ASSOCIATED"]
 ApplicationAttributeType = Literal["LAUNCH_PARAMETERS", "WORKING_DIRECTORY"]
 AuthenticationTypeType = Literal["API", "AWS_AD", "SAML", "USERPOOL"]
 CertificateBasedAuthStatusType = Literal[
     "DISABLED", "ENABLED", "ENABLED_NO_DIRECTORY_LOGIN_FALLBACK"
 ]
 DescribeDirectoryConfigsPaginatorName = Literal["describe_directory_configs"]
@@ -167,15 +156,14 @@
 ]
 ImageStateType = Literal[
     "AVAILABLE", "COPYING", "CREATING", "DELETING", "FAILED", "IMPORTING", "PENDING"
 ]
 ListAssociatedFleetsPaginatorName = Literal["list_associated_fleets"]
 ListAssociatedStacksPaginatorName = Literal["list_associated_stacks"]
 MessageActionType = Literal["RESEND", "SUPPRESS"]
-PackagingTypeType = Literal["APPSTREAM2", "CUSTOM"]
 PermissionType = Literal["DISABLED", "ENABLED"]
 PlatformTypeType = Literal["AMAZON_LINUX2", "WINDOWS", "WINDOWS_SERVER_2016", "WINDOWS_SERVER_2019"]
 PreferredProtocolType = Literal["TCP", "UDP"]
 SessionConnectionStateType = Literal["CONNECTED", "NOT_CONNECTED"]
 SessionStateType = Literal["ACTIVE", "EXPIRED", "PENDING"]
 StackAttributeType = Literal[
     "ACCESS_ENDPOINTS",
@@ -214,15 +202,14 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
-    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -254,23 +241,21 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
-    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -349,15 +334,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -368,15 +352,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -412,15 +395,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -439,19 +421,16 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
-    "payment-cryptography",
-    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -531,21 +510,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
-    "verifiedpermissions",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/paginator.py` & `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/paginator.pyi` & `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/type_defs.py` & `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,31 +13,27 @@
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ActionType,
-    AppBlockBuilderAttributeType,
-    AppBlockBuilderStateType,
-    AppBlockStateType,
     ApplicationAttributeType,
     AppVisibilityType,
     AuthenticationTypeType,
     CertificateBasedAuthStatusType,
     FleetAttributeType,
     FleetErrorCodeType,
     FleetStateType,
     FleetTypeType,
     ImageBuilderStateChangeReasonCodeType,
     ImageBuilderStateType,
     ImageStateChangeReasonCodeType,
     ImageStateType,
     MessageActionType,
-    PackagingTypeType,
     PermissionType,
     PlatformTypeType,
     PreferredProtocolType,
     SessionConnectionStateType,
     SessionStateType,
     StackAttributeType,
     StackErrorCodeType,
@@ -56,57 +52,48 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessEndpointTypeDef",
-    "AppBlockBuilderAppBlockAssociationTypeDef",
-    "AppBlockBuilderStateChangeReasonTypeDef",
-    "ResourceErrorTypeDef",
-    "VpcConfigTypeDef",
-    "ErrorDetailsTypeDef",
     "S3LocationTypeDef",
     "ApplicationFleetAssociationTypeDef",
     "ApplicationSettingsResponseTypeDef",
     "ApplicationSettingsTypeDef",
-    "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AssociateApplicationFleetRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateApplicationToEntitlementRequestRequestTypeDef",
     "AssociateFleetRequestRequestTypeDef",
     "UserStackAssociationTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
     "ComputeCapacityStatusTypeDef",
     "ComputeCapacityTypeDef",
     "CopyImageRequestRequestTypeDef",
-    "CreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
     "ServiceAccountCredentialsTypeDef",
     "EntitlementAttributeTypeDef",
     "DomainJoinInfoTypeDef",
+    "VpcConfigTypeDef",
     "CreateImageBuilderStreamingURLRequestRequestTypeDef",
     "StorageConnectorTypeDef",
     "StreamingExperienceSettingsTypeDef",
     "UserSettingTypeDef",
     "CreateStreamingURLRequestRequestTypeDef",
     "CreateUpdatedImageRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "DeleteAppBlockBuilderRequestRequestTypeDef",
     "DeleteAppBlockRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteDirectoryConfigRequestRequestTypeDef",
     "DeleteEntitlementRequestRequestTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteImageBuilderRequestRequestTypeDef",
     "DeleteImagePermissionsRequestRequestTypeDef",
     "DeleteImageRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
-    "DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef",
-    "DescribeAppBlockBuildersRequestRequestTypeDef",
     "DescribeAppBlocksRequestRequestTypeDef",
     "DescribeApplicationFleetAssociationsRequestRequestTypeDef",
     "DescribeApplicationsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeDirectoryConfigsRequestRequestTypeDef",
     "DescribeEntitlementsRequestRequestTypeDef",
     "WaiterConfigTypeDef",
@@ -117,55 +104,47 @@
     "DescribeSessionsRequestRequestTypeDef",
     "DescribeStacksRequestRequestTypeDef",
     "DescribeUsageReportSubscriptionsRequestRequestTypeDef",
     "DescribeUserStackAssociationsRequestRequestTypeDef",
     "DescribeUsersRequestRequestTypeDef",
     "UserTypeDef",
     "DisableUserRequestRequestTypeDef",
-    "DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     "DisassociateApplicationFleetRequestRequestTypeDef",
     "DisassociateApplicationFromEntitlementRequestRequestTypeDef",
     "DisassociateFleetRequestRequestTypeDef",
     "EnableUserRequestRequestTypeDef",
     "EntitledApplicationTypeDef",
     "ExpireSessionRequestRequestTypeDef",
     "FleetErrorTypeDef",
     "ImageBuilderStateChangeReasonTypeDef",
     "NetworkAccessConfigurationTypeDef",
+    "ResourceErrorTypeDef",
     "ImagePermissionsTypeDef",
     "ImageStateChangeReasonTypeDef",
     "LastReportGenerationExecutionErrorTypeDef",
     "ListAssociatedFleetsRequestRequestTypeDef",
     "ListAssociatedStacksRequestRequestTypeDef",
     "ListEntitledApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "StackErrorTypeDef",
-    "StartAppBlockBuilderRequestRequestTypeDef",
     "StartFleetRequestRequestTypeDef",
     "StartImageBuilderRequestRequestTypeDef",
-    "StopAppBlockBuilderRequestRequestTypeDef",
     "StopFleetRequestRequestTypeDef",
     "StopImageBuilderRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AppBlockBuilderTypeDef",
-    "CreateAppBlockBuilderRequestRequestTypeDef",
-    "UpdateAppBlockBuilderRequestRequestTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "ScriptDetailsTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "AssociateAppBlockBuilderAppBlockResultTypeDef",
     "AssociateApplicationFleetResultTypeDef",
     "CopyImageResponseTypeDef",
-    "CreateAppBlockBuilderStreamingURLResultTypeDef",
     "CreateImageBuilderStreamingURLResultTypeDef",
     "CreateStreamingURLResultTypeDef",
     "CreateUsageReportSubscriptionResultTypeDef",
-    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
     "DescribeApplicationFleetAssociationsResultTypeDef",
     "ListAssociatedFleetsResultTypeDef",
     "ListAssociatedStacksResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "BatchAssociateUserStackRequestRequestTypeDef",
     "BatchDisassociateUserStackRequestRequestTypeDef",
     "DescribeUserStackAssociationsResultTypeDef",
@@ -192,25 +171,20 @@
     "ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
     "ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
     "DescribeFleetsRequestFleetStartedWaitTypeDef",
     "DescribeFleetsRequestFleetStoppedWaitTypeDef",
     "DescribeUsersResultTypeDef",
     "ListEntitledApplicationsResultTypeDef",
     "FleetTypeDef",
-    "ImageBuilderTypeDef",
     "SessionTypeDef",
+    "ImageBuilderTypeDef",
     "SharedImagePermissionsTypeDef",
     "UpdateImagePermissionsRequestRequestTypeDef",
     "UsageReportSubscriptionTypeDef",
     "StackTypeDef",
-    "CreateAppBlockBuilderResultTypeDef",
-    "DescribeAppBlockBuildersResultTypeDef",
-    "StartAppBlockBuilderResultTypeDef",
-    "StopAppBlockBuilderResultTypeDef",
-    "UpdateAppBlockBuilderResultTypeDef",
     "CreateApplicationResultTypeDef",
     "DescribeApplicationsResultTypeDef",
     "ImageTypeDef",
     "UpdateApplicationResultTypeDef",
     "AppBlockTypeDef",
     "CreateAppBlockRequestRequestTypeDef",
     "BatchAssociateUserStackResultTypeDef",
@@ -220,20 +194,20 @@
     "UpdateDirectoryConfigResultTypeDef",
     "CreateEntitlementResultTypeDef",
     "DescribeEntitlementsResultTypeDef",
     "UpdateEntitlementResultTypeDef",
     "CreateFleetResultTypeDef",
     "DescribeFleetsResultTypeDef",
     "UpdateFleetResultTypeDef",
+    "DescribeSessionsResultTypeDef",
     "CreateImageBuilderResultTypeDef",
     "DeleteImageBuilderResultTypeDef",
     "DescribeImageBuildersResultTypeDef",
     "StartImageBuilderResultTypeDef",
     "StopImageBuilderResultTypeDef",
-    "DescribeSessionsResultTypeDef",
     "DescribeImagePermissionsResultTypeDef",
     "DescribeUsageReportSubscriptionsResultTypeDef",
     "CreateStackResultTypeDef",
     "DescribeStacksResultTypeDef",
     "UpdateStackResultTypeDef",
     "CreateUpdatedImageResultTypeDef",
     "DeleteImageResultTypeDef",
@@ -257,78 +231,22 @@
 )
 
 
 class AccessEndpointTypeDef(_RequiredAccessEndpointTypeDef, _OptionalAccessEndpointTypeDef):
     pass
 
 
-AppBlockBuilderAppBlockAssociationTypeDef = TypedDict(
-    "AppBlockBuilderAppBlockAssociationTypeDef",
-    {
-        "AppBlockArn": str,
-        "AppBlockBuilderName": str,
-    },
-)
-
-AppBlockBuilderStateChangeReasonTypeDef = TypedDict(
-    "AppBlockBuilderStateChangeReasonTypeDef",
-    {
-        "Code": Literal["INTERNAL_ERROR"],
-        "Message": str,
-    },
-    total=False,
-)
-
-ResourceErrorTypeDef = TypedDict(
-    "ResourceErrorTypeDef",
-    {
-        "ErrorCode": FleetErrorCodeType,
-        "ErrorMessage": str,
-        "ErrorTimestamp": datetime,
-    },
-    total=False,
-)
-
-VpcConfigTypeDef = TypedDict(
-    "VpcConfigTypeDef",
-    {
-        "SubnetIds": Sequence[str],
-        "SecurityGroupIds": Sequence[str],
-    },
-    total=False,
-)
-
-ErrorDetailsTypeDef = TypedDict(
-    "ErrorDetailsTypeDef",
-    {
-        "ErrorCode": str,
-        "ErrorMessage": str,
-    },
-    total=False,
-)
-
-_RequiredS3LocationTypeDef = TypedDict(
-    "_RequiredS3LocationTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
         "S3Bucket": str,
-    },
-)
-_OptionalS3LocationTypeDef = TypedDict(
-    "_OptionalS3LocationTypeDef",
-    {
         "S3Key": str,
     },
-    total=False,
 )
 
-
-class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
-    pass
-
-
 ApplicationFleetAssociationTypeDef = TypedDict(
     "ApplicationFleetAssociationTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
     },
 )
@@ -360,41 +278,33 @@
 
 class ApplicationSettingsTypeDef(
     _RequiredApplicationSettingsTypeDef, _OptionalApplicationSettingsTypeDef
 ):
     pass
 
 
-AssociateAppBlockBuilderAppBlockRequestRequestTypeDef = TypedDict(
-    "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
+AssociateApplicationFleetRequestRequestTypeDef = TypedDict(
+    "AssociateApplicationFleetRequestRequestTypeDef",
     {
-        "AppBlockArn": str,
-        "AppBlockBuilderName": str,
+        "FleetName": str,
+        "ApplicationArn": str,
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-AssociateApplicationFleetRequestRequestTypeDef = TypedDict(
-    "AssociateApplicationFleetRequestRequestTypeDef",
-    {
-        "FleetName": str,
-        "ApplicationArn": str,
-    },
-)
-
 AssociateApplicationToEntitlementRequestRequestTypeDef = TypedDict(
     "AssociateApplicationToEntitlementRequestRequestTypeDef",
     {
         "StackName": str,
         "EntitlementName": str,
         "ApplicationIdentifier": str,
     },
@@ -489,36 +399,14 @@
 
 class CopyImageRequestRequestTypeDef(
     _RequiredCopyImageRequestRequestTypeDef, _OptionalCopyImageRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
-    {
-        "AppBlockBuilderName": str,
-    },
-)
-_OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
-    {
-        "Validity": int,
-    },
-    total=False,
-)
-
-
-class CreateAppBlockBuilderStreamingURLRequestRequestTypeDef(
-    _RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
-    _OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
-):
-    pass
-
-
 ServiceAccountCredentialsTypeDef = TypedDict(
     "ServiceAccountCredentialsTypeDef",
     {
         "AccountName": str,
         "AccountPassword": str,
     },
 )
@@ -536,14 +424,23 @@
     {
         "DirectoryName": str,
         "OrganizationalUnitDistinguishedName": str,
     },
     total=False,
 )
 
+VpcConfigTypeDef = TypedDict(
+    "VpcConfigTypeDef",
+    {
+        "SubnetIds": Sequence[str],
+        "SecurityGroupIds": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef = TypedDict(
@@ -670,21 +567,14 @@
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
 
-DeleteAppBlockBuilderRequestRequestTypeDef = TypedDict(
-    "DeleteAppBlockBuilderRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 DeleteAppBlockRequestRequestTypeDef = TypedDict(
     "DeleteAppBlockRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -750,35 +640,14 @@
     "DeleteUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 
-DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef = TypedDict(
-    "DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef",
-    {
-        "AppBlockArn": str,
-        "AppBlockBuilderName": str,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-DescribeAppBlockBuildersRequestRequestTypeDef = TypedDict(
-    "DescribeAppBlockBuildersRequestRequestTypeDef",
-    {
-        "Names": Sequence[str],
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 DescribeAppBlocksRequestRequestTypeDef = TypedDict(
     "DescribeAppBlocksRequestRequestTypeDef",
     {
         "Arns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -1020,22 +889,14 @@
     "DisableUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 
-DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef = TypedDict(
-    "DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef",
-    {
-        "AppBlockArn": str,
-        "AppBlockBuilderName": str,
-    },
-)
-
 DisassociateApplicationFleetRequestRequestTypeDef = TypedDict(
     "DisassociateApplicationFleetRequestRequestTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
     },
 )
@@ -1102,14 +963,24 @@
     {
         "EniPrivateIpAddress": str,
         "EniId": str,
     },
     total=False,
 )
 
+ResourceErrorTypeDef = TypedDict(
+    "ResourceErrorTypeDef",
+    {
+        "ErrorCode": FleetErrorCodeType,
+        "ErrorMessage": str,
+        "ErrorTimestamp": datetime,
+    },
+    total=False,
+)
+
 ImagePermissionsTypeDef = TypedDict(
     "ImagePermissionsTypeDef",
     {
         "allowFleet": bool,
         "allowImageBuilder": bool,
     },
     total=False,
@@ -1213,21 +1084,14 @@
     {
         "ErrorCode": StackErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-StartAppBlockBuilderRequestRequestTypeDef = TypedDict(
-    "StartAppBlockBuilderRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 StartFleetRequestRequestTypeDef = TypedDict(
     "StartFleetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1248,21 +1112,14 @@
 
 class StartImageBuilderRequestRequestTypeDef(
     _RequiredStartImageBuilderRequestRequestTypeDef, _OptionalStartImageBuilderRequestRequestTypeDef
 ):
     pass
 
 
-StopAppBlockBuilderRequestRequestTypeDef = TypedDict(
-    "StopAppBlockBuilderRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 StopFleetRequestRequestTypeDef = TypedDict(
     "StopFleetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1285,105 +1142,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredAppBlockBuilderTypeDef = TypedDict(
-    "_RequiredAppBlockBuilderTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "Platform": Literal["WINDOWS_SERVER_2019"],
-        "InstanceType": str,
-        "VpcConfig": VpcConfigTypeDef,
-        "State": AppBlockBuilderStateType,
-    },
-)
-_OptionalAppBlockBuilderTypeDef = TypedDict(
-    "_OptionalAppBlockBuilderTypeDef",
-    {
-        "DisplayName": str,
-        "Description": str,
-        "EnableDefaultInternetAccess": bool,
-        "IamRoleArn": str,
-        "CreatedTime": datetime,
-        "AppBlockBuilderErrors": List[ResourceErrorTypeDef],
-        "StateChangeReason": AppBlockBuilderStateChangeReasonTypeDef,
-        "AccessEndpoints": List[AccessEndpointTypeDef],
-    },
-    total=False,
-)
-
-
-class AppBlockBuilderTypeDef(_RequiredAppBlockBuilderTypeDef, _OptionalAppBlockBuilderTypeDef):
-    pass
-
-
-_RequiredCreateAppBlockBuilderRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppBlockBuilderRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Platform": Literal["WINDOWS_SERVER_2019"],
-        "InstanceType": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-)
-_OptionalCreateAppBlockBuilderRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppBlockBuilderRequestRequestTypeDef",
-    {
-        "Description": str,
-        "DisplayName": str,
-        "Tags": Mapping[str, str],
-        "EnableDefaultInternetAccess": bool,
-        "IamRoleArn": str,
-        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateAppBlockBuilderRequestRequestTypeDef(
-    _RequiredCreateAppBlockBuilderRequestRequestTypeDef,
-    _OptionalCreateAppBlockBuilderRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateAppBlockBuilderRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppBlockBuilderRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateAppBlockBuilderRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppBlockBuilderRequestRequestTypeDef",
-    {
-        "Description": str,
-        "DisplayName": str,
-        "Platform": PlatformTypeType,
-        "InstanceType": str,
-        "VpcConfig": VpcConfigTypeDef,
-        "EnableDefaultInternetAccess": bool,
-        "IamRoleArn": str,
-        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
-        "AttributesToDelete": Sequence[AppBlockBuilderAttributeType],
-    },
-    total=False,
-)
-
-
-class UpdateAppBlockBuilderRequestRequestTypeDef(
-    _RequiredUpdateAppBlockBuilderRequestRequestTypeDef,
-    _OptionalUpdateAppBlockBuilderRequestRequestTypeDef,
-):
-    pass
-
-
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "Name": str,
         "DisplayName": str,
         "IconURL": str,
         "LaunchPath": str,
@@ -1477,22 +1243,14 @@
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
 
-AssociateAppBlockBuilderAppBlockResultTypeDef = TypedDict(
-    "AssociateAppBlockBuilderAppBlockResultTypeDef",
-    {
-        "AppBlockBuilderAppBlockAssociation": AppBlockBuilderAppBlockAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AssociateApplicationFleetResultTypeDef = TypedDict(
     "AssociateApplicationFleetResultTypeDef",
     {
         "ApplicationFleetAssociation": ApplicationFleetAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1501,23 +1259,14 @@
     "CopyImageResponseTypeDef",
     {
         "DestinationImageName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAppBlockBuilderStreamingURLResultTypeDef = TypedDict(
-    "CreateAppBlockBuilderStreamingURLResultTypeDef",
-    {
-        "StreamingURL": str,
-        "Expires": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateImageBuilderStreamingURLResultTypeDef = TypedDict(
     "CreateImageBuilderStreamingURLResultTypeDef",
     {
         "StreamingURL": str,
         "Expires": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1537,23 +1286,14 @@
     {
         "S3BucketName": str,
         "Schedule": Literal["DAILY"],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef = TypedDict(
-    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
-    {
-        "AppBlockBuilderAppBlockAssociations": List[AppBlockBuilderAppBlockAssociationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeApplicationFleetAssociationsResultTypeDef = TypedDict(
     "DescribeApplicationFleetAssociationsResultTypeDef",
     {
         "ApplicationFleetAssociations": List[ApplicationFleetAssociationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2148,14 +1888,41 @@
 )
 
 
 class FleetTypeDef(_RequiredFleetTypeDef, _OptionalFleetTypeDef):
     pass
 
 
+_RequiredSessionTypeDef = TypedDict(
+    "_RequiredSessionTypeDef",
+    {
+        "Id": str,
+        "UserId": str,
+        "StackName": str,
+        "FleetName": str,
+        "State": SessionStateType,
+    },
+)
+_OptionalSessionTypeDef = TypedDict(
+    "_OptionalSessionTypeDef",
+    {
+        "ConnectionState": SessionConnectionStateType,
+        "StartTime": datetime,
+        "MaxExpirationTime": datetime,
+        "AuthenticationType": AuthenticationTypeType,
+        "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
+    pass
+
+
 _RequiredImageBuilderTypeDef = TypedDict(
     "_RequiredImageBuilderTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalImageBuilderTypeDef = TypedDict(
@@ -2183,41 +1950,14 @@
 )
 
 
 class ImageBuilderTypeDef(_RequiredImageBuilderTypeDef, _OptionalImageBuilderTypeDef):
     pass
 
 
-_RequiredSessionTypeDef = TypedDict(
-    "_RequiredSessionTypeDef",
-    {
-        "Id": str,
-        "UserId": str,
-        "StackName": str,
-        "FleetName": str,
-        "State": SessionStateType,
-    },
-)
-_OptionalSessionTypeDef = TypedDict(
-    "_OptionalSessionTypeDef",
-    {
-        "ConnectionState": SessionConnectionStateType,
-        "StartTime": datetime,
-        "MaxExpirationTime": datetime,
-        "AuthenticationType": AuthenticationTypeType,
-        "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
-    pass
-
-
 SharedImagePermissionsTypeDef = TypedDict(
     "SharedImagePermissionsTypeDef",
     {
         "sharedAccountId": str,
         "imagePermissions": ImagePermissionsTypeDef,
     },
 )
@@ -2269,55 +2009,14 @@
 )
 
 
 class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
     pass
 
 
-CreateAppBlockBuilderResultTypeDef = TypedDict(
-    "CreateAppBlockBuilderResultTypeDef",
-    {
-        "AppBlockBuilder": AppBlockBuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAppBlockBuildersResultTypeDef = TypedDict(
-    "DescribeAppBlockBuildersResultTypeDef",
-    {
-        "AppBlockBuilders": List[AppBlockBuilderTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartAppBlockBuilderResultTypeDef = TypedDict(
-    "StartAppBlockBuilderResultTypeDef",
-    {
-        "AppBlockBuilder": AppBlockBuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopAppBlockBuilderResultTypeDef = TypedDict(
-    "StopAppBlockBuilderResultTypeDef",
-    {
-        "AppBlockBuilder": AppBlockBuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAppBlockBuilderResultTypeDef = TypedDict(
-    "UpdateAppBlockBuilderResultTypeDef",
-    {
-        "AppBlockBuilder": AppBlockBuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateApplicationResultTypeDef = TypedDict(
     "CreateApplicationResultTypeDef",
     {
         "Application": ApplicationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2374,53 +2073,47 @@
 )
 
 _RequiredAppBlockTypeDef = TypedDict(
     "_RequiredAppBlockTypeDef",
     {
         "Name": str,
         "Arn": str,
+        "SetupScriptDetails": ScriptDetailsTypeDef,
     },
 )
 _OptionalAppBlockTypeDef = TypedDict(
     "_OptionalAppBlockTypeDef",
     {
         "Description": str,
         "DisplayName": str,
         "SourceS3Location": S3LocationTypeDef,
-        "SetupScriptDetails": ScriptDetailsTypeDef,
         "CreatedTime": datetime,
-        "PostSetupScriptDetails": ScriptDetailsTypeDef,
-        "PackagingType": PackagingTypeType,
-        "State": AppBlockStateType,
-        "AppBlockErrors": List[ErrorDetailsTypeDef],
     },
     total=False,
 )
 
 
 class AppBlockTypeDef(_RequiredAppBlockTypeDef, _OptionalAppBlockTypeDef):
     pass
 
 
 _RequiredCreateAppBlockRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppBlockRequestRequestTypeDef",
     {
         "Name": str,
         "SourceS3Location": S3LocationTypeDef,
+        "SetupScriptDetails": ScriptDetailsTypeDef,
     },
 )
 _OptionalCreateAppBlockRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAppBlockRequestRequestTypeDef",
     {
         "Description": str,
         "DisplayName": str,
-        "SetupScriptDetails": ScriptDetailsTypeDef,
         "Tags": Mapping[str, str],
-        "PostSetupScriptDetails": ScriptDetailsTypeDef,
-        "PackagingType": PackagingTypeType,
     },
     total=False,
 )
 
 
 class CreateAppBlockRequestRequestTypeDef(
     _RequiredCreateAppBlockRequestRequestTypeDef, _OptionalCreateAppBlockRequestRequestTypeDef
@@ -2515,14 +2208,23 @@
     "UpdateFleetResultTypeDef",
     {
         "Fleet": FleetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeSessionsResultTypeDef = TypedDict(
+    "DescribeSessionsResultTypeDef",
+    {
+        "Sessions": List[SessionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateImageBuilderResultTypeDef = TypedDict(
     "CreateImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2556,23 +2258,14 @@
     "StopImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeSessionsResultTypeDef = TypedDict(
-    "DescribeSessionsResultTypeDef",
-    {
-        "Sessions": List[SessionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeImagePermissionsResultTypeDef = TypedDict(
     "DescribeImagePermissionsResultTypeDef",
     {
         "Name": str,
         "SharedImagePermissionsList": List[SharedImagePermissionsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/type_defs.pyi` & `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -13,31 +13,27 @@
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ActionType,
-    AppBlockBuilderAttributeType,
-    AppBlockBuilderStateType,
-    AppBlockStateType,
     ApplicationAttributeType,
     AppVisibilityType,
     AuthenticationTypeType,
     CertificateBasedAuthStatusType,
     FleetAttributeType,
     FleetErrorCodeType,
     FleetStateType,
     FleetTypeType,
     ImageBuilderStateChangeReasonCodeType,
     ImageBuilderStateType,
     ImageStateChangeReasonCodeType,
     ImageStateType,
     MessageActionType,
-    PackagingTypeType,
     PermissionType,
     PlatformTypeType,
     PreferredProtocolType,
     SessionConnectionStateType,
     SessionStateType,
     StackAttributeType,
     StackErrorCodeType,
@@ -55,57 +51,48 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessEndpointTypeDef",
-    "AppBlockBuilderAppBlockAssociationTypeDef",
-    "AppBlockBuilderStateChangeReasonTypeDef",
-    "ResourceErrorTypeDef",
-    "VpcConfigTypeDef",
-    "ErrorDetailsTypeDef",
     "S3LocationTypeDef",
     "ApplicationFleetAssociationTypeDef",
     "ApplicationSettingsResponseTypeDef",
     "ApplicationSettingsTypeDef",
-    "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AssociateApplicationFleetRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateApplicationToEntitlementRequestRequestTypeDef",
     "AssociateFleetRequestRequestTypeDef",
     "UserStackAssociationTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
     "ComputeCapacityStatusTypeDef",
     "ComputeCapacityTypeDef",
     "CopyImageRequestRequestTypeDef",
-    "CreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
     "ServiceAccountCredentialsTypeDef",
     "EntitlementAttributeTypeDef",
     "DomainJoinInfoTypeDef",
+    "VpcConfigTypeDef",
     "CreateImageBuilderStreamingURLRequestRequestTypeDef",
     "StorageConnectorTypeDef",
     "StreamingExperienceSettingsTypeDef",
     "UserSettingTypeDef",
     "CreateStreamingURLRequestRequestTypeDef",
     "CreateUpdatedImageRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "DeleteAppBlockBuilderRequestRequestTypeDef",
     "DeleteAppBlockRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteDirectoryConfigRequestRequestTypeDef",
     "DeleteEntitlementRequestRequestTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteImageBuilderRequestRequestTypeDef",
     "DeleteImagePermissionsRequestRequestTypeDef",
     "DeleteImageRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
-    "DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef",
-    "DescribeAppBlockBuildersRequestRequestTypeDef",
     "DescribeAppBlocksRequestRequestTypeDef",
     "DescribeApplicationFleetAssociationsRequestRequestTypeDef",
     "DescribeApplicationsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeDirectoryConfigsRequestRequestTypeDef",
     "DescribeEntitlementsRequestRequestTypeDef",
     "WaiterConfigTypeDef",
@@ -116,55 +103,47 @@
     "DescribeSessionsRequestRequestTypeDef",
     "DescribeStacksRequestRequestTypeDef",
     "DescribeUsageReportSubscriptionsRequestRequestTypeDef",
     "DescribeUserStackAssociationsRequestRequestTypeDef",
     "DescribeUsersRequestRequestTypeDef",
     "UserTypeDef",
     "DisableUserRequestRequestTypeDef",
-    "DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     "DisassociateApplicationFleetRequestRequestTypeDef",
     "DisassociateApplicationFromEntitlementRequestRequestTypeDef",
     "DisassociateFleetRequestRequestTypeDef",
     "EnableUserRequestRequestTypeDef",
     "EntitledApplicationTypeDef",
     "ExpireSessionRequestRequestTypeDef",
     "FleetErrorTypeDef",
     "ImageBuilderStateChangeReasonTypeDef",
     "NetworkAccessConfigurationTypeDef",
+    "ResourceErrorTypeDef",
     "ImagePermissionsTypeDef",
     "ImageStateChangeReasonTypeDef",
     "LastReportGenerationExecutionErrorTypeDef",
     "ListAssociatedFleetsRequestRequestTypeDef",
     "ListAssociatedStacksRequestRequestTypeDef",
     "ListEntitledApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "StackErrorTypeDef",
-    "StartAppBlockBuilderRequestRequestTypeDef",
     "StartFleetRequestRequestTypeDef",
     "StartImageBuilderRequestRequestTypeDef",
-    "StopAppBlockBuilderRequestRequestTypeDef",
     "StopFleetRequestRequestTypeDef",
     "StopImageBuilderRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AppBlockBuilderTypeDef",
-    "CreateAppBlockBuilderRequestRequestTypeDef",
-    "UpdateAppBlockBuilderRequestRequestTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "ScriptDetailsTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "AssociateAppBlockBuilderAppBlockResultTypeDef",
     "AssociateApplicationFleetResultTypeDef",
     "CopyImageResponseTypeDef",
-    "CreateAppBlockBuilderStreamingURLResultTypeDef",
     "CreateImageBuilderStreamingURLResultTypeDef",
     "CreateStreamingURLResultTypeDef",
     "CreateUsageReportSubscriptionResultTypeDef",
-    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
     "DescribeApplicationFleetAssociationsResultTypeDef",
     "ListAssociatedFleetsResultTypeDef",
     "ListAssociatedStacksResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "BatchAssociateUserStackRequestRequestTypeDef",
     "BatchDisassociateUserStackRequestRequestTypeDef",
     "DescribeUserStackAssociationsResultTypeDef",
@@ -191,25 +170,20 @@
     "ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
     "ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
     "DescribeFleetsRequestFleetStartedWaitTypeDef",
     "DescribeFleetsRequestFleetStoppedWaitTypeDef",
     "DescribeUsersResultTypeDef",
     "ListEntitledApplicationsResultTypeDef",
     "FleetTypeDef",
-    "ImageBuilderTypeDef",
     "SessionTypeDef",
+    "ImageBuilderTypeDef",
     "SharedImagePermissionsTypeDef",
     "UpdateImagePermissionsRequestRequestTypeDef",
     "UsageReportSubscriptionTypeDef",
     "StackTypeDef",
-    "CreateAppBlockBuilderResultTypeDef",
-    "DescribeAppBlockBuildersResultTypeDef",
-    "StartAppBlockBuilderResultTypeDef",
-    "StopAppBlockBuilderResultTypeDef",
-    "UpdateAppBlockBuilderResultTypeDef",
     "CreateApplicationResultTypeDef",
     "DescribeApplicationsResultTypeDef",
     "ImageTypeDef",
     "UpdateApplicationResultTypeDef",
     "AppBlockTypeDef",
     "CreateAppBlockRequestRequestTypeDef",
     "BatchAssociateUserStackResultTypeDef",
@@ -219,20 +193,20 @@
     "UpdateDirectoryConfigResultTypeDef",
     "CreateEntitlementResultTypeDef",
     "DescribeEntitlementsResultTypeDef",
     "UpdateEntitlementResultTypeDef",
     "CreateFleetResultTypeDef",
     "DescribeFleetsResultTypeDef",
     "UpdateFleetResultTypeDef",
+    "DescribeSessionsResultTypeDef",
     "CreateImageBuilderResultTypeDef",
     "DeleteImageBuilderResultTypeDef",
     "DescribeImageBuildersResultTypeDef",
     "StartImageBuilderResultTypeDef",
     "StopImageBuilderResultTypeDef",
-    "DescribeSessionsResultTypeDef",
     "DescribeImagePermissionsResultTypeDef",
     "DescribeUsageReportSubscriptionsResultTypeDef",
     "CreateStackResultTypeDef",
     "DescribeStacksResultTypeDef",
     "UpdateStackResultTypeDef",
     "CreateUpdatedImageResultTypeDef",
     "DeleteImageResultTypeDef",
@@ -254,76 +228,22 @@
     },
     total=False,
 )
 
 class AccessEndpointTypeDef(_RequiredAccessEndpointTypeDef, _OptionalAccessEndpointTypeDef):
     pass
 
-AppBlockBuilderAppBlockAssociationTypeDef = TypedDict(
-    "AppBlockBuilderAppBlockAssociationTypeDef",
-    {
-        "AppBlockArn": str,
-        "AppBlockBuilderName": str,
-    },
-)
-
-AppBlockBuilderStateChangeReasonTypeDef = TypedDict(
-    "AppBlockBuilderStateChangeReasonTypeDef",
-    {
-        "Code": Literal["INTERNAL_ERROR"],
-        "Message": str,
-    },
-    total=False,
-)
-
-ResourceErrorTypeDef = TypedDict(
-    "ResourceErrorTypeDef",
-    {
-        "ErrorCode": FleetErrorCodeType,
-        "ErrorMessage": str,
-        "ErrorTimestamp": datetime,
-    },
-    total=False,
-)
-
-VpcConfigTypeDef = TypedDict(
-    "VpcConfigTypeDef",
-    {
-        "SubnetIds": Sequence[str],
-        "SecurityGroupIds": Sequence[str],
-    },
-    total=False,
-)
-
-ErrorDetailsTypeDef = TypedDict(
-    "ErrorDetailsTypeDef",
-    {
-        "ErrorCode": str,
-        "ErrorMessage": str,
-    },
-    total=False,
-)
-
-_RequiredS3LocationTypeDef = TypedDict(
-    "_RequiredS3LocationTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
         "S3Bucket": str,
-    },
-)
-_OptionalS3LocationTypeDef = TypedDict(
-    "_OptionalS3LocationTypeDef",
-    {
         "S3Key": str,
     },
-    total=False,
 )
 
-class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
-    pass
-
 ApplicationFleetAssociationTypeDef = TypedDict(
     "ApplicationFleetAssociationTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
     },
 )
@@ -353,41 +273,33 @@
 )
 
 class ApplicationSettingsTypeDef(
     _RequiredApplicationSettingsTypeDef, _OptionalApplicationSettingsTypeDef
 ):
     pass
 
-AssociateAppBlockBuilderAppBlockRequestRequestTypeDef = TypedDict(
-    "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
+AssociateApplicationFleetRequestRequestTypeDef = TypedDict(
+    "AssociateApplicationFleetRequestRequestTypeDef",
     {
-        "AppBlockArn": str,
-        "AppBlockBuilderName": str,
+        "FleetName": str,
+        "ApplicationArn": str,
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-AssociateApplicationFleetRequestRequestTypeDef = TypedDict(
-    "AssociateApplicationFleetRequestRequestTypeDef",
-    {
-        "FleetName": str,
-        "ApplicationArn": str,
-    },
-)
-
 AssociateApplicationToEntitlementRequestRequestTypeDef = TypedDict(
     "AssociateApplicationToEntitlementRequestRequestTypeDef",
     {
         "StackName": str,
         "EntitlementName": str,
         "ApplicationIdentifier": str,
     },
@@ -476,34 +388,14 @@
 )
 
 class CopyImageRequestRequestTypeDef(
     _RequiredCopyImageRequestRequestTypeDef, _OptionalCopyImageRequestRequestTypeDef
 ):
     pass
 
-_RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
-    {
-        "AppBlockBuilderName": str,
-    },
-)
-_OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
-    {
-        "Validity": int,
-    },
-    total=False,
-)
-
-class CreateAppBlockBuilderStreamingURLRequestRequestTypeDef(
-    _RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
-    _OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
-):
-    pass
-
 ServiceAccountCredentialsTypeDef = TypedDict(
     "ServiceAccountCredentialsTypeDef",
     {
         "AccountName": str,
         "AccountPassword": str,
     },
 )
@@ -521,14 +413,23 @@
     {
         "DirectoryName": str,
         "OrganizationalUnitDistinguishedName": str,
     },
     total=False,
 )
 
+VpcConfigTypeDef = TypedDict(
+    "VpcConfigTypeDef",
+    {
+        "SubnetIds": Sequence[str],
+        "SecurityGroupIds": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef = TypedDict(
@@ -645,21 +546,14 @@
 )
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
-DeleteAppBlockBuilderRequestRequestTypeDef = TypedDict(
-    "DeleteAppBlockBuilderRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 DeleteAppBlockRequestRequestTypeDef = TypedDict(
     "DeleteAppBlockRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -725,35 +619,14 @@
     "DeleteUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 
-DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef = TypedDict(
-    "DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef",
-    {
-        "AppBlockArn": str,
-        "AppBlockBuilderName": str,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-DescribeAppBlockBuildersRequestRequestTypeDef = TypedDict(
-    "DescribeAppBlockBuildersRequestRequestTypeDef",
-    {
-        "Names": Sequence[str],
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 DescribeAppBlocksRequestRequestTypeDef = TypedDict(
     "DescribeAppBlocksRequestRequestTypeDef",
     {
         "Arns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -985,22 +858,14 @@
     "DisableUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 
-DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef = TypedDict(
-    "DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef",
-    {
-        "AppBlockArn": str,
-        "AppBlockBuilderName": str,
-    },
-)
-
 DisassociateApplicationFleetRequestRequestTypeDef = TypedDict(
     "DisassociateApplicationFleetRequestRequestTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
     },
 )
@@ -1067,14 +932,24 @@
     {
         "EniPrivateIpAddress": str,
         "EniId": str,
     },
     total=False,
 )
 
+ResourceErrorTypeDef = TypedDict(
+    "ResourceErrorTypeDef",
+    {
+        "ErrorCode": FleetErrorCodeType,
+        "ErrorMessage": str,
+        "ErrorTimestamp": datetime,
+    },
+    total=False,
+)
+
 ImagePermissionsTypeDef = TypedDict(
     "ImagePermissionsTypeDef",
     {
         "allowFleet": bool,
         "allowImageBuilder": bool,
     },
     total=False,
@@ -1172,21 +1047,14 @@
     {
         "ErrorCode": StackErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-StartAppBlockBuilderRequestRequestTypeDef = TypedDict(
-    "StartAppBlockBuilderRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 StartFleetRequestRequestTypeDef = TypedDict(
     "StartFleetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1205,21 +1073,14 @@
 )
 
 class StartImageBuilderRequestRequestTypeDef(
     _RequiredStartImageBuilderRequestRequestTypeDef, _OptionalStartImageBuilderRequestRequestTypeDef
 ):
     pass
 
-StopAppBlockBuilderRequestRequestTypeDef = TypedDict(
-    "StopAppBlockBuilderRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 StopFleetRequestRequestTypeDef = TypedDict(
     "StopFleetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1242,99 +1103,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredAppBlockBuilderTypeDef = TypedDict(
-    "_RequiredAppBlockBuilderTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "Platform": Literal["WINDOWS_SERVER_2019"],
-        "InstanceType": str,
-        "VpcConfig": VpcConfigTypeDef,
-        "State": AppBlockBuilderStateType,
-    },
-)
-_OptionalAppBlockBuilderTypeDef = TypedDict(
-    "_OptionalAppBlockBuilderTypeDef",
-    {
-        "DisplayName": str,
-        "Description": str,
-        "EnableDefaultInternetAccess": bool,
-        "IamRoleArn": str,
-        "CreatedTime": datetime,
-        "AppBlockBuilderErrors": List[ResourceErrorTypeDef],
-        "StateChangeReason": AppBlockBuilderStateChangeReasonTypeDef,
-        "AccessEndpoints": List[AccessEndpointTypeDef],
-    },
-    total=False,
-)
-
-class AppBlockBuilderTypeDef(_RequiredAppBlockBuilderTypeDef, _OptionalAppBlockBuilderTypeDef):
-    pass
-
-_RequiredCreateAppBlockBuilderRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppBlockBuilderRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Platform": Literal["WINDOWS_SERVER_2019"],
-        "InstanceType": str,
-        "VpcConfig": VpcConfigTypeDef,
-    },
-)
-_OptionalCreateAppBlockBuilderRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppBlockBuilderRequestRequestTypeDef",
-    {
-        "Description": str,
-        "DisplayName": str,
-        "Tags": Mapping[str, str],
-        "EnableDefaultInternetAccess": bool,
-        "IamRoleArn": str,
-        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
-    },
-    total=False,
-)
-
-class CreateAppBlockBuilderRequestRequestTypeDef(
-    _RequiredCreateAppBlockBuilderRequestRequestTypeDef,
-    _OptionalCreateAppBlockBuilderRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateAppBlockBuilderRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppBlockBuilderRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateAppBlockBuilderRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppBlockBuilderRequestRequestTypeDef",
-    {
-        "Description": str,
-        "DisplayName": str,
-        "Platform": PlatformTypeType,
-        "InstanceType": str,
-        "VpcConfig": VpcConfigTypeDef,
-        "EnableDefaultInternetAccess": bool,
-        "IamRoleArn": str,
-        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
-        "AttributesToDelete": Sequence[AppBlockBuilderAttributeType],
-    },
-    total=False,
-)
-
-class UpdateAppBlockBuilderRequestRequestTypeDef(
-    _RequiredUpdateAppBlockBuilderRequestRequestTypeDef,
-    _OptionalUpdateAppBlockBuilderRequestRequestTypeDef,
-):
-    pass
-
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "Name": str,
         "DisplayName": str,
         "IconURL": str,
         "LaunchPath": str,
@@ -1422,22 +1198,14 @@
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-AssociateAppBlockBuilderAppBlockResultTypeDef = TypedDict(
-    "AssociateAppBlockBuilderAppBlockResultTypeDef",
-    {
-        "AppBlockBuilderAppBlockAssociation": AppBlockBuilderAppBlockAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AssociateApplicationFleetResultTypeDef = TypedDict(
     "AssociateApplicationFleetResultTypeDef",
     {
         "ApplicationFleetAssociation": ApplicationFleetAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1446,23 +1214,14 @@
     "CopyImageResponseTypeDef",
     {
         "DestinationImageName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAppBlockBuilderStreamingURLResultTypeDef = TypedDict(
-    "CreateAppBlockBuilderStreamingURLResultTypeDef",
-    {
-        "StreamingURL": str,
-        "Expires": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateImageBuilderStreamingURLResultTypeDef = TypedDict(
     "CreateImageBuilderStreamingURLResultTypeDef",
     {
         "StreamingURL": str,
         "Expires": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1482,23 +1241,14 @@
     {
         "S3BucketName": str,
         "Schedule": Literal["DAILY"],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef = TypedDict(
-    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
-    {
-        "AppBlockBuilderAppBlockAssociations": List[AppBlockBuilderAppBlockAssociationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeApplicationFleetAssociationsResultTypeDef = TypedDict(
     "DescribeApplicationFleetAssociationsResultTypeDef",
     {
         "ApplicationFleetAssociations": List[ApplicationFleetAssociationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2063,14 +1813,39 @@
     },
     total=False,
 )
 
 class FleetTypeDef(_RequiredFleetTypeDef, _OptionalFleetTypeDef):
     pass
 
+_RequiredSessionTypeDef = TypedDict(
+    "_RequiredSessionTypeDef",
+    {
+        "Id": str,
+        "UserId": str,
+        "StackName": str,
+        "FleetName": str,
+        "State": SessionStateType,
+    },
+)
+_OptionalSessionTypeDef = TypedDict(
+    "_OptionalSessionTypeDef",
+    {
+        "ConnectionState": SessionConnectionStateType,
+        "StartTime": datetime,
+        "MaxExpirationTime": datetime,
+        "AuthenticationType": AuthenticationTypeType,
+        "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
+    pass
+
 _RequiredImageBuilderTypeDef = TypedDict(
     "_RequiredImageBuilderTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalImageBuilderTypeDef = TypedDict(
@@ -2096,39 +1871,14 @@
     },
     total=False,
 )
 
 class ImageBuilderTypeDef(_RequiredImageBuilderTypeDef, _OptionalImageBuilderTypeDef):
     pass
 
-_RequiredSessionTypeDef = TypedDict(
-    "_RequiredSessionTypeDef",
-    {
-        "Id": str,
-        "UserId": str,
-        "StackName": str,
-        "FleetName": str,
-        "State": SessionStateType,
-    },
-)
-_OptionalSessionTypeDef = TypedDict(
-    "_OptionalSessionTypeDef",
-    {
-        "ConnectionState": SessionConnectionStateType,
-        "StartTime": datetime,
-        "MaxExpirationTime": datetime,
-        "AuthenticationType": AuthenticationTypeType,
-        "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
-    pass
-
 SharedImagePermissionsTypeDef = TypedDict(
     "SharedImagePermissionsTypeDef",
     {
         "sharedAccountId": str,
         "imagePermissions": ImagePermissionsTypeDef,
     },
 )
@@ -2178,55 +1928,14 @@
     },
     total=False,
 )
 
 class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
     pass
 
-CreateAppBlockBuilderResultTypeDef = TypedDict(
-    "CreateAppBlockBuilderResultTypeDef",
-    {
-        "AppBlockBuilder": AppBlockBuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAppBlockBuildersResultTypeDef = TypedDict(
-    "DescribeAppBlockBuildersResultTypeDef",
-    {
-        "AppBlockBuilders": List[AppBlockBuilderTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartAppBlockBuilderResultTypeDef = TypedDict(
-    "StartAppBlockBuilderResultTypeDef",
-    {
-        "AppBlockBuilder": AppBlockBuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopAppBlockBuilderResultTypeDef = TypedDict(
-    "StopAppBlockBuilderResultTypeDef",
-    {
-        "AppBlockBuilder": AppBlockBuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAppBlockBuilderResultTypeDef = TypedDict(
-    "UpdateAppBlockBuilderResultTypeDef",
-    {
-        "AppBlockBuilder": AppBlockBuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateApplicationResultTypeDef = TypedDict(
     "CreateApplicationResultTypeDef",
     {
         "Application": ApplicationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2281,51 +1990,45 @@
 )
 
 _RequiredAppBlockTypeDef = TypedDict(
     "_RequiredAppBlockTypeDef",
     {
         "Name": str,
         "Arn": str,
+        "SetupScriptDetails": ScriptDetailsTypeDef,
     },
 )
 _OptionalAppBlockTypeDef = TypedDict(
     "_OptionalAppBlockTypeDef",
     {
         "Description": str,
         "DisplayName": str,
         "SourceS3Location": S3LocationTypeDef,
-        "SetupScriptDetails": ScriptDetailsTypeDef,
         "CreatedTime": datetime,
-        "PostSetupScriptDetails": ScriptDetailsTypeDef,
-        "PackagingType": PackagingTypeType,
-        "State": AppBlockStateType,
-        "AppBlockErrors": List[ErrorDetailsTypeDef],
     },
     total=False,
 )
 
 class AppBlockTypeDef(_RequiredAppBlockTypeDef, _OptionalAppBlockTypeDef):
     pass
 
 _RequiredCreateAppBlockRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppBlockRequestRequestTypeDef",
     {
         "Name": str,
         "SourceS3Location": S3LocationTypeDef,
+        "SetupScriptDetails": ScriptDetailsTypeDef,
     },
 )
 _OptionalCreateAppBlockRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAppBlockRequestRequestTypeDef",
     {
         "Description": str,
         "DisplayName": str,
-        "SetupScriptDetails": ScriptDetailsTypeDef,
         "Tags": Mapping[str, str],
-        "PostSetupScriptDetails": ScriptDetailsTypeDef,
-        "PackagingType": PackagingTypeType,
     },
     total=False,
 )
 
 class CreateAppBlockRequestRequestTypeDef(
     _RequiredCreateAppBlockRequestRequestTypeDef, _OptionalCreateAppBlockRequestRequestTypeDef
 ):
@@ -2418,14 +2121,23 @@
     "UpdateFleetResultTypeDef",
     {
         "Fleet": FleetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeSessionsResultTypeDef = TypedDict(
+    "DescribeSessionsResultTypeDef",
+    {
+        "Sessions": List[SessionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateImageBuilderResultTypeDef = TypedDict(
     "CreateImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2459,23 +2171,14 @@
     "StopImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeSessionsResultTypeDef = TypedDict(
-    "DescribeSessionsResultTypeDef",
-    {
-        "Sessions": List[SessionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeImagePermissionsResultTypeDef = TypedDict(
     "DescribeImagePermissionsResultTypeDef",
     {
         "Name": str,
         "SharedImagePermissionsList": List[SharedImagePermissionsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/waiter.py` & `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.26.164/mypy_boto3_appstream/waiter.pyi` & `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.26.164/mypy_boto3_appstream.egg-info/PKG-INFO` & `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appstream
-Version: 1.26.164
-Summary: Type annotations for boto3.AppStream 1.26.164 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.59
+Summary: Type annotations for boto3.AppStream 1.26.59 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-appstream"></a>
 
 # mypy-boto3-appstream
 
 [![PyPI - mypy-boto3-appstream](https://img.shields.io/pypi/v/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appstream?color=blue)](https://pypistats.org/packages/mypy-boto3-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppStream 1.26.164](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[boto3.AppStream 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,19 +349,14 @@
 `mypy_boto3_appstream.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_appstream.literals import (
     AccessEndpointTypeType,
     ActionType,
-    AppBlockBuilderAttributeType,
-    AppBlockBuilderPlatformTypeType,
-    AppBlockBuilderStateChangeReasonCodeType,
-    AppBlockBuilderStateType,
-    AppBlockStateType,
     AppVisibilityType,
     ApplicationAttributeType,
     AuthenticationTypeType,
     CertificateBasedAuthStatusType,
     DescribeDirectoryConfigsPaginatorName,
     DescribeFleetsPaginatorName,
     DescribeImageBuildersPaginatorName,
@@ -379,15 +374,14 @@
     ImageBuilderStateChangeReasonCodeType,
     ImageBuilderStateType,
     ImageStateChangeReasonCodeType,
     ImageStateType,
     ListAssociatedFleetsPaginatorName,
     ListAssociatedStacksPaginatorName,
     MessageActionType,
-    PackagingTypeType,
     PermissionType,
     PlatformTypeType,
     PreferredProtocolType,
     SessionConnectionStateType,
     SessionStateType,
     StackAttributeType,
     StackErrorCodeType,
@@ -416,57 +410,48 @@
 
 `mypy_boto3_appstream.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appstream.type_defs import (
     AccessEndpointTypeDef,
-    AppBlockBuilderAppBlockAssociationTypeDef,
-    AppBlockBuilderStateChangeReasonTypeDef,
-    ResourceErrorTypeDef,
-    VpcConfigTypeDef,
-    ErrorDetailsTypeDef,
     S3LocationTypeDef,
     ApplicationFleetAssociationTypeDef,
     ApplicationSettingsResponseTypeDef,
     ApplicationSettingsTypeDef,
-    AssociateAppBlockBuilderAppBlockRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AssociateApplicationFleetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AssociateApplicationToEntitlementRequestRequestTypeDef,
     AssociateFleetRequestRequestTypeDef,
     UserStackAssociationTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityStatusTypeDef,
     ComputeCapacityTypeDef,
     CopyImageRequestRequestTypeDef,
-    CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
+    VpcConfigTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UserSettingTypeDef,
     CreateStreamingURLRequestRequestTypeDef,
     CreateUpdatedImageRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
-    DeleteAppBlockBuilderRequestRequestTypeDef,
     DeleteAppBlockRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteDirectoryConfigRequestRequestTypeDef,
     DeleteEntitlementRequestRequestTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteImageBuilderRequestRequestTypeDef,
     DeleteImagePermissionsRequestRequestTypeDef,
     DeleteImageRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
-    DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef,
-    DescribeAppBlockBuildersRequestRequestTypeDef,
     DescribeAppBlocksRequestRequestTypeDef,
     DescribeApplicationFleetAssociationsRequestRequestTypeDef,
     DescribeApplicationsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeDirectoryConfigsRequestRequestTypeDef,
     DescribeEntitlementsRequestRequestTypeDef,
     WaiterConfigTypeDef,
@@ -477,55 +462,47 @@
     DescribeSessionsRequestRequestTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeUsageReportSubscriptionsRequestRequestTypeDef,
     DescribeUserStackAssociationsRequestRequestTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UserTypeDef,
     DisableUserRequestRequestTypeDef,
-    DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     DisassociateApplicationFleetRequestRequestTypeDef,
     DisassociateApplicationFromEntitlementRequestRequestTypeDef,
     DisassociateFleetRequestRequestTypeDef,
     EnableUserRequestRequestTypeDef,
     EntitledApplicationTypeDef,
     ExpireSessionRequestRequestTypeDef,
     FleetErrorTypeDef,
     ImageBuilderStateChangeReasonTypeDef,
     NetworkAccessConfigurationTypeDef,
+    ResourceErrorTypeDef,
     ImagePermissionsTypeDef,
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
     ListAssociatedStacksRequestRequestTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     StackErrorTypeDef,
-    StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
-    StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AppBlockBuilderTypeDef,
-    CreateAppBlockBuilderRequestRequestTypeDef,
-    UpdateAppBlockBuilderRequestRequestTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     ScriptDetailsTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    AssociateAppBlockBuilderAppBlockResultTypeDef,
     AssociateApplicationFleetResultTypeDef,
     CopyImageResponseTypeDef,
-    CreateAppBlockBuilderStreamingURLResultTypeDef,
     CreateImageBuilderStreamingURLResultTypeDef,
     CreateStreamingURLResultTypeDef,
     CreateUsageReportSubscriptionResultTypeDef,
-    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
     ListAssociatedFleetsResultTypeDef,
     ListAssociatedStacksResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     BatchAssociateUserStackRequestRequestTypeDef,
     BatchDisassociateUserStackRequestRequestTypeDef,
     DescribeUserStackAssociationsResultTypeDef,
@@ -552,25 +529,20 @@
     ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
     ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
     DescribeFleetsRequestFleetStartedWaitTypeDef,
     DescribeFleetsRequestFleetStoppedWaitTypeDef,
     DescribeUsersResultTypeDef,
     ListEntitledApplicationsResultTypeDef,
     FleetTypeDef,
-    ImageBuilderTypeDef,
     SessionTypeDef,
+    ImageBuilderTypeDef,
     SharedImagePermissionsTypeDef,
     UpdateImagePermissionsRequestRequestTypeDef,
     UsageReportSubscriptionTypeDef,
     StackTypeDef,
-    CreateAppBlockBuilderResultTypeDef,
-    DescribeAppBlockBuildersResultTypeDef,
-    StartAppBlockBuilderResultTypeDef,
-    StopAppBlockBuilderResultTypeDef,
-    UpdateAppBlockBuilderResultTypeDef,
     CreateApplicationResultTypeDef,
     DescribeApplicationsResultTypeDef,
     ImageTypeDef,
     UpdateApplicationResultTypeDef,
     AppBlockTypeDef,
     CreateAppBlockRequestRequestTypeDef,
     BatchAssociateUserStackResultTypeDef,
@@ -580,20 +552,20 @@
     UpdateDirectoryConfigResultTypeDef,
     CreateEntitlementResultTypeDef,
     DescribeEntitlementsResultTypeDef,
     UpdateEntitlementResultTypeDef,
     CreateFleetResultTypeDef,
     DescribeFleetsResultTypeDef,
     UpdateFleetResultTypeDef,
+    DescribeSessionsResultTypeDef,
     CreateImageBuilderResultTypeDef,
     DeleteImageBuilderResultTypeDef,
     DescribeImageBuildersResultTypeDef,
     StartImageBuilderResultTypeDef,
     StopImageBuilderResultTypeDef,
-    DescribeSessionsResultTypeDef,
     DescribeImagePermissionsResultTypeDef,
     DescribeUsageReportSubscriptionsResultTypeDef,
     CreateStackResultTypeDef,
     DescribeStacksResultTypeDef,
     UpdateStackResultTypeDef,
     CreateUpdatedImageResultTypeDef,
     DeleteImageResultTypeDef,
@@ -610,42 +582,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-appstream-1.26.164/mypy_boto3_appstream.egg-info/SOURCES.txt` & `mypy-boto3-appstream-1.26.59/mypy_boto3_appstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.26.164/setup.py` & `mypy-boto3-appstream-1.26.59/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-appstream.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-appstream",
-    version="1.26.164",
+    version="1.26.59",
     packages=["mypy_boto3_appstream"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppStream 1.26.164 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.AppStream 1.26.59 service generated with mypy-boto3-builder"
+        " 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

