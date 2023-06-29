# Comparing `tmp/eox-tenant-9.1.1.tar.gz` & `tmp/eox-tenant-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eox-tenant-9.1.1.tar", last modified: Fri May 26 13:49:53 2023, max compression
+gzip compressed data, was "eox-tenant-9.2.0.tar", last modified: Thu Jun 29 19:31:26 2023, max compression
```

## Comparing `eox-tenant-9.1.1.tar` & `eox-tenant-9.2.0.tar`

### file list

```diff
@@ -1,135 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.571823 eox-tenant-9.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-05-26 13:49:53.571823 eox-tenant-9.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.563823 eox-tenant-9.1.1/eox_tenant/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.563823 eox-tenant-9.1.1/eox_tenant/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.563823 eox-tenant-9.1.1/eox_tenant/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.563823 eox-tenant-9.1.1/eox_tenant/api/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/tests/test_microsites.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/tests/test_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/tests/test_tenant_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.567823 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.567823 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/bearer_authentication_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/bearer_authentication_test_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/branding_api_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/edx_auth_i_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/edxmako_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/oauth_dispatch_j_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/site_configuration_module_i_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/site_configuration_module_test_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/theming_helpers_h_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/theming_helpers_test_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/users_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/users_test_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/bearer_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/branding_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/edxmako_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/get_common_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/oauth_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/site_configuration_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/theming_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.567823 eox-tenant-9.1.1/eox_tenant/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/filters/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.567823 eox-tenant-9.1.1/eox_tenant/filters/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/filters/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/filters/test/test_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.567823 eox-tenant-9.1.1/eox_tenant/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.567823 eox-tenant-9.1.1/eox_tenant/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/management/commands/change_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/management/commands/change_signup_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/management/commands/edit_tenant_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/management/commands/synchronize_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.567823 eox-tenant-9.1.1/eox_tenant/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/migrations/0003_auto_20190620_1704.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/migrations/0005_auto_20191226_1225.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/migrations/0006_tenantorganization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/migrations/0007_auto_20200922_1421.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/migrations/0008_synchronize_tenants.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/receivers_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.567823 eox-tenant-9.1.1/eox_tenant/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/settings/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.559823 eox-tenant-9.1.1/eox_tenant/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.571823 eox-tenant-9.1.1/eox_tenant/templates/eox-tenant/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/templates/eox-tenant/not_found.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.571823 eox-tenant-9.1.1/eox_tenant/templates/eox-tenant/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/templates/eox-tenant/widgets/json_widget.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.571823 eox-tenant-9.1.1/eox_tenant/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/templatetags/ednx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.571823 eox-tenant-9.1.1/eox_tenant/tenant_aware_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/tenant_aware_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/tenant_aware_functions/enrollments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.571823 eox-tenant-9.1.1/eox_tenant/tenant_wise/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/tenant_wise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/tenant_wise/context_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/tenant_wise/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.571823 eox-tenant-9.1.1/eox_tenant/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_change_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_change_signupsource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_edit_tenant_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_receivers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_tenant_aware_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_tenant_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.563823 eox-tenant-9.1.1/eox_tenant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-05-26 13:49:53.000000 eox-tenant-9.1.1/eox_tenant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-26 13:49:53.000000 eox-tenant-9.1.1/eox_tenant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:49:53.000000 eox-tenant-9.1.1/eox_tenant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-26 13:49:53.000000 eox-tenant-9.1.1/eox_tenant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:49:53.000000 eox-tenant-9.1.1/eox_tenant.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 13:49:53.000000 eox-tenant-9.1.1/eox_tenant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-05-26 13:49:53.575823 eox-tenant-9.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.546257 eox-tenant-9.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-06-29 19:31:26.546257 eox-tenant-9.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.534257 eox-tenant-9.2.0/eox_tenant/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.538257 eox-tenant-9.2.0/eox_tenant/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.538257 eox-tenant-9.2.0/eox_tenant/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.538257 eox-tenant-9.2.0/eox_tenant/api/v1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/tests/test_microsites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/tests/test_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/tests/test_tenant_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/api/v1/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.538257 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.542257 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/bearer_authentication_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/bearer_authentication_test_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/branding_api_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/dark_lang_middleware_o_test_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/dark_lang_middleware_o_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/edx_auth_i_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/edxmako_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/oauth_dispatch_j_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/site_configuration_module_i_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/site_configuration_module_test_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/theming_helpers_h_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/theming_helpers_test_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/users_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/users_test_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/bearer_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/branding_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/dark_lang_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/edxmako_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/get_common_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/oauth_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/site_configuration_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/theming_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.542257 eox-tenant-9.2.0/eox_tenant/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/filters/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.542257 eox-tenant-9.2.0/eox_tenant/filters/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/filters/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/filters/test/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.542257 eox-tenant-9.2.0/eox_tenant/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.542257 eox-tenant-9.2.0/eox_tenant/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/management/commands/change_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/management/commands/change_signup_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/management/commands/edit_tenant_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/management/commands/synchronize_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.542257 eox-tenant-9.2.0/eox_tenant/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/migrations/0003_auto_20190620_1704.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/migrations/0005_auto_20191226_1225.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/migrations/0006_tenantorganization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/migrations/0007_auto_20200922_1421.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/migrations/0008_synchronize_tenants.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/receivers_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.542257 eox-tenant-9.2.0/eox_tenant/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/settings/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.530257 eox-tenant-9.2.0/eox_tenant/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.542257 eox-tenant-9.2.0/eox_tenant/templates/eox-tenant/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/templates/eox-tenant/not_found.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.546257 eox-tenant-9.2.0/eox_tenant/templates/eox-tenant/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/templates/eox-tenant/widgets/json_widget.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.546257 eox-tenant-9.2.0/eox_tenant/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/templatetags/ednx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.546257 eox-tenant-9.2.0/eox_tenant/tenant_aware_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/tenant_aware_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/tenant_aware_functions/enrollments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/tenant_aware_functions/released_languages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.546257 eox-tenant-9.2.0/eox_tenant/tenant_wise/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/tenant_wise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/tenant_wise/context_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/tenant_wise/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.546257 eox-tenant-9.2.0/eox_tenant/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_change_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_change_signupsource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_edit_tenant_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_receivers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_tenant_aware_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_tenant_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test/test_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/eox_tenant/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:31:26.538257 eox-tenant-9.2.0/eox_tenant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-06-29 19:31:26.000000 eox-tenant-9.2.0/eox_tenant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-29 19:31:26.000000 eox-tenant-9.2.0/eox_tenant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:31:26.000000 eox-tenant-9.2.0/eox_tenant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-29 19:31:26.000000 eox-tenant-9.2.0/eox_tenant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:31:26.000000 eox-tenant-9.2.0/eox_tenant.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 19:31:26.000000 eox-tenant-9.2.0/eox_tenant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-29 19:31:26.550257 eox-tenant-9.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-29 19:31:14.000000 eox-tenant-9.2.0/setup.py
```

### Comparing `eox-tenant-9.1.1/LICENSE.txt` & `eox-tenant-9.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/PKG-INFO` & `eox-tenant-9.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eox-tenant
-Version: 9.1.1
+Version: 9.2.0
 Summary: Edunext Open edx extensions tenant.
 Author: eduNEXT
 Author-email: contact@edunext.co
 License: AGPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
