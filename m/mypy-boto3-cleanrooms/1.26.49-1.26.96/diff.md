# Comparing `tmp/mypy-boto3-cleanrooms-1.26.49.tar.gz` & `tmp/mypy-boto3-cleanrooms-1.26.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cleanrooms-1.26.49.tar", last modified: Thu Jan 12 20:34:32 2023, max compression
+gzip compressed data, was "mypy-boto3-cleanrooms-1.26.96.tar", last modified: Tue Mar 21 19:19:40 2023, max compression
```

## Comparing `mypy-boto3-cleanrooms-1.26.49.tar` & `mypy-boto3-cleanrooms-1.26.96.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 20:34:32.467100 mypy-boto3-cleanrooms-1.26.49/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-12 20:34:04.000000 mypy-boto3-cleanrooms-1.26.49/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18780 2023-01-12 20:34:32.467100 mypy-boto3-cleanrooms-1.26.49/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-01-12 20:34:04.000000 mypy-boto3-cleanrooms-1.26.49/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 20:34:32.463100 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-01-12 20:34:04.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-01-12 20:34:04.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-12 20:34:04.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28266 2023-01-12 20:34:04.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28218 2023-01-12 20:34:04.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-01-12 20:34:04.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-01-12 20:34:04.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-01-12 20:34:04.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-01-12 20:34:04.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 20:34:04.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39937 2023-01-12 20:34:05.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39886 2023-01-12 20:34:05.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-12 20:34:04.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 20:34:32.467100 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18780 2023-01-12 20:34:32.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-12 20:34:32.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 20:34:32.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 20:34:32.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-12 20:34:32.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-12 20:34:32.000000 mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 20:34:32.467100 mypy-boto3-cleanrooms-1.26.49/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-01-12 20:34:03.000000 mypy-boto3-cleanrooms-1.26.49/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:40.909032 mypy-boto3-cleanrooms-1.26.96/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18936 2023-03-21 19:19:40.909032 mypy-boto3-cleanrooms-1.26.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17430 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:40.909032 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29891 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29840 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-03-21 19:18:33.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41217 2023-03-21 19:18:33.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41164 2023-03-21 19:18:33.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:40.909032 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18936 2023-03-21 19:19:40.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-21 19:19:40.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:19:40.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:19:40.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-21 19:19:40.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-21 19:19:40.000000 mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 19:19:40.909032 mypy-boto3-cleanrooms-1.26.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-21 19:18:32.000000 mypy-boto3-cleanrooms-1.26.96/setup.py
```

### Comparing `mypy-boto3-cleanrooms-1.26.49/LICENSE` & `mypy-boto3-cleanrooms-1.26.96/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.26.49/PKG-INFO` & `mypy-boto3-cleanrooms-1.26.96/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cleanrooms
-Version: 1.26.49
-Summary: Type annotations for boto3.CleanRoomsService 1.26.49 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.96
+Summary: Type annotations for boto3.CleanRoomsService 1.26.96 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cleanrooms?color=blue)](https://pypistats.org/packages/mypy-boto3-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsService 1.26.49](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[boto3.CleanRoomsService 1.26.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cleanrooms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -408,25 +408,29 @@
     MemberSummaryTypeDef,
     ListMembershipsInputRequestTypeDef,
     MembershipSummaryTypeDef,
     ListProtectedQueriesInputRequestTypeDef,
     ProtectedQuerySummaryTypeDef,
     ListSchemasInputRequestTypeDef,
     SchemaSummaryTypeDef,
+    ListTagsForResourceInputRequestTypeDef,
     ProtectedQueryErrorTypeDef,
     ProtectedQueryS3OutputConfigurationTypeDef,
     ProtectedQueryS3OutputTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     ProtectedQueryStatisticsTypeDef,
+    TagResourceInputRequestTypeDef,
+    UntagResourceInputRequestTypeDef,
     UpdateCollaborationInputRequestTypeDef,
     UpdateConfiguredTableAssociationInputRequestTypeDef,
     UpdateConfiguredTableInputRequestTypeDef,
     UpdateMembershipInputRequestTypeDef,
     UpdateProtectedQueryInputRequestTypeDef,
     AnalysisRuleAggregationTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListCollaborationsOutputTypeDef,
     CollaborationTypeDef,
     SchemaTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
```

### Comparing `mypy-boto3-cleanrooms-1.26.49/README.md` & `mypy-boto3-cleanrooms-1.26.96/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cleanrooms?color=blue)](https://pypistats.org/packages/mypy-boto3-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsService 1.26.49](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[boto3.CleanRoomsService 1.26.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cleanrooms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -376,25 +376,29 @@
     MemberSummaryTypeDef,
     ListMembershipsInputRequestTypeDef,
     MembershipSummaryTypeDef,
     ListProtectedQueriesInputRequestTypeDef,
     ProtectedQuerySummaryTypeDef,
     ListSchemasInputRequestTypeDef,
     SchemaSummaryTypeDef,
+    ListTagsForResourceInputRequestTypeDef,
     ProtectedQueryErrorTypeDef,
     ProtectedQueryS3OutputConfigurationTypeDef,
     ProtectedQueryS3OutputTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     ProtectedQueryStatisticsTypeDef,
+    TagResourceInputRequestTypeDef,
+    UntagResourceInputRequestTypeDef,
     UpdateCollaborationInputRequestTypeDef,
     UpdateConfiguredTableAssociationInputRequestTypeDef,
     UpdateConfiguredTableInputRequestTypeDef,
     UpdateMembershipInputRequestTypeDef,
     UpdateProtectedQueryInputRequestTypeDef,
     AnalysisRuleAggregationTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListCollaborationsOutputTypeDef,
     CollaborationTypeDef,
     SchemaTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
```

### Comparing `mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/__init__.py` & `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/__init__.pyi` & `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/__main__.py` & `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CleanRoomsService 1.26.49\nVersion:         1.26.49\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.CleanRoomsService 1.26.96\nVersion:         1.26.96\nBuilder"
+        " version: 7.13.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.49")
+    print("1.26.96")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/client.py` & `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     ListCollaborationsOutputTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListMembersOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     MemberSpecificationTypeDef,
     ProtectedQueryResultConfigurationTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     StartProtectedQueryOutputTypeDef,
     TableReferenceTypeDef,
     UpdateCollaborationOutputTypeDef,
     UpdateConfiguredTableAnalysisRuleOutputTypeDef,
