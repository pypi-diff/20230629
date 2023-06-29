# Comparing `tmp/ds_caselaw_marklogic_api_client-8.0.0.tar.gz` & `tmp/ds_caselaw_marklogic_api_client-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds_caselaw_marklogic_api_client-8.0.0.tar", max compression
+gzip compressed data, was "ds_caselaw_marklogic_api_client-9.0.0.tar", max compression
```

## Comparing `ds_caselaw_marklogic_api_client-8.0.0.tar` & `ds_caselaw_marklogic_api_client-9.0.0.tar`

### file list

```diff
@@ -1,52 +1,54 @@
--rw-r--r--   0        0        0     1108 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/LICENSE.md
--rw-r--r--   0        0        0     3128 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/README.md
--rw-r--r--   0        0        0      937 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/pyproject.toml
--rw-r--r--   0        0        0    27558 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/Client.py
--rw-r--r--   0        0        0        0 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/__init__.py
--rw-r--r--   0        0        0     2236 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/content_hash.py
--rw-r--r--   0        0        0     2526 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/errors.py
--rw-r--r--   0        0        0        0 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/models/__init__.py
--rw-r--r--   0        0        0     6376 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/models/judgments.py
--rw-r--r--   0        0        0     1341 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/models/utilities/__init__.py
--rw-r--r--   0        0        0     4098 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/models/utilities/aws.py
--rw-r--r--   0        0        0        0 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/py.typed
--rw-r--r--   0        0        0        0 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/responses/__init__.py
--rw-r--r--   0        0        0     1697 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/responses/search_response.py
--rw-r--r--   0        0        0     6999 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/responses/search_result.py
--rw-r--r--   0        0        0      918 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/responses/xsl/search_match.xsl
--rw-r--r--   0        0        0     3001 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/search_parameters.py
--rw-r--r--   0        0        0     3821 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xml_tools.py
--rw-r--r--   0        0        0      220 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/break_judgment_checkout.xqy
--rw-r--r--   0        0        0      197 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/checkin_judgment.xqy
--rw-r--r--   0        0        0      385 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/checkout_judgment.xqy
--rw-r--r--   0        0        0      318 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/copy_judgment.xqy
--rw-r--r--   0        0        0      302 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/delete_judgment.xqy
--rw-r--r--   0        0        0      715 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_judgment.xqy
--rw-r--r--   0        0        0      193 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_judgment_checkout_status.xqy
--rw-r--r--   0        0        0      292 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_judgment_version.xqy
--rw-r--r--   0        0        0      172 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_last_modified.xqy
--rw-r--r--   0        0        0      338 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_metadata_citation.xqy
--rw-r--r--   0        0        0      339 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_metadata_court.xqy
--rw-r--r--   0        0        0      221 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_metadata_name.xqy
--rw-r--r--   0        0        0      358 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_metadata_work_date.xqy
--rw-r--r--   0        0        0      594 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_properties_for_search_results.xqy
--rw-r--r--   0        0        0      209 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_property.xqy
--rw-r--r--   0        0        0      326 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/insert_judgment.xqy
--rw-r--r--   0        0        0       95 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/judgment_exists.xqy
--rw-r--r--   0        0        0      190 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/list_judgment_versions.xqy
--rw-r--r--   0        0        0      355 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_boolean_property.xqy
--rw-r--r--   0        0        0      659 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_citation.xqy
--rw-r--r--   0        0        0     1013 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_court.xqy
--rw-r--r--   0        0        0      756 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_name.xqy
--rw-r--r--   0        0        0     1762 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_this_uri.xqy
--rw-r--r--   0        0        0      939 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy
--rw-r--r--   0        0        0      343 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_property.xqy
--rw-r--r--   0        0        0      420 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/update_judgment.xqy
--rw-r--r--   0        0        0      556 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/update_locked_judgment.xqy
--rw-r--r--   0        0        0      371 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/user_has_privilege.xqy
--rw-r--r--   0        0        0      246 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/user_has_role.xqy
--rw-r--r--   0        0        0      156 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/validate_all_documents.xqy
--rw-r--r--   0        0        0      199 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/xslt.xqy
--rw-r--r--   0        0        0     1381 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/xslt_transform.xqy
--rw-r--r--   0        0        0     3536 2023-05-30 16:16:32.007963 ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery_type_dicts.py
--rw-r--r--   0        0        0     4182 1970-01-01 00:00:00.000000 ds_caselaw_marklogic_api_client-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/LICENSE.md
+-rw-r--r--   0        0        0     3128 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/README.md
+-rw-r--r--   0        0        0      937 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0    27562 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/Client.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/client_helpers/__init__.py
+-rw-r--r--   0        0        0     1580 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/client_helpers/search_helpers.py
+-rw-r--r--   0        0        0     2236 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/content_hash.py
+-rw-r--r--   0        0        0     2526 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/errors.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/models/__init__.py
+-rw-r--r--   0        0        0     6376 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/models/judgments.py
+-rw-r--r--   0        0        0     1341 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/models/utilities/__init__.py
+-rw-r--r--   0        0        0     4098 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/models/utilities/aws.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/py.typed
+-rw-r--r--   0        0        0        0 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/responses/__init__.py
+-rw-r--r--   0        0        0     1697 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/responses/search_response.py
+-rw-r--r--   0        0        0     6999 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/responses/search_result.py
+-rw-r--r--   0        0        0      918 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/responses/xsl/search_match.xsl
+-rw-r--r--   0        0        0     3009 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/search_parameters.py
+-rw-r--r--   0        0        0     3821 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xml_tools.py
+-rw-r--r--   0        0        0      220 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/break_judgment_checkout.xqy
+-rw-r--r--   0        0        0      197 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/checkin_judgment.xqy
+-rw-r--r--   0        0        0      385 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/checkout_judgment.xqy
+-rw-r--r--   0        0        0      318 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/copy_judgment.xqy
+-rw-r--r--   0        0        0      302 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/delete_judgment.xqy
+-rw-r--r--   0        0        0      715 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/get_judgment.xqy
+-rw-r--r--   0        0        0      193 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/get_judgment_checkout_status.xqy
+-rw-r--r--   0        0        0      292 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/get_judgment_version.xqy
+-rw-r--r--   0        0        0      172 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/get_last_modified.xqy
+-rw-r--r--   0        0        0      338 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/get_metadata_citation.xqy
+-rw-r--r--   0        0        0      339 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/get_metadata_court.xqy
+-rw-r--r--   0        0        0      221 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/get_metadata_name.xqy
+-rw-r--r--   0        0        0      358 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/get_metadata_work_date.xqy
+-rw-r--r--   0        0        0      594 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/get_properties_for_search_results.xqy
+-rw-r--r--   0        0        0      209 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/get_property.xqy
+-rw-r--r--   0        0        0      326 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/insert_judgment.xqy
+-rw-r--r--   0        0        0       95 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/judgment_exists.xqy
+-rw-r--r--   0        0        0      190 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/list_judgment_versions.xqy
+-rw-r--r--   0        0        0      355 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/set_boolean_property.xqy
+-rw-r--r--   0        0        0      659 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/set_metadata_citation.xqy
+-rw-r--r--   0        0        0     1013 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/set_metadata_court.xqy
+-rw-r--r--   0        0        0      756 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/set_metadata_name.xqy
+-rw-r--r--   0        0        0     1762 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/set_metadata_this_uri.xqy
+-rw-r--r--   0        0        0      939 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy
+-rw-r--r--   0        0        0      343 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/set_property.xqy
+-rw-r--r--   0        0        0      420 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/update_judgment.xqy
+-rw-r--r--   0        0        0      556 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/update_locked_judgment.xqy
+-rw-r--r--   0        0        0      371 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/user_has_privilege.xqy
+-rw-r--r--   0        0        0      246 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/user_has_role.xqy
+-rw-r--r--   0        0        0      156 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/validate_all_documents.xqy
+-rw-r--r--   0        0        0      199 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/xslt.xqy
+-rw-r--r--   0        0        0     1381 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/xslt_transform.xqy
+-rw-r--r--   0        0        0     3536 2023-05-31 12:10:59.692379 ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery_type_dicts.py
+-rw-r--r--   0        0        0     4182 1970-01-01 00:00:00.000000 ds_caselaw_marklogic_api_client-9.0.0/PKG-INFO
```

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/LICENSE.md` & `ds_caselaw_marklogic_api_client-9.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/README.md` & `ds_caselaw_marklogic_api_client-9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/pyproject.toml` & `ds_caselaw_marklogic_api_client-9.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ds-caselaw-marklogic-api-client"
-version = "8.0.0"
+version = "9.0.0"
 description = "An API client for interacting with the underlying data in Find Caselaw."
 authors = ["The National Archives"]
 homepage = "https://github.com/nationalarchives/ds-caselaw-custom-api-client"
 keywords = ["national archives", "caselaw"]
 readme = "README.md"
 packages = [
     { include = "caselawclient", from = "src" },
```

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/Client.py` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/Client.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,15 @@
         self._raise_for_status(response)
         return response
 
     def advanced_search(self, search_parameters: SearchParameters) -> requests.Response:
         """
         Performs a search on the entire document set.
 
-        :param q:
+        :param query:
         :param court:
         :param judge:
         :param party:
         :param neutral_citation:
         :param specific_keyword:
         :param order:
         :param date_from:
```

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/content_hash.py` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/content_hash.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/errors.py` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/errors.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/models/judgments.py` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/models/judgments.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/models/utilities/__init__.py` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/models/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/models/utilities/aws.py` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/models/utilities/aws.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/responses/search_response.py` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/responses/search_response.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/responses/search_result.py` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/responses/search_result.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/responses/xsl/search_match.xsl` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/responses/xsl/search_match.xsl`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/search_parameters.py` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/search_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 RESULTS_PER_PAGE = 10
 
 
 @dataclass
 class SearchParameters:
     """Represents search parameters for a case law search."""
 