```

### Comparing `eox-tenant-9.1.1/README.rst` & `eox-tenant-9.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/admin.py` & `eox-tenant-9.2.0/eox_tenant/admin.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/api/v1/permissions.py` & `eox-tenant-9.2.0/eox_tenant/api/v1/permissions.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/api/v1/serializers.py` & `eox-tenant-9.2.0/eox_tenant/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/api/v1/tests/test_microsites.py` & `eox-tenant-9.2.0/eox_tenant/api/v1/tests/test_microsites.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/api/v1/tests/test_permissions.py` & `eox-tenant-9.2.0/eox_tenant/api/v1/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/api/v1/tests/test_routes.py` & `eox-tenant-9.2.0/eox_tenant/api/v1/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/api/v1/tests/test_tenant_config.py` & `eox-tenant-9.2.0/eox_tenant/api/v1/tests/test_tenant_config.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/api/v1/viewsets.py` & `eox-tenant-9.2.0/eox_tenant/api/v1/viewsets.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/apps.py` & `eox-tenant-9.2.0/eox_tenant/apps.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/async_utils.py` & `eox-tenant-9.2.0/eox_tenant/async_utils.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/auth.py` & `eox-tenant-9.2.0/eox_tenant/auth.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/auth.py` & `eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/auth.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/bearer_authentication_l_v1.py` & `eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/bearer_authentication_l_v1.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/edx_auth_i_v1.py` & `eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/edx_auth_i_v1.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/site_configuration_module_test_v1.py` & `eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/backends/site_configuration_module_test_v1.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/site_configuration_module.py` & `eox-tenant-9.2.0/eox_tenant/edxapp_wrapper/site_configuration_module.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/filters/pipeline.py` & `eox-tenant-9.2.0/eox_tenant/filters/pipeline.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/filters/test/test_pipeline.py` & `eox-tenant-9.2.0/eox_tenant/filters/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/management/commands/change_domain.py` & `eox-tenant-9.2.0/eox_tenant/management/commands/change_domain.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/management/commands/change_signup_sources.py` & `eox-tenant-9.2.0/eox_tenant/management/commands/change_signup_sources.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/management/commands/edit_tenant_values.py` & `eox-tenant-9.2.0/eox_tenant/management/commands/edit_tenant_values.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/management/commands/synchronize_organizations.py` & `eox-tenant-9.2.0/eox_tenant/management/commands/synchronize_organizations.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/middleware.py` & `eox-tenant-9.2.0/eox_tenant/middleware.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/migrations/0001_initial.py` & `eox-tenant-9.2.0/eox_tenant/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/migrations/0003_auto_20190620_1704.py` & `eox-tenant-9.2.0/eox_tenant/migrations/0003_auto_20190620_1704.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/migrations/0005_auto_20191226_1225.py` & `eox-tenant-9.2.0/eox_tenant/migrations/0005_auto_20191226_1225.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/migrations/0006_tenantorganization.py` & `eox-tenant-9.2.0/eox_tenant/migrations/0006_tenantorganization.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/migrations/0007_auto_20200922_1421.py` & `eox-tenant-9.2.0/eox_tenant/migrations/0007_auto_20200922_1421.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/models.py` & `eox-tenant-9.2.0/eox_tenant/models.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/permissions.py` & `eox-tenant-9.2.0/eox_tenant/permissions.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/pipeline.py` & `eox-tenant-9.2.0/eox_tenant/pipeline.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/receivers_helpers.py` & `eox-tenant-9.2.0/eox_tenant/receivers_helpers.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/settings/common.py` & `eox-tenant-9.2.0/eox_tenant/settings/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     settings.EOX_TENANT_EDX_AUTH_BACKEND = "eox_tenant.edxapp_wrapper.backends.edx_auth_i_v1"
     settings.EOX_TENANT_USERS_BACKEND = 'eox_tenant.edxapp_wrapper.backends.users_l_v1'
     settings.EOX_TENANT_BEARER_AUTHENTICATION = 'eox_tenant.edxapp_wrapper.backends.bearer_authentication_l_v1'
     settings.EOX_MAX_CONFIG_OVERRIDE_SECONDS = 300
     settings.EDXMAKO_MODULE_BACKEND = 'eox_tenant.edxapp_wrapper.backends.edxmako_l_v1'
     settings.UTILS_MODULE_BACKEND = 'eox_tenant.edxapp_wrapper.backends.util_h_v1'
     settings.CHANGE_DOMAIN_DEFAULT_SITE_NAME = "stage.edunext.co"