@@ -150,15 +151,16 @@
         *,
         members: Sequence[MemberSpecificationTypeDef],
         name: str,
         description: str,
         creatorMemberAbilities: Sequence[MemberAbilityType],
         creatorDisplayName: str,
         queryLogStatus: CollaborationQueryLogStatusType,
-        dataEncryptionMetadata: DataEncryptionMetadataTypeDef = ...
+        dataEncryptionMetadata: DataEncryptionMetadataTypeDef = ...,
+        tags: Mapping[str, str] = ...
     ) -> CreateCollaborationOutputTypeDef:
         """
         Creates a new collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_collaboration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#create_collaboration)
         """
@@ -166,15 +168,16 @@
     def create_configured_table(
         self,
         *,
         name: str,
         tableReference: TableReferenceTypeDef,
         allowedColumns: Sequence[str],
         analysisMethod: Literal["DIRECT_QUERY"],
-        description: str = ...
+        description: str = ...,
+        tags: Mapping[str, str] = ...
     ) -> CreateConfiguredTableOutputTypeDef:
         """
         Creates a new configured table resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#create_configured_table)
         """
@@ -196,25 +199,30 @@
     def create_configured_table_association(
         self,
         *,
         name: str,
         membershipIdentifier: str,
         configuredTableIdentifier: str,
         roleArn: str,
-        description: str = ...
+        description: str = ...,
+        tags: Mapping[str, str] = ...
     ) -> CreateConfiguredTableAssociationOutputTypeDef:
         """
         Creates a configured table association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#create_configured_table_association)
         """
 
     def create_membership(
-        self, *, collaborationIdentifier: str, queryLogStatus: MembershipQueryLogStatusType
+        self,
+        *,
+        collaborationIdentifier: str,
+        queryLogStatus: MembershipQueryLogStatusType,
+        tags: Mapping[str, str] = ...
     ) -> CreateMembershipOutputTypeDef:
         """
         Creates a membership for a specific collaboration identifier and joins the
         collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_membership)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#create_membership)
@@ -446,14 +454,22 @@
         """
         Lists the schemas for relations within a collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#list_schemas)
         """
 
+    def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceOutputTypeDef:
+        """
+        Lists all of the tags that have been added to a resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_tags_for_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#list_tags_for_resource)
+        """
+
     def start_protected_query(
         self,
         *,
         type: Literal["SQL"],
         membershipIdentifier: str,
         sqlParameters: ProtectedQuerySQLParametersTypeDef,
         resultConfiguration: ProtectedQueryResultConfigurationTypeDef
@@ -461,14 +477,30 @@
         """
         Creates a protected query that is started by AWS Clean Rooms.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.start_protected_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#start_protected_query)
         """
 
+    def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
+        """
+        Tags a resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.tag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#tag_resource)
+        """
+
+    def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
+        """
+        Removes a tag or list of tags from a resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.untag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#untag_resource)
+        """
+
     def update_collaboration(
         self, *, collaborationIdentifier: str, name: str = ..., description: str = ...
     ) -> UpdateCollaborationOutputTypeDef:
         """
         Updates collaboration metadata and can only be called by the collaboration
         owner.