-    q: Optional[str] = None
+    query: Optional[str] = None
     court: Optional[str] = None
     judge: Optional[str] = None
     party: Optional[str] = None
     neutral_citation: Optional[str] = None
     specific_keyword: Optional[str] = None
     order: Optional[str] = None
     date_from: Optional[str] = None
@@ -29,15 +29,15 @@
         fo MarkLogic.
         """
         return {
             "court": self._marklogic_courts,
             "judge": str(self.judge or ""),
             "page": max(1, int(self.page)),
             "page-size": int(self.page_size),
-            "q": str(self.q or ""),
+            "q": str(self.query or ""),
             "party": str(self.party or ""),
             "neutral_citation": str(self.neutral_citation or ""),
             "specific_keyword": str(self.specific_keyword or ""),
             "order": str(self.order or ""),
             "from": str(self.date_from or ""),
             "to": str(self.date_to or ""),
             "show_unpublished": str(self.show_unpublished).lower(),
```

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xml_tools.py` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xml_tools.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_judgment.xqy` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/get_judgment.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/get_properties_for_search_results.xqy` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/get_properties_for_search_results.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_citation.xqy` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/set_metadata_citation.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_court.xqy` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/set_metadata_court.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_name.xqy` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/set_metadata_name.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_this_uri.xqy` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/set_metadata_this_uri.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/update_locked_judgment.xqy` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/update_locked_judgment.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery/xslt_transform.xqy` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery/xslt_transform.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/src/caselawclient/xquery_type_dicts.py` & `ds_caselaw_marklogic_api_client-9.0.0/src/caselawclient/xquery_type_dicts.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-8.0.0/PKG-INFO` & `ds_caselaw_marklogic_api_client-9.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds-caselaw-marklogic-api-client
-Version: 8.0.0
+Version: 9.0.0
 Summary: An API client for interacting with the underlying data in Find Caselaw.
 Home-page: https://github.com/nationalarchives/ds-caselaw-custom-api-client
 Keywords: national archives,caselaw
 Author: The National Archives
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