+    settings.DARK_LANG_MIDDLEWARE = 'eox_tenant.edxapp_wrapper.backends.dark_lang_middleware_o_v1'
     settings.EOX_TENANT_LOAD_PERMISSIONS = True
     settings.EOX_TENANT_APPEND_LMS_MIDDLEWARE_CLASSES = False
     settings.USE_EOX_TENANT = False
 
     settings.EOX_TENANT_ASYNC_TASKS_HANDLER_DICT = {
         "openedx.core.djangoapps.schedules.tasks.ScheduleRecurringNudge": "get_host_from_siteid",
     }
```

### Comparing `eox-tenant-9.1.1/eox_tenant/settings/production.py` & `eox-tenant-9.2.0/eox_tenant/settings/production.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/settings/test.py` & `eox-tenant-9.2.0/eox_tenant/settings/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         INSTALLED_APPS.append(app)
 
 GET_CERTIFICATES_MODULE = 'eox_tenant.edxapp_wrapper.backends.certificates_module_test_v1'
 GET_SITE_CONFIGURATION_MODULE = 'eox_tenant.edxapp_wrapper.backends.site_configuration_module_test_v1'
 GET_THEMING_HELPERS = 'eox_tenant.edxapp_wrapper.backends.theming_helpers_test_v1'
 EOX_TENANT_USERS_BACKEND = 'eox_tenant.edxapp_wrapper.backends.users_test_v1'
 EOX_TENANT_BEARER_AUTHENTICATION = 'eox_tenant.edxapp_wrapper.backends.bearer_authentication_test_v1'