```

### Comparing `mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/client.pyi` & `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     ListCollaborationsOutputTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListMembersOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     MemberSpecificationTypeDef,
     ProtectedQueryResultConfigurationTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     StartProtectedQueryOutputTypeDef,
     TableReferenceTypeDef,
     UpdateCollaborationOutputTypeDef,
     UpdateConfiguredTableAnalysisRuleOutputTypeDef,
@@ -142,30 +143,32 @@
         *,
         members: Sequence[MemberSpecificationTypeDef],
         name: str,
         description: str,
         creatorMemberAbilities: Sequence[MemberAbilityType],
         creatorDisplayName: str,
         queryLogStatus: CollaborationQueryLogStatusType,
-        dataEncryptionMetadata: DataEncryptionMetadataTypeDef = ...
+        dataEncryptionMetadata: DataEncryptionMetadataTypeDef = ...,
+        tags: Mapping[str, str] = ...
     ) -> CreateCollaborationOutputTypeDef:
         """
         Creates a new collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_collaboration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#create_collaboration)
         """
     def create_configured_table(
         self,
         *,
         name: str,
         tableReference: TableReferenceTypeDef,
         allowedColumns: Sequence[str],
         analysisMethod: Literal["DIRECT_QUERY"],
-        description: str = ...
+        description: str = ...,
+        tags: Mapping[str, str] = ...
     ) -> CreateConfiguredTableOutputTypeDef:
         """
         Creates a new configured table resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#create_configured_table)
         """
@@ -185,24 +188,29 @@
     def create_configured_table_association(
         self,
         *,
         name: str,
         membershipIdentifier: str,
         configuredTableIdentifier: str,
         roleArn: str,
-        description: str = ...
+        description: str = ...,
+        tags: Mapping[str, str] = ...
     ) -> CreateConfiguredTableAssociationOutputTypeDef:
         """
         Creates a configured table association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#create_configured_table_association)
         """
     def create_membership(
-        self, *, collaborationIdentifier: str, queryLogStatus: MembershipQueryLogStatusType
+        self,
+        *,
+        collaborationIdentifier: str,
+        queryLogStatus: MembershipQueryLogStatusType,
+        tags: Mapping[str, str] = ...
     ) -> CreateMembershipOutputTypeDef:
         """
         Creates a membership for a specific collaboration identifier and joins the
         collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_membership)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#create_membership)
@@ -411,28 +419,49 @@
     ) -> ListSchemasOutputTypeDef:
         """
         Lists the schemas for relations within a collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#list_schemas)
         """
+    def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceOutputTypeDef:
+        """
+        Lists all of the tags that have been added to a resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_tags_for_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#list_tags_for_resource)
+        """
     def start_protected_query(
         self,
         *,
         type: Literal["SQL"],
         membershipIdentifier: str,
         sqlParameters: ProtectedQuerySQLParametersTypeDef,
         resultConfiguration: ProtectedQueryResultConfigurationTypeDef
     ) -> StartProtectedQueryOutputTypeDef:
         """
         Creates a protected query that is started by AWS Clean Rooms.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.start_protected_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#start_protected_query)
         """
+    def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
+        """
+        Tags a resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.tag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#tag_resource)
+        """
+    def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
+        """
+        Removes a tag or list of tags from a resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.untag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#untag_resource)
+        """
     def update_collaboration(
         self, *, collaborationIdentifier: str, name: str = ..., description: str = ...
     ) -> UpdateCollaborationOutputTypeDef:
         """
         Updates collaboration metadata and can only be called by the collaboration
         owner.