+DARK_LANG_MIDDLEWARE = 'eox_tenant.edxapp_wrapper.backends.dark_lang_middleware_o_test_v1'
 
 COURSE_KEY_PATTERN = r'(?P<course_key_string>[^/+]+(/|\+)[^/+]+(/|\+)[^/?]+)'
 COURSE_ID_PATTERN = COURSE_KEY_PATTERN.replace('course_key_string', 'course_id')
 
 TEST_DICT_OVERRIDE_TEST = {
     'key1': 'Some Value'
 }
```

### Comparing `eox-tenant-9.1.1/eox_tenant/signals.py` & `eox-tenant-9.2.0/eox_tenant/signals.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/templatetags/ednx.py` & `eox-tenant-9.2.0/eox_tenant/templatetags/ednx.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/tenant_aware_functions/enrollments.py` & `eox-tenant-9.2.0/eox_tenant/tenant_aware_functions/enrollments.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/tenant_wise/context_managers.py` & `eox-tenant-9.2.0/eox_tenant/tenant_wise/context_managers.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/tenant_wise/proxies.py` & `eox-tenant-9.2.0/eox_tenant/tenant_wise/proxies.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 import logging
 from itertools import chain
 
 import six
 from django.conf import settings
 from django.core.cache import cache
 
+from eox_tenant.edxapp_wrapper.dark_lang_middleware import get_dark_lang_middleware
 from eox_tenant.edxapp_wrapper.site_configuration_module import get_site_configuration_models
 from eox_tenant.models import Microsite, TenantConfig, TenantOrganization
 from eox_tenant.utils import clean_serializable_values
 
 SiteConfigurationModels = get_site_configuration_models()
+DarkLangMiddleware = get_dark_lang_middleware()
 
 TENANT_ALL_ORGS_CACHE_KEY = "tenant.all_orgs_list"
 EOX_TENANT_CACHE_KEY_TIMEOUT = getattr(
     settings,
     "EOX_TENANT_CACHE_KEY_TIMEOUT",
     300
 )