```

### Comparing `mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/literals.py` & `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,14 +145,15 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -238,14 +239,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -414,14 +416,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/literals.pyi` & `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,15 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -236,14 +237,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -412,14 +414,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/paginator.py` & `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/paginator.pyi` & `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/type_defs.py` & `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_cleanrooms.type_defs import AggregateColumnTypeDef
 
     data: AggregateColumnTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AggregateFunctionNameType,
     AnalysisRuleTypeType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
     FilterableMemberStatusType,
@@ -80,25 +80,29 @@
     "MemberSummaryTypeDef",
     "ListMembershipsInputRequestTypeDef",
     "MembershipSummaryTypeDef",
     "ListProtectedQueriesInputRequestTypeDef",
     "ProtectedQuerySummaryTypeDef",
     "ListSchemasInputRequestTypeDef",
     "SchemaSummaryTypeDef",
+    "ListTagsForResourceInputRequestTypeDef",
     "ProtectedQueryErrorTypeDef",
     "ProtectedQueryS3OutputConfigurationTypeDef",
     "ProtectedQueryS3OutputTypeDef",
     "ProtectedQuerySQLParametersTypeDef",
     "ProtectedQueryStatisticsTypeDef",
+    "TagResourceInputRequestTypeDef",
+    "UntagResourceInputRequestTypeDef",
     "UpdateCollaborationInputRequestTypeDef",
     "UpdateConfiguredTableAssociationInputRequestTypeDef",
     "UpdateConfiguredTableInputRequestTypeDef",
     "UpdateMembershipInputRequestTypeDef",
     "UpdateProtectedQueryInputRequestTypeDef",
     "AnalysisRuleAggregationTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ListCollaborationsOutputTypeDef",
     "CollaborationTypeDef",
     "SchemaTypeDef",
     "ListConfiguredTableAssociationsOutputTypeDef",
     "CreateConfiguredTableAssociationOutputTypeDef",
     "GetConfiguredTableAssociationOutputTypeDef",
     "UpdateConfiguredTableAssociationOutputTypeDef",