@@ -192,7 +194,43 @@
                 org_filter = [org_filter]
 
             for org in org_filter:
                 key = "org-value-{}-{}".format(org, val_name)
                 cls.set_key_to_cache(key, result)
 
         cls.set_key_to_cache(pre_load_value_key, True)
+
+
+class DarkLangMiddlewareProxy(DarkLangMiddleware):
+    """This Middleware will be used if you have FEATURES["EDNX_SITE_AWARE_LOCALE"] in True.
+    This take the released_languages from the site aware settings, and set a HTTP_ACCEPT_LANGUAGE if
+    you don't have one."""
+
+    class Meta:
+        """ Set as a proxy model. """
+        proxy = True
+
+    @property
+    def released_langs(self):
+        """
+        Current list of released languages from settings.
+        """
+
+        get_language_options = getattr(settings, "released_languages", "")
+        language_options = [lang.lower().strip() for lang in get_language_options.split(',')]
+        if settings.LANGUAGE_CODE not in language_options:
+            language_options.append(settings.LANGUAGE_CODE)
+        return language_options
+
+    def process_request(self, request):
+        """
+        This will be run when you do a request, and prevent user from requesting un-released languages.
+        """
+
+        # If the request doesn't have HTTP_ACCEPT_LANGUAGE, eduNEXT set it to
+        # settings.LANGUAGE_CODE that is site aware so that
+        # django.utils.locale.LocaleMiddleware can pick it up
+        accept = request.META.get('HTTP_ACCEPT_LANGUAGE', None)
+        if not accept:
+            request.META['HTTP_ACCEPT_LANGUAGE'] = f"{settings.LANGUAGE_CODE};q=0.1"
+
+        self._clean_accept_headers(request)
```

### Comparing `eox-tenant-9.1.1/eox_tenant/test/test_admin.py` & `eox-tenant-9.2.0/eox_tenant/test/test_admin.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/test/test_async_utils.py` & `eox-tenant-9.2.0/eox_tenant/test/test_async_utils.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/test/test_auth_backend.py` & `eox-tenant-9.2.0/eox_tenant/test/test_auth_backend.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/test/test_change_domain.py` & `eox-tenant-9.2.0/eox_tenant/test/test_change_domain.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/test/test_change_signupsource.py` & `eox-tenant-9.2.0/eox_tenant/test/test_change_signupsource.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/test/test_edit_tenant_values.py` & `eox-tenant-9.2.0/eox_tenant/test/test_edit_tenant_values.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/test/test_middleware.py` & `eox-tenant-9.2.0/eox_tenant/test/test_middleware.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/test/test_models.py` & `eox-tenant-9.2.0/eox_tenant/test/test_models.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/test/test_pipeline.py` & `eox-tenant-9.2.0/eox_tenant/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/test/test_receivers_helpers.py` & `eox-tenant-9.2.0/eox_tenant/test/test_receivers_helpers.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/test/test_signals.py` & `eox-tenant-9.2.0/eox_tenant/test/test_signals.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/test/test_tenant_aware_functions.py` & `eox-tenant-9.2.0/eox_tenant/test/test_tenant_aware_functions.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/test/test_tenant_wise.py` & `eox-tenant-9.2.0/eox_tenant/test/test_tenant_wise.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/test/test_utils.py` & `eox-tenant-9.2.0/eox_tenant/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/test/test_views.py` & `eox-tenant-9.2.0/eox_tenant/test/test_views.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/test/test_wrappers.py` & `eox-tenant-9.2.0/eox_tenant/test/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/utils.py` & `eox-tenant-9.2.0/eox_tenant/utils.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/validators.py` & `eox-tenant-9.2.0/eox_tenant/validators.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/views.py` & `eox-tenant-9.2.0/eox_tenant/views.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant/widgets.py` & `eox-tenant-9.2.0/eox_tenant/widgets.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.1/eox_tenant.egg-info/PKG-INFO` & `eox-tenant-9.2.0/eox_tenant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eox-tenant
-Version: 9.1.1
+Version: 9.2.0
 Summary: Edunext Open edx extensions tenant.
 Author: eduNEXT
 Author-email: contact@edunext.co
 License: AGPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