@@ -327,33 +331,48 @@
         "roleArn": str,
     },
 )
 _OptionalCreateConfiguredTableAssociationInputRequestTypeDef = TypedDict(
     "_OptionalCreateConfiguredTableAssociationInputRequestTypeDef",
     {
         "description": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class CreateConfiguredTableAssociationInputRequestTypeDef(
     _RequiredCreateConfiguredTableAssociationInputRequestTypeDef,
     _OptionalCreateConfiguredTableAssociationInputRequestTypeDef,
 ):
     pass
 
 
-CreateMembershipInputRequestTypeDef = TypedDict(
-    "CreateMembershipInputRequestTypeDef",
+_RequiredCreateMembershipInputRequestTypeDef = TypedDict(
+    "_RequiredCreateMembershipInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
         "queryLogStatus": MembershipQueryLogStatusType,
     },
 )
+_OptionalCreateMembershipInputRequestTypeDef = TypedDict(
+    "_OptionalCreateMembershipInputRequestTypeDef",
+    {
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateMembershipInputRequestTypeDef(
+    _RequiredCreateMembershipInputRequestTypeDef, _OptionalCreateMembershipInputRequestTypeDef
+):
+    pass
+
 
 MembershipTypeDef = TypedDict(
     "MembershipTypeDef",
     {
         "id": str,
         "arn": str,
         "collaborationArn": str,
@@ -690,14 +709,21 @@
 )
 
 
 class SchemaSummaryTypeDef(_RequiredSchemaSummaryTypeDef, _OptionalSchemaSummaryTypeDef):
     pass
 
 
+ListTagsForResourceInputRequestTypeDef = TypedDict(
+    "ListTagsForResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+
 ProtectedQueryErrorTypeDef = TypedDict(
     "ProtectedQueryErrorTypeDef",
     {
         "message": str,
         "code": str,
     },
 )
@@ -743,14 +769,30 @@
     "ProtectedQueryStatisticsTypeDef",
     {
         "totalDurationInMillis": int,
     },
     total=False,
 )
 
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Mapping[str, str],
+    },
+)
+
+UntagResourceInputRequestTypeDef = TypedDict(
+    "UntagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
+    },
+)
+
 _RequiredUpdateCollaborationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateCollaborationInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 _OptionalUpdateCollaborationInputRequestTypeDef = TypedDict(
@@ -867,14 +909,22 @@
 
 class AnalysisRuleAggregationTypeDef(
     _RequiredAnalysisRuleAggregationTypeDef, _OptionalAnalysisRuleAggregationTypeDef
 ):
     pass
 
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCollaborationsOutputTypeDef = TypedDict(
     "ListCollaborationsOutputTypeDef",
     {
         "nextToken": str,
         "collaborationList": List[CollaborationSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -992,14 +1042,15 @@
         "queryLogStatus": CollaborationQueryLogStatusType,
     },
 )
 _OptionalCreateCollaborationInputRequestTypeDef = TypedDict(
     "_OptionalCreateCollaborationInputRequestTypeDef",
     {
         "dataEncryptionMetadata": DataEncryptionMetadataTypeDef,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class CreateCollaborationInputRequestTypeDef(
     _RequiredCreateCollaborationInputRequestTypeDef, _OptionalCreateCollaborationInputRequestTypeDef
@@ -1302,14 +1353,15 @@
         "analysisMethod": Literal["DIRECT_QUERY"],
     },
 )
 _OptionalCreateConfiguredTableInputRequestTypeDef = TypedDict(
     "_OptionalCreateConfiguredTableInputRequestTypeDef",
     {
         "description": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class CreateConfiguredTableInputRequestTypeDef(
     _RequiredCreateConfiguredTableInputRequestTypeDef,
```

### Comparing `mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms/type_defs.pyi` & `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_cleanrooms.type_defs import AggregateColumnTypeDef
 
     data: AggregateColumnTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AggregateFunctionNameType,
     AnalysisRuleTypeType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
     FilterableMemberStatusType,
@@ -79,25 +79,29 @@
     "MemberSummaryTypeDef",
     "ListMembershipsInputRequestTypeDef",
     "MembershipSummaryTypeDef",
     "ListProtectedQueriesInputRequestTypeDef",
     "ProtectedQuerySummaryTypeDef",
     "ListSchemasInputRequestTypeDef",
     "SchemaSummaryTypeDef",
+    "ListTagsForResourceInputRequestTypeDef",
     "ProtectedQueryErrorTypeDef",
     "ProtectedQueryS3OutputConfigurationTypeDef",
     "ProtectedQueryS3OutputTypeDef",
     "ProtectedQuerySQLParametersTypeDef",
     "ProtectedQueryStatisticsTypeDef",
+    "TagResourceInputRequestTypeDef",
+    "UntagResourceInputRequestTypeDef",
     "UpdateCollaborationInputRequestTypeDef",
     "UpdateConfiguredTableAssociationInputRequestTypeDef",
     "UpdateConfiguredTableInputRequestTypeDef",
     "UpdateMembershipInputRequestTypeDef",
     "UpdateProtectedQueryInputRequestTypeDef",
     "AnalysisRuleAggregationTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ListCollaborationsOutputTypeDef",
     "CollaborationTypeDef",
     "SchemaTypeDef",
     "ListConfiguredTableAssociationsOutputTypeDef",
     "CreateConfiguredTableAssociationOutputTypeDef",
     "GetConfiguredTableAssociationOutputTypeDef",
     "UpdateConfiguredTableAssociationOutputTypeDef",
@@ -322,31 +326,44 @@
         "roleArn": str,
     },
 )
 _OptionalCreateConfiguredTableAssociationInputRequestTypeDef = TypedDict(
     "_OptionalCreateConfiguredTableAssociationInputRequestTypeDef",
     {
         "description": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateConfiguredTableAssociationInputRequestTypeDef(
     _RequiredCreateConfiguredTableAssociationInputRequestTypeDef,
     _OptionalCreateConfiguredTableAssociationInputRequestTypeDef,
 ):
     pass
 
-CreateMembershipInputRequestTypeDef = TypedDict(
-    "CreateMembershipInputRequestTypeDef",
+_RequiredCreateMembershipInputRequestTypeDef = TypedDict(
+    "_RequiredCreateMembershipInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
         "queryLogStatus": MembershipQueryLogStatusType,
     },
 )
+_OptionalCreateMembershipInputRequestTypeDef = TypedDict(
+    "_OptionalCreateMembershipInputRequestTypeDef",
+    {
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateMembershipInputRequestTypeDef(
+    _RequiredCreateMembershipInputRequestTypeDef, _OptionalCreateMembershipInputRequestTypeDef
+):
+    pass
 
 MembershipTypeDef = TypedDict(
     "MembershipTypeDef",
     {
         "id": str,
         "arn": str,
         "collaborationArn": str,
@@ -671,14 +688,21 @@
     },
     total=False,
 )
 
 class SchemaSummaryTypeDef(_RequiredSchemaSummaryTypeDef, _OptionalSchemaSummaryTypeDef):
     pass
 
+ListTagsForResourceInputRequestTypeDef = TypedDict(
+    "ListTagsForResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+
 ProtectedQueryErrorTypeDef = TypedDict(
     "ProtectedQueryErrorTypeDef",
     {
         "message": str,
         "code": str,
     },
 )
@@ -722,14 +746,30 @@
     "ProtectedQueryStatisticsTypeDef",
     {
         "totalDurationInMillis": int,
     },
     total=False,
 )
 
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Mapping[str, str],
+    },
+)
+
+UntagResourceInputRequestTypeDef = TypedDict(
+    "UntagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
+    },
+)
+
 _RequiredUpdateCollaborationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateCollaborationInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 _OptionalUpdateCollaborationInputRequestTypeDef = TypedDict(
@@ -836,14 +876,22 @@
 )
 
 class AnalysisRuleAggregationTypeDef(
     _RequiredAnalysisRuleAggregationTypeDef, _OptionalAnalysisRuleAggregationTypeDef
 ):
     pass
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCollaborationsOutputTypeDef = TypedDict(
     "ListCollaborationsOutputTypeDef",
     {
         "nextToken": str,
         "collaborationList": List[CollaborationSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -957,14 +1005,15 @@
         "queryLogStatus": CollaborationQueryLogStatusType,
     },
 )
 _OptionalCreateCollaborationInputRequestTypeDef = TypedDict(
     "_OptionalCreateCollaborationInputRequestTypeDef",
     {
         "dataEncryptionMetadata": DataEncryptionMetadataTypeDef,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateCollaborationInputRequestTypeDef(
     _RequiredCreateCollaborationInputRequestTypeDef, _OptionalCreateCollaborationInputRequestTypeDef
 ):
@@ -1255,14 +1304,15 @@
         "analysisMethod": Literal["DIRECT_QUERY"],
     },
 )
 _OptionalCreateConfiguredTableInputRequestTypeDef = TypedDict(
     "_OptionalCreateConfiguredTableInputRequestTypeDef",
     {
         "description": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateConfiguredTableInputRequestTypeDef(
     _RequiredCreateConfiguredTableInputRequestTypeDef,
     _OptionalCreateConfiguredTableInputRequestTypeDef,
```

### Comparing `mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms.egg-info/PKG-INFO` & `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cleanrooms
-Version: 1.26.49
-Summary: Type annotations for boto3.CleanRoomsService 1.26.49 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.96
+Summary: Type annotations for boto3.CleanRoomsService 1.26.96 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cleanrooms?color=blue)](https://pypistats.org/packages/mypy-boto3-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsService 1.26.49](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[boto3.CleanRoomsService 1.26.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cleanrooms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -408,25 +408,29 @@
     MemberSummaryTypeDef,
     ListMembershipsInputRequestTypeDef,
     MembershipSummaryTypeDef,
     ListProtectedQueriesInputRequestTypeDef,
     ProtectedQuerySummaryTypeDef,
     ListSchemasInputRequestTypeDef,
     SchemaSummaryTypeDef,
+    ListTagsForResourceInputRequestTypeDef,
     ProtectedQueryErrorTypeDef,
     ProtectedQueryS3OutputConfigurationTypeDef,
     ProtectedQueryS3OutputTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     ProtectedQueryStatisticsTypeDef,
+    TagResourceInputRequestTypeDef,
+    UntagResourceInputRequestTypeDef,
     UpdateCollaborationInputRequestTypeDef,
     UpdateConfiguredTableAssociationInputRequestTypeDef,
     UpdateConfiguredTableInputRequestTypeDef,
     UpdateMembershipInputRequestTypeDef,
     UpdateProtectedQueryInputRequestTypeDef,
     AnalysisRuleAggregationTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListCollaborationsOutputTypeDef,
     CollaborationTypeDef,
     SchemaTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
```

### Comparing `mypy-boto3-cleanrooms-1.26.49/mypy_boto3_cleanrooms.egg-info/SOURCES.txt` & `mypy-boto3-cleanrooms-1.26.96/mypy_boto3_cleanrooms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.26.49/setup.py` & `mypy-boto3-cleanrooms-1.26.96/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-cleanrooms",
-    version="1.26.49",
+    version="1.26.96",
     packages=["mypy_boto3_cleanrooms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CleanRoomsService 1.26.49 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.CleanRoomsService 1.26.96 service generated with"
+        " mypy-boto3-builder 7.13.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