```

### Comparing `eox-tenant-9.1.1/eox_tenant.egg-info/SOURCES.txt` & `eox-tenant-9.2.0/eox_tenant.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -41,24 +41,27 @@
 eox_tenant/api/v1/tests/test_permissions.py
 eox_tenant/api/v1/tests/test_routes.py
 eox_tenant/api/v1/tests/test_tenant_config.py
 eox_tenant/edxapp_wrapper/__init__.py
 eox_tenant/edxapp_wrapper/auth.py
 eox_tenant/edxapp_wrapper/bearer_authentication.py
 eox_tenant/edxapp_wrapper/branding_api.py
+eox_tenant/edxapp_wrapper/dark_lang_middleware.py
 eox_tenant/edxapp_wrapper/edxmako_module.py
 eox_tenant/edxapp_wrapper/get_common_util.py
 eox_tenant/edxapp_wrapper/oauth_dispatch.py
 eox_tenant/edxapp_wrapper/site_configuration_module.py
 eox_tenant/edxapp_wrapper/theming_helpers.py
 eox_tenant/edxapp_wrapper/users.py
 eox_tenant/edxapp_wrapper/backends/__init__.py
 eox_tenant/edxapp_wrapper/backends/bearer_authentication_l_v1.py
 eox_tenant/edxapp_wrapper/backends/bearer_authentication_test_v1.py
 eox_tenant/edxapp_wrapper/backends/branding_api_l_v1.py
+eox_tenant/edxapp_wrapper/backends/dark_lang_middleware_o_test_v1.py
+eox_tenant/edxapp_wrapper/backends/dark_lang_middleware_o_v1.py
 eox_tenant/edxapp_wrapper/backends/edx_auth_i_v1.py
 eox_tenant/edxapp_wrapper/backends/edxmako_l_v1.py
 eox_tenant/edxapp_wrapper/backends/oauth_dispatch_j_v1.py
 eox_tenant/edxapp_wrapper/backends/site_configuration_module_i_v1.py
 eox_tenant/edxapp_wrapper/backends/site_configuration_module_test_v1.py
 eox_tenant/edxapp_wrapper/backends/theming_helpers_h_v1.py
 eox_tenant/edxapp_wrapper/backends/theming_helpers_test_v1.py
@@ -87,14 +90,15 @@
 eox_tenant/settings/test.py
 eox_tenant/templates/eox-tenant/not_found.html
 eox_tenant/templates/eox-tenant/widgets/json_widget.html
 eox_tenant/templatetags/__init__.py
 eox_tenant/templatetags/ednx.py
 eox_tenant/tenant_aware_functions/__init__.py
 eox_tenant/tenant_aware_functions/enrollments.py
+eox_tenant/tenant_aware_functions/released_languages.py
 eox_tenant/tenant_wise/__init__.py
 eox_tenant/tenant_wise/context_managers.py
 eox_tenant/tenant_wise/proxies.py
 eox_tenant/test/__init__.py
 eox_tenant/test/test_admin.py
 eox_tenant/test/test_async_utils.py
 eox_tenant/test/test_auth_backend.py
```

### Comparing `eox-tenant-9.1.1/setup.cfg` & `eox-tenant-9.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 9.1.1
+current_version = 9.2.0
 commit = False
 tag = False
 
 [bumpversion:file:eox_tenant/__init__.py]
 
 [coverage:run]
 data_file = .coverage
```

### Comparing `eox-tenant-9.1.1/setup.py` & `eox-tenant-9.2.0/setup.py`

 * *Files identical despite different names*

