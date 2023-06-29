# Comparing `tmp/peek-core-user-3.4.5.tar.gz` & `tmp/peek-core-user-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-core-user-3.4.5.tar", last modified: Wed Jun 28 07:26:33 2023, max compression
+gzip compressed data, was "peek-core-user-3.4.6.tar", last modified: Thu Jun 29 10:20:23 2023, max compression
```

## Comparing `peek-core-user-3.4.5.tar` & `peek-core-user-3.4.6.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.293077 peek-core-user-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      376 2023-06-28 07:26:33.293077 peek-core-user-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      293 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.282076 peek-core-user-3.4.5/peek_core_user/
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)      271 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/TempUnitTest.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-06-28 07:26:33.000000 peek-core-user-3.4.5/peek_core_user/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.282076 peek-core-user-3.4.5/peek_core_user/_private/
--rw-r--r--   0 root         (0) root         (0)      183 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.282076 peek-core-user-3.4.5/peek_core_user/_private/admin-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.283077 peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-internal-group-table/
--rw-r--r--   0 root         (0) root         (0)     1643 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-internal-group-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     2063 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-internal-group-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.283077 peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-internal-user-table/
--rw-r--r--   0 root         (0) root         (0)     5971 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-internal-user-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     4802 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-internal-user-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.283077 peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-ldap-setting-table/
--rw-r--r--   0 root         (0) root         (0)     4398 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-ldap-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     2040 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-ldap-setting-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.283077 peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     1828 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1626 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-setting-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.283077 peek-core-user-3.4.5/peek_core_user/_private/admin-app/logged-in-user/
--rw-r--r--   0 root         (0) root         (0)     1673 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/logged-in-user/logged-in-user.component.html
--rw-r--r--   0 root         (0) root         (0)     3419 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/logged-in-user/logged-in-user.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.283077 peek-core-user-3.4.5/peek_core_user/_private/admin-app/tuples/
--rw-r--r--   0 root         (0) root         (0)      527 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/tuples/InternalGroupTuple.ts
--rw-r--r--   0 root         (0) root         (0)      996 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/tuples/InternalUserTuple.ts
--rw-r--r--   0 root         (0) root         (0)      541 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/tuples/InternalUserUpdatePasswordAction.ts
--rw-r--r--   0 root         (0) root         (0)      646 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/tuples/LdapSettingTuple.ts
--rw-r--r--   0 root         (0) root         (0)      580 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/tuples/SettingPropertyTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.283077 peek-core-user-3.4.5/peek_core_user/_private/admin-app/tuples/constants/
--rw-r--r--   0 root         (0) root         (0)       79 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/tuples/constants/UserAuthTargetEnum.ts
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/user.component.html
--rw-r--r--   0 root         (0) root         (0)      158 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/user.component.ts
--rw-r--r--   0 root         (0) root         (0)     2998 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/admin-app/user.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.283077 peek-core-user-3.4.5/peek_core_user/_private/agent/
--rw-r--r--   0 root         (0) root         (0)      847 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/agent/AgentEntryHook.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/agent/RpcForLogic.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.284077 peek-core-user-3.4.5/peek_core_user/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      299 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      552 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.285076 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     4602 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/0498d92479c8_implemented_internal_directory.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/1176bc54abf3_added_foreign_key_to_user_logged_in.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/2209cf338e6d_added_ldap_table.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/2c6728ebc562_separated_password.py
--rw-r--r--   0 root         (0) root         (0)     2463 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/3a9cddaf05e5_added_settings_table.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/3fd59734e444_removed_string_limits.py
--rw-r--r--   0 root         (0) root         (0)     1096 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/3fec57d8da58_initial.py
--rw-r--r--   0 root         (0) root         (0)     2501 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/43df0e05c728_added_user_import_source.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/45c62f8acd87_added_vehical_to_loggedin.py
--rw-r--r--   0 root         (0) root         (0)     1617 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/56d805072d2a_added_importhash.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/5e33c6b788fd_removed_unique_logged_in_user.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/73d65f042834_removed_foreign_key_from_user_logged_in.py
--rw-r--r--   0 root         (0) root         (0)     1269 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/7e3f668edf0e_updated_settings.py
--rw-r--r--   0 root         (0) root         (0)      663 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/9b65be31926e_timezone_aware.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2664 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/b09fe7b3b31b_add_userkey.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/d03db0fcb600_convert_userkey_and_username_to_all_.py
--rw-r--r--   0 root         (0) root         (0)      829 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/d79da9333e2a_drop_internaluser_rows_from_ldap_for_useruuid_change.py
--rw-r--r--   0 root         (0) root         (0)      756 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/eef485ef2e0e_added_agenturi_column_to_ldapsetting.py
--rw-r--r--   0 root         (0) root         (0)       95 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.285076 peek-core-user-3.4.5/peek_core_user/_private/both-app/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/both-app/__init__.py
--rw-r--r--   0 root         (0) root         (0)      779 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/both-app/plugin-user.module.ts
--rw-r--r--   0 root         (0) root         (0)      667 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/both-app/plugin-user.routes.ts
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/both-app/plugin-user.text.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.285076 peek-core-user-3.4.5/peek_core_user/_private/both-app/scss/
--rw-r--r--   0 root         (0) root         (0)      560 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/both-app/scss/plugin-user.dweb.scss
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/both-app/scss/plugin-user.mweb.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.285076 peek-core-user-3.4.5/peek_core_user/_private/both-app/tuples/
--rw-r--r--   0 root         (0) root         (0)      557 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/both-app/tuples/UserLoginUiSettingTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.285076 peek-core-user-3.4.5/peek_core_user/_private/both-app/user-login/
--rw-r--r--   0 root         (0) root         (0)     1563 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/both-app/user-login/user-login.component.dweb.html
--rw-r--r--   0 root         (0) root         (0)     3209 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/both-app/user-login/user-login.component.mweb.html
--rw-r--r--   0 root         (0) root         (0)     6145 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/both-app/user-login/user-login.component.ts
--rw-r--r--   0 root         (0) root         (0)      502 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/both-app/user-login/user-login.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.285076 peek-core-user-3.4.5/peek_core_user/_private/both-app/user-logout/
--rw-r--r--   0 root         (0) root         (0)      744 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/both-app/user-logout/user-logout.component.dweb.html
--rw-r--r--   0 root         (0) root         (0)     1281 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/both-app/user-logout/user-logout.component.mweb.html
--rw-r--r--   0 root         (0) root         (0)     2990 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/both-app/user-logout/user-logout.component.ts
--rw-r--r--   0 root         (0) root         (0)      507 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/both-app/user-logout/user-logout.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.286076 peek-core-user-3.4.5/peek_core_user/_private/both-assets/
--rw-r--r--   0 root         (0) root         (0)     5572 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/both-assets/plugin_icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.286076 peek-core-user-3.4.5/peek_core_user/_private/client/
--rw-r--r--   0 root         (0) root         (0)     1320 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/client/PluginClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      474 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/client/TupleActionProcessorProxy.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/client/TupleDataObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.286076 peek-core-user-3.4.5/peek_core_user/_private/ldap_auth/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/ldap_auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11154 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/ldap_auth/ldap_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.286076 peek-core-user-3.4.5/peek_core_user/_private/server/
--rw-r--r--   0 root         (0) root         (0)     2010 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/AdminTupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)      593 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/ClientTupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     2185 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/ClientTupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)     7217 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/PluginLogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.286076 peek-core-user-3.4.5/peek_core_user/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)     1810 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/admin_backend/InternalGroupTableHandler.py
--rw-r--r--   0 root         (0) root         (0)     4037 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/admin_backend/InternalUserTableHandler.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/admin_backend/LdapSettingsHandler.py
--rw-r--r--   0 root         (0) root         (0)     2234 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/admin_backend/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)      836 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.286076 peek-core-user-3.4.5/peek_core_user/_private/server/admin_tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     2875 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/admin_tuple_providers/LoggedInUserStatusTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/admin_tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.287077 peek-core-user-3.4.5/peek_core_user/_private/server/api/
--rw-r--r--   0 root         (0) root         (0)      714 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/api/UserAdminAuthApi.py
--rw-r--r--   0 root         (0) root         (0)     2573 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/api/UserApi.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/api/UserFieldHookApi.py
--rw-r--r--   0 root         (0) root         (0)      991 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/api/UserImportApi.py
--rw-r--r--   0 root         (0) root         (0)     8974 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/api/UserInfoApi.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/api/UserLoginApi.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.287077 peek-core-user-3.4.5/peek_core_user/_private/server/auth_connectors/
--rw-r--r--   0 root         (0) root         (0)     2835 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/auth_connectors/AuthABC.py
--rw-r--r--   0 root         (0) root         (0)     5088 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/auth_connectors/InternalAuth.py
--rw-r--r--   0 root         (0) root         (0)     9769 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/auth_connectors/LdapAuth.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/auth_connectors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.287077 peek-core-user-3.4.5/peek_core_user/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)     2104 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/controller/AdminAuthController.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/controller/ImportController.py
--rw-r--r--   0 root         (0) root         (0)    18854 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/controller/LoginLogoutController.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/controller/PasswordUpdateController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.288076 peek-core-user-3.4.5/peek_core_user/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)      965 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/tuple_providers/GroupDetailTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/tuple_providers/UserListItemTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     2274 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/tuple_providers/UserLoggedInTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1394 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/tuple_providers/UserLoginUiSettingTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.288076 peek-core-user-3.4.5/peek_core_user/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      937 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     1191 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/storage/DirectoryTuple.py
--rw-r--r--   0 root         (0) root         (0)     1032 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/storage/InternalGroupTuple.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/storage/InternalUserGroupTuple.py
--rw-r--r--   0 root         (0) root         (0)     1290 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/storage/InternalUserPassword.py
--rw-r--r--   0 root         (0) root         (0)     2377 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/storage/InternalUserTuple.py
--rw-r--r--   0 root         (0) root         (0)     1269 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/storage/LdapSetting.py
--rw-r--r--   0 root         (0) root         (0)     9046 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/storage/UserLoggedIn.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.289076 peek-core-user-3.4.5/peek_core_user/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      536 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/tuples/InternalGroupImportResultTuple.py
--rw-r--r--   0 root         (0) root         (0)      534 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/tuples/InternalUserImportResultTuple.py
--rw-r--r--   0 root         (0) root         (0)      447 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/tuples/InternalUserUpdatePasswordAction.py
--rw-r--r--   0 root         (0) root         (0)      696 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/tuples/LdapLoggedInUserTuple.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/tuples/LoggedInUserStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/tuples/UserLoggedInTuple.py
--rw-r--r--   0 root         (0) root         (0)      504 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/tuples/UserLoginUiSettingTuple.py
--rw-r--r--   0 root         (0) root         (0)      175 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.289076 peek-core-user-3.4.5/peek_core_user/_private/worker/
--rw-r--r--   0 root         (0) root         (0)      972 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/worker/WorkerEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/worker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.289076 peek-core-user-3.4.5/peek_core_user/_private/worker/tasks/
--rw-r--r--   0 root         (0) root         (0)     3590 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/worker/tasks/UserImportInternalGroupTask.py
--rw-r--r--   0 root         (0) root         (0)     6341 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/worker/tasks/UserImportInternalUserTask.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/_private/worker/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.289076 peek-core-user-3.4.5/peek_core_user/admin-doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.290077 peek-core-user-3.4.5/peek_core_user/admin-doc/configuration/
--rw-r--r--   0 root         (0) root         (0)    64196 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/admin-doc/configuration/add_group.png
--rw-r--r--   0 root         (0) root         (0)    88232 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/admin-doc/configuration/add_user.png
--rw-r--r--   0 root         (0) root         (0)     4375 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/admin-doc/configuration/configuration.rst
--rw-r--r--   0 root         (0) root         (0)    57815 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/admin-doc/configuration/edit-internal-groups.png
--rw-r--r--   0 root         (0) root         (0)    77342 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/admin-doc/configuration/edit-internal-user.png
--rw-r--r--   0 root         (0) root         (0)    64921 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/admin-doc/configuration/settings-general.png
--rw-r--r--   0 root         (0) root         (0)    45579 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/admin-doc/configuration/settings-ldap.png
--rw-r--r--   0 root         (0) root         (0)      256 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/admin-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.290077 peek-core-user-3.4.5/peek_core_user/admin-doc/logged_in/
--rw-r--r--   0 root         (0) root         (0)      817 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/admin-doc/logged_in/logged_in.rst
--rw-r--r--   0 root         (0) root         (0)    57636 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/admin-doc/logged_in/logout_user.png
--rw-r--r--   0 root         (0) root         (0)    22311 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/admin-doc/logged_in/logout_yes.png
--rw-r--r--   0 root         (0) root         (0)    56963 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/admin-doc/logged_in/manage-logged-in-users.png
--rw-r--r--   0 root         (0) root         (0)      742 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/admin-doc/overview.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.290077 peek-core-user-3.4.5/peek_core_user/both-doc/
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/both-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)    16799 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/both-doc/login.png
--rw-r--r--   0 root         (0) root         (0)    12482 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/both-doc/login_logout.png
--rwxr-xr-x   0 root         (0) root         (0)      901 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/both-doc/login_logout.rst
--rwxr-xr-x   0 root         (0) root         (0)     1171 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/both-doc/user_button.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.290077 peek-core-user-3.4.5/peek_core_user/plugin-module/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.290077 peek-core-user-3.4.5/peek_core_user/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)      307 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/_private/PluginNames.ts
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.291077 peek-core-user-3.4.5/peek_core_user/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      952 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/_private/tuples/LoggedInUserStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      691 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/_private/tuples/UserLoggedInTuple.ts
--rw-r--r--   0 root         (0) root         (0)     2655 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/_private/user-tuple.service.ts
--rw-r--r--   0 root         (0) root         (0)      762 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/index.ts
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.291077 peek-core-user-3.4.5/peek_core_user/plugin-module/services/
--rw-r--r--   0 root         (0) root         (0)      836 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/services/logged-in.guard.ts
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/services/logged-out.guard.ts
--rw-r--r--   0 root         (0) root         (0)      491 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/services/profile.service.ts
--rw-r--r--   0 root         (0) root         (0)    10343 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/services/user.service.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.291077 peek-core-user-3.4.5/peek_core_user/plugin-module/tuples/
--rw-r--r--   0 root         (0) root         (0)      483 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/tuples/GroupDetailTuple.ts
--rw-r--r--   0 root         (0) root         (0)      867 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/tuples/UserDetailTuple.ts
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/tuples/UserListItemTuple.ts
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/tuples/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.291077 peek-core-user-3.4.5/peek_core_user/plugin-module/tuples/login/
--rw-r--r--   0 root         (0) root         (0)      722 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/tuples/login/UserLoginAction.ts
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/tuples/login/UserLoginResponseTuple.ts
--rw-r--r--   0 root         (0) root         (0)      671 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/tuples/login/UserLogoutAction.ts
--rw-r--r--   0 root         (0) root         (0)      894 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/plugin-module/tuples/login/UserLogoutResponseTuple.ts
--rw-r--r--   0 root         (0) root         (0)     2718 2023-06-28 07:26:33.000000 peek-core-user-3.4.5/peek_core_user/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.292076 peek-core-user-3.4.5/peek_core_user/server/
--rw-r--r--   0 root         (0) root         (0)      354 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/server/UserAdminAuthApiABC.py
--rw-r--r--   0 root         (0) root         (0)     2108 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/server/UserApiABC.py
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/server/UserDbErrors.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/server/UserFieldHookApiABC.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/server/UserImportApiABC.py
--rw-r--r--   0 root         (0) root         (0)     3782 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/server/UserInfoApiABC.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/server/UserLoginApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.292076 peek-core-user-3.4.5/peek_core_user/tuples/
--rw-r--r--   0 root         (0) root         (0)      668 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/DeviceWithUserDetails.py
--rw-r--r--   0 root         (0) root         (0)      436 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/GroupDetailTuple.py
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/UserAuthTarget.py
--rw-r--r--   0 root         (0) root         (0)     1185 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/UserDetailTuple.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/UserListItemTuple.py
--rw-r--r--   0 root         (0) root         (0)      518 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/UserLoggedInInfoTuple.py
--rw-r--r--   0 root         (0) root         (0)      274 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.292076 peek-core-user-3.4.5/peek_core_user/tuples/constants/
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/constants/UserAuthTargetEnum.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/constants/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.292076 peek-core-user-3.4.5/peek_core_user/tuples/import_/
--rw-r--r--   0 root         (0) root         (0)      450 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/import_/ImportInternalGroupTuple.py
--rw-r--r--   0 root         (0) root         (0)     1123 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/import_/ImportInternalUserTuple.py
--rw-r--r--   0 root         (0) root         (0)      168 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/import_/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.293077 peek-core-user-3.4.5/peek_core_user/tuples/login/
--rw-r--r--   0 root         (0) root         (0)      715 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/login/UserLoginAction.py
--rw-r--r--   0 root         (0) root         (0)     1163 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/login/UserLoginResponseTuple.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/login/UserLogoutAction.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/login/UserLogoutResponseTuple.py
--rw-r--r--   0 root         (0) root         (0)      168 2023-06-28 07:25:23.000000 peek-core-user-3.4.5/peek_core_user/tuples/login/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:33.282076 peek-core-user-3.4.5/peek_core_user.egg-info/
--rw-r--r--   0 root         (0) root         (0)      376 2023-06-28 07:26:33.000000 peek-core-user-3.4.5/peek_core_user.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11383 2023-06-28 07:26:33.000000 peek-core-user-3.4.5/peek_core_user.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:26:33.000000 peek-core-user-3.4.5/peek_core_user.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:26:33.000000 peek-core-user-3.4.5/peek_core_user.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-28 07:26:33.000000 peek-core-user-3.4.5/peek_core_user.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-28 07:26:33.000000 peek-core-user-3.4.5/peek_core_user.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:26:33.293077 peek-core-user-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2703 2023-06-28 07:26:33.000000 peek-core-user-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.019406 peek-core-user-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      376 2023-06-29 10:20:23.019406 peek-core-user-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      293 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.008406 peek-core-user-3.4.6/peek_core_user/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)      271 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/TempUnitTest.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-06-29 10:20:22.000000 peek-core-user-3.4.6/peek_core_user/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.009406 peek-core-user-3.4.6/peek_core_user/_private/
+-rw-r--r--   0 root         (0) root         (0)      183 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.009406 peek-core-user-3.4.6/peek_core_user/_private/admin-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.009406 peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-internal-group-table/
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-internal-group-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     2063 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-internal-group-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.009406 peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-internal-user-table/
+-rw-r--r--   0 root         (0) root         (0)     5971 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-internal-user-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     4802 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-internal-user-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.009406 peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-ldap-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     4398 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-ldap-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-ldap-setting-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.009406 peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     1828 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-setting-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.009406 peek-core-user-3.4.6/peek_core_user/_private/admin-app/logged-in-user/
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/logged-in-user/logged-in-user.component.html
+-rw-r--r--   0 root         (0) root         (0)     3419 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/logged-in-user/logged-in-user.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.010406 peek-core-user-3.4.6/peek_core_user/_private/admin-app/tuples/
+-rw-r--r--   0 root         (0) root         (0)      527 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/tuples/InternalGroupTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      996 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/tuples/InternalUserTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      541 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/tuples/InternalUserUpdatePasswordAction.ts
+-rw-r--r--   0 root         (0) root         (0)      646 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/tuples/LdapSettingTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      580 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/tuples/SettingPropertyTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.010406 peek-core-user-3.4.6/peek_core_user/_private/admin-app/tuples/constants/
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/tuples/constants/UserAuthTargetEnum.ts
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/user.component.html
+-rw-r--r--   0 root         (0) root         (0)      158 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/user.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2998 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/admin-app/user.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.010406 peek-core-user-3.4.6/peek_core_user/_private/agent/
+-rw-r--r--   0 root         (0) root         (0)      847 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/agent/AgentEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/agent/RpcForLogic.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.010406 peek-core-user-3.4.6/peek_core_user/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      299 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.011406 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     4602 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/0498d92479c8_implemented_internal_directory.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/1176bc54abf3_added_foreign_key_to_user_logged_in.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/2209cf338e6d_added_ldap_table.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/2c6728ebc562_separated_password.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/3a9cddaf05e5_added_settings_table.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/3fd59734e444_removed_string_limits.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/3fec57d8da58_initial.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/43df0e05c728_added_user_import_source.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/45c62f8acd87_added_vehical_to_loggedin.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/56d805072d2a_added_importhash.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/5e33c6b788fd_removed_unique_logged_in_user.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/73d65f042834_removed_foreign_key_from_user_logged_in.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/7e3f668edf0e_updated_settings.py
+-rw-r--r--   0 root         (0) root         (0)      663 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/9b65be31926e_timezone_aware.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2664 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/b09fe7b3b31b_add_userkey.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/d03db0fcb600_convert_userkey_and_username_to_all_.py
+-rw-r--r--   0 root         (0) root         (0)      829 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/d79da9333e2a_drop_internaluser_rows_from_ldap_for_useruuid_change.py
+-rw-r--r--   0 root         (0) root         (0)      756 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/eef485ef2e0e_added_agenturi_column_to_ldapsetting.py
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.011406 peek-core-user-3.4.6/peek_core_user/_private/both-app/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/both-app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      779 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/both-app/plugin-user.module.ts
+-rw-r--r--   0 root         (0) root         (0)      667 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/both-app/plugin-user.routes.ts
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/both-app/plugin-user.text.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.011406 peek-core-user-3.4.6/peek_core_user/_private/both-app/scss/
+-rw-r--r--   0 root         (0) root         (0)      560 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/both-app/scss/plugin-user.dweb.scss
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/both-app/scss/plugin-user.mweb.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.011406 peek-core-user-3.4.6/peek_core_user/_private/both-app/tuples/
+-rw-r--r--   0 root         (0) root         (0)      557 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/both-app/tuples/UserLoginUiSettingTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.012406 peek-core-user-3.4.6/peek_core_user/_private/both-app/user-login/
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/both-app/user-login/user-login.component.dweb.html
+-rw-r--r--   0 root         (0) root         (0)     3209 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/both-app/user-login/user-login.component.mweb.html
+-rw-r--r--   0 root         (0) root         (0)     6145 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/both-app/user-login/user-login.component.ts
+-rw-r--r--   0 root         (0) root         (0)      502 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/both-app/user-login/user-login.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.012406 peek-core-user-3.4.6/peek_core_user/_private/both-app/user-logout/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/both-app/user-logout/user-logout.component.dweb.html
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/both-app/user-logout/user-logout.component.mweb.html
+-rw-r--r--   0 root         (0) root         (0)     2990 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/both-app/user-logout/user-logout.component.ts
+-rw-r--r--   0 root         (0) root         (0)      507 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/both-app/user-logout/user-logout.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.012406 peek-core-user-3.4.6/peek_core_user/_private/both-assets/
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/both-assets/plugin_icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.012406 peek-core-user-3.4.6/peek_core_user/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/client/PluginClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      474 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/client/TupleActionProcessorProxy.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/client/TupleDataObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.012406 peek-core-user-3.4.6/peek_core_user/_private/ldap_auth/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/ldap_auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11154 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/ldap_auth/ldap_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.012406 peek-core-user-3.4.6/peek_core_user/_private/server/
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/AdminTupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)      593 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/ClientTupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     2185 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/ClientTupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)     7217 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/PluginLogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.013406 peek-core-user-3.4.6/peek_core_user/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/admin_backend/InternalGroupTableHandler.py
+-rw-r--r--   0 root         (0) root         (0)     4037 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/admin_backend/InternalUserTableHandler.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/admin_backend/LdapSettingsHandler.py
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/admin_backend/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)      836 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.013406 peek-core-user-3.4.6/peek_core_user/_private/server/admin_tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     2875 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/admin_tuple_providers/LoggedInUserStatusTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/admin_tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.013406 peek-core-user-3.4.6/peek_core_user/_private/server/api/
+-rw-r--r--   0 root         (0) root         (0)      714 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/api/UserAdminAuthApi.py
+-rw-r--r--   0 root         (0) root         (0)     2573 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/api/UserApi.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/api/UserFieldHookApi.py
+-rw-r--r--   0 root         (0) root         (0)      991 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/api/UserImportApi.py
+-rw-r--r--   0 root         (0) root         (0)     8974 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/api/UserInfoApi.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/api/UserLoginApi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.013406 peek-core-user-3.4.6/peek_core_user/_private/server/auth_connectors/
+-rw-r--r--   0 root         (0) root         (0)     2835 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/auth_connectors/AuthABC.py
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/auth_connectors/InternalAuth.py
+-rw-r--r--   0 root         (0) root         (0)     9769 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/auth_connectors/LdapAuth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/auth_connectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.014406 peek-core-user-3.4.6/peek_core_user/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/controller/AdminAuthController.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/controller/ImportController.py
+-rw-r--r--   0 root         (0) root         (0)    18854 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/controller/LoginLogoutController.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/controller/PasswordUpdateController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.014406 peek-core-user-3.4.6/peek_core_user/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)      965 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/tuple_providers/GroupDetailTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/tuple_providers/UserListItemTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/tuple_providers/UserLoggedInTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1394 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/tuple_providers/UserLoginUiSettingTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.015406 peek-core-user-3.4.6/peek_core_user/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      937 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/storage/DirectoryTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/storage/InternalGroupTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/storage/InternalUserGroupTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1290 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/storage/InternalUserPassword.py
+-rw-r--r--   0 root         (0) root         (0)     2377 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/storage/InternalUserTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/storage/LdapSetting.py
+-rw-r--r--   0 root         (0) root         (0)     9046 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/storage/UserLoggedIn.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.015406 peek-core-user-3.4.6/peek_core_user/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      536 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/tuples/InternalGroupImportResultTuple.py
+-rw-r--r--   0 root         (0) root         (0)      534 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/tuples/InternalUserImportResultTuple.py
+-rw-r--r--   0 root         (0) root         (0)      447 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/tuples/InternalUserUpdatePasswordAction.py
+-rw-r--r--   0 root         (0) root         (0)      696 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/tuples/LdapLoggedInUserTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/tuples/LoggedInUserStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/tuples/UserLoggedInTuple.py
+-rw-r--r--   0 root         (0) root         (0)      504 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/tuples/UserLoginUiSettingTuple.py
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.015406 peek-core-user-3.4.6/peek_core_user/_private/worker/
+-rw-r--r--   0 root         (0) root         (0)      972 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/worker/WorkerEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/worker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.015406 peek-core-user-3.4.6/peek_core_user/_private/worker/tasks/
+-rw-r--r--   0 root         (0) root         (0)     3590 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/worker/tasks/UserImportInternalGroupTask.py
+-rw-r--r--   0 root         (0) root         (0)     6341 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/worker/tasks/UserImportInternalUserTask.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/_private/worker/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.015406 peek-core-user-3.4.6/peek_core_user/admin-doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.016406 peek-core-user-3.4.6/peek_core_user/admin-doc/configuration/
+-rw-r--r--   0 root         (0) root         (0)    64196 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/admin-doc/configuration/add_group.png
+-rw-r--r--   0 root         (0) root         (0)    88232 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/admin-doc/configuration/add_user.png
+-rw-r--r--   0 root         (0) root         (0)     4375 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/admin-doc/configuration/configuration.rst
+-rw-r--r--   0 root         (0) root         (0)    57815 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/admin-doc/configuration/edit-internal-groups.png
+-rw-r--r--   0 root         (0) root         (0)    77342 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/admin-doc/configuration/edit-internal-user.png
+-rw-r--r--   0 root         (0) root         (0)    64921 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/admin-doc/configuration/settings-general.png
+-rw-r--r--   0 root         (0) root         (0)    45579 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/admin-doc/configuration/settings-ldap.png
+-rw-r--r--   0 root         (0) root         (0)      256 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/admin-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.016406 peek-core-user-3.4.6/peek_core_user/admin-doc/logged_in/
+-rw-r--r--   0 root         (0) root         (0)      817 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/admin-doc/logged_in/logged_in.rst
+-rw-r--r--   0 root         (0) root         (0)    57636 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/admin-doc/logged_in/logout_user.png
+-rw-r--r--   0 root         (0) root         (0)    22311 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/admin-doc/logged_in/logout_yes.png
+-rw-r--r--   0 root         (0) root         (0)    56963 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/admin-doc/logged_in/manage-logged-in-users.png
+-rw-r--r--   0 root         (0) root         (0)      742 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/admin-doc/overview.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.016406 peek-core-user-3.4.6/peek_core_user/both-doc/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/both-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)    16799 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/both-doc/login.png
+-rw-r--r--   0 root         (0) root         (0)    12482 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/both-doc/login_logout.png
+-rwxr-xr-x   0 root         (0) root         (0)      901 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/both-doc/login_logout.rst
+-rwxr-xr-x   0 root         (0) root         (0)     1171 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/both-doc/user_button.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.017406 peek-core-user-3.4.6/peek_core_user/plugin-module/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.017406 peek-core-user-3.4.6/peek_core_user/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)      307 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/_private/PluginNames.ts
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.017406 peek-core-user-3.4.6/peek_core_user/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/_private/tuples/LoggedInUserStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      691 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/_private/tuples/UserLoggedInTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/_private/user-tuple.service.ts
+-rw-r--r--   0 root         (0) root         (0)      762 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/index.ts
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.017406 peek-core-user-3.4.6/peek_core_user/plugin-module/services/
+-rw-r--r--   0 root         (0) root         (0)      836 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/services/logged-in.guard.ts
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/services/logged-out.guard.ts
+-rw-r--r--   0 root         (0) root         (0)      491 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/services/profile.service.ts
+-rw-r--r--   0 root         (0) root         (0)    10343 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/services/user.service.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.017406 peek-core-user-3.4.6/peek_core_user/plugin-module/tuples/
+-rw-r--r--   0 root         (0) root         (0)      483 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/tuples/GroupDetailTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      867 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/tuples/UserDetailTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/tuples/UserListItemTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/tuples/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.017406 peek-core-user-3.4.6/peek_core_user/plugin-module/tuples/login/
+-rw-r--r--   0 root         (0) root         (0)      722 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/tuples/login/UserLoginAction.ts
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/tuples/login/UserLoginResponseTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      671 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/tuples/login/UserLogoutAction.ts
+-rw-r--r--   0 root         (0) root         (0)      894 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/plugin-module/tuples/login/UserLogoutResponseTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-06-29 10:20:22.000000 peek-core-user-3.4.6/peek_core_user/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.018406 peek-core-user-3.4.6/peek_core_user/server/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/server/UserAdminAuthApiABC.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/server/UserApiABC.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/server/UserDbErrors.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/server/UserFieldHookApiABC.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/server/UserImportApiABC.py
+-rw-r--r--   0 root         (0) root         (0)     3782 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/server/UserInfoApiABC.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/server/UserLoginApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.018406 peek-core-user-3.4.6/peek_core_user/tuples/
+-rw-r--r--   0 root         (0) root         (0)      668 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/DeviceWithUserDetails.py
+-rw-r--r--   0 root         (0) root         (0)      436 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/GroupDetailTuple.py
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/UserAuthTarget.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/UserDetailTuple.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/UserListItemTuple.py
+-rw-r--r--   0 root         (0) root         (0)      518 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/UserLoggedInInfoTuple.py
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.018406 peek-core-user-3.4.6/peek_core_user/tuples/constants/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/constants/UserAuthTargetEnum.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/constants/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.019406 peek-core-user-3.4.6/peek_core_user/tuples/import_/
+-rw-r--r--   0 root         (0) root         (0)      450 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/import_/ImportInternalGroupTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/import_/ImportInternalUserTuple.py
+-rw-r--r--   0 root         (0) root         (0)      168 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/import_/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.019406 peek-core-user-3.4.6/peek_core_user/tuples/login/
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/login/UserLoginAction.py
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/login/UserLoginResponseTuple.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/login/UserLogoutAction.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/login/UserLogoutResponseTuple.py
+-rw-r--r--   0 root         (0) root         (0)      168 2023-06-29 10:19:14.000000 peek-core-user-3.4.6/peek_core_user/tuples/login/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:23.008406 peek-core-user-3.4.6/peek_core_user.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      376 2023-06-29 10:20:22.000000 peek-core-user-3.4.6/peek_core_user.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11383 2023-06-29 10:20:22.000000 peek-core-user-3.4.6/peek_core_user.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:20:22.000000 peek-core-user-3.4.6/peek_core_user.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:20:22.000000 peek-core-user-3.4.6/peek_core_user.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-29 10:20:22.000000 peek-core-user-3.4.6/peek_core_user.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-29 10:20:22.000000 peek-core-user-3.4.6/peek_core_user.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:20:23.019406 peek-core-user-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-06-29 10:20:22.000000 peek-core-user-3.4.6/setup.py
```

### Comparing `peek-core-user-3.4.5/peek_core_user/__init__.py` & `peek-core-user-3.4.6/peek_core_user/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Type
 
 from peek_plugin_base.agent.PluginAgentEntryHookABC import PluginAgentEntryHookABC
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 from peek_plugin_base.worker.PluginWorkerEntryHookABC import PluginWorkerEntryHookABC
 
-__version__ = '3.4.5'
+__version__ = '3.4.6'
 
 
 def peekFieldEntryHook() -> Type[PluginClientEntryHookABC]:
     from peek_core_user._private.client.PluginClientEntryHook import (
         PluginClientEntryHook,
     )
```

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-internal-group-table/edit.component.html` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-internal-group-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-internal-group-table/edit.component.ts` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-internal-group-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-internal-user-table/edit.component.html` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-internal-user-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-internal-user-table/edit.component.ts` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-internal-user-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-ldap-setting-table/edit.component.html` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-ldap-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-ldap-setting-table/edit.component.ts` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-ldap-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-setting-table/edit.component.html` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/logged-in-user/logged-in-user.component.html` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/logged-in-user/logged-in-user.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/logged-in-user/logged-in-user.component.ts` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/logged-in-user/logged-in-user.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/tuples/InternalGroupTuple.ts` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/tuples/InternalGroupTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/tuples/InternalUserTuple.ts` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/tuples/InternalUserTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/tuples/InternalUserUpdatePasswordAction.ts` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/tuples/InternalUserUpdatePasswordAction.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/tuples/LdapSettingTuple.ts` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/tuples/LdapSettingTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/tuples/SettingPropertyTuple.ts` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/tuples/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/user.component.html` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/user.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/admin-app/user.module.ts` & `peek-core-user-3.4.6/peek_core_user/_private/admin-app/user.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/agent/AgentEntryHook.py` & `peek-core-user-3.4.6/peek_core_user/_private/agent/AgentEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/agent/RpcForLogic.py` & `peek-core-user-3.4.6/peek_core_user/_private/agent/RpcForLogic.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/script.py.mako` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/0498d92479c8_implemented_internal_directory.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/0498d92479c8_implemented_internal_directory.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/1176bc54abf3_added_foreign_key_to_user_logged_in.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/1176bc54abf3_added_foreign_key_to_user_logged_in.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/2209cf338e6d_added_ldap_table.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/2209cf338e6d_added_ldap_table.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/2c6728ebc562_separated_password.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/2c6728ebc562_separated_password.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/3a9cddaf05e5_added_settings_table.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/3a9cddaf05e5_added_settings_table.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/3fd59734e444_removed_string_limits.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/3fd59734e444_removed_string_limits.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/3fec57d8da58_initial.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/3fec57d8da58_initial.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/43df0e05c728_added_user_import_source.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/43df0e05c728_added_user_import_source.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/45c62f8acd87_added_vehical_to_loggedin.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/45c62f8acd87_added_vehical_to_loggedin.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/56d805072d2a_added_importhash.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/56d805072d2a_added_importhash.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/5e33c6b788fd_removed_unique_logged_in_user.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/5e33c6b788fd_removed_unique_logged_in_user.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/73d65f042834_removed_foreign_key_from_user_logged_in.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/73d65f042834_removed_foreign_key_from_user_logged_in.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/7e3f668edf0e_updated_settings.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/7e3f668edf0e_updated_settings.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/9b65be31926e_timezone_aware.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/9b65be31926e_timezone_aware.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/b09fe7b3b31b_add_userkey.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/b09fe7b3b31b_add_userkey.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/d03db0fcb600_convert_userkey_and_username_to_all_.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/d03db0fcb600_convert_userkey_and_username_to_all_.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/d79da9333e2a_drop_internaluser_rows_from_ldap_for_useruuid_change.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/d79da9333e2a_drop_internaluser_rows_from_ldap_for_useruuid_change.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/alembic/versions/eef485ef2e0e_added_agenturi_column_to_ldapsetting.py` & `peek-core-user-3.4.6/peek_core_user/_private/alembic/versions/eef485ef2e0e_added_agenturi_column_to_ldapsetting.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/both-app/plugin-user.module.ts` & `peek-core-user-3.4.6/peek_core_user/_private/both-app/plugin-user.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/both-app/plugin-user.routes.ts` & `peek-core-user-3.4.6/peek_core_user/_private/both-app/plugin-user.routes.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/both-app/scss/plugin-user.dweb.scss` & `peek-core-user-3.4.6/peek_core_user/_private/both-app/scss/plugin-user.dweb.scss`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/both-app/scss/plugin-user.mweb.scss` & `peek-core-user-3.4.6/peek_core_user/_private/both-app/scss/plugin-user.mweb.scss`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/both-app/tuples/UserLoginUiSettingTuple.ts` & `peek-core-user-3.4.6/peek_core_user/_private/both-app/tuples/UserLoginUiSettingTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/both-app/user-login/user-login.component.dweb.html` & `peek-core-user-3.4.6/peek_core_user/_private/both-app/user-login/user-login.component.dweb.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/both-app/user-login/user-login.component.mweb.html` & `peek-core-user-3.4.6/peek_core_user/_private/both-app/user-login/user-login.component.mweb.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/both-app/user-login/user-login.component.ts` & `peek-core-user-3.4.6/peek_core_user/_private/both-app/user-login/user-login.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/both-app/user-logout/user-logout.component.dweb.html` & `peek-core-user-3.4.6/peek_core_user/_private/both-app/user-logout/user-logout.component.dweb.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/both-app/user-logout/user-logout.component.mweb.html` & `peek-core-user-3.4.6/peek_core_user/_private/both-app/user-logout/user-logout.component.mweb.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/both-app/user-logout/user-logout.component.ts` & `peek-core-user-3.4.6/peek_core_user/_private/both-app/user-logout/user-logout.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/both-assets/plugin_icon.png` & `peek-core-user-3.4.6/peek_core_user/_private/both-assets/plugin_icon.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/client/PluginClientEntryHook.py` & `peek-core-user-3.4.6/peek_core_user/_private/client/PluginClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/ldap_auth/ldap_auth.py` & `peek-core-user-3.4.6/peek_core_user/_private/ldap_auth/ldap_auth.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/AdminTupleDataObservable.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/AdminTupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/ClientTupleActionProcessor.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/ClientTupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/ClientTupleDataObservable.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/ClientTupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/PluginLogicEntryHook.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/PluginLogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/admin_backend/InternalGroupTableHandler.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/admin_backend/InternalGroupTableHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/admin_backend/InternalUserTableHandler.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/admin_backend/InternalUserTableHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/admin_backend/LdapSettingsHandler.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/admin_backend/LdapSettingsHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/admin_backend/SettingPropertyHandler.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/admin_backend/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/admin_backend/__init__.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/admin_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/admin_tuple_providers/LoggedInUserStatusTupleProvider.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/admin_tuple_providers/LoggedInUserStatusTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/api/UserAdminAuthApi.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/api/UserAdminAuthApi.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/api/UserApi.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/api/UserApi.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/api/UserFieldHookApi.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/api/UserFieldHookApi.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/api/UserImportApi.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/api/UserImportApi.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/api/UserInfoApi.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/api/UserInfoApi.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/api/UserLoginApi.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/api/UserLoginApi.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/auth_connectors/AuthABC.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/auth_connectors/AuthABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/auth_connectors/InternalAuth.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/auth_connectors/InternalAuth.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/auth_connectors/LdapAuth.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/auth_connectors/LdapAuth.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/controller/AdminAuthController.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/controller/AdminAuthController.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/controller/ImportController.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/controller/ImportController.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/controller/LoginLogoutController.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/controller/LoginLogoutController.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/controller/MainController.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/controller/PasswordUpdateController.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/controller/PasswordUpdateController.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/tuple_providers/GroupDetailTupleProvider.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/tuple_providers/GroupDetailTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/tuple_providers/UserListItemTupleProvider.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/tuple_providers/UserListItemTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/tuple_providers/UserLoggedInTupleProvider.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/tuple_providers/UserLoggedInTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/server/tuple_providers/UserLoginUiSettingTupleProvider.py` & `peek-core-user-3.4.6/peek_core_user/_private/server/tuple_providers/UserLoginUiSettingTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/storage/DeclarativeBase.py` & `peek-core-user-3.4.6/peek_core_user/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/storage/DirectoryTuple.py` & `peek-core-user-3.4.6/peek_core_user/_private/storage/DirectoryTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/storage/InternalGroupTuple.py` & `peek-core-user-3.4.6/peek_core_user/_private/storage/InternalGroupTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/storage/InternalUserGroupTuple.py` & `peek-core-user-3.4.6/peek_core_user/_private/storage/InternalUserGroupTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/storage/InternalUserPassword.py` & `peek-core-user-3.4.6/peek_core_user/_private/storage/InternalUserPassword.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/storage/InternalUserTuple.py` & `peek-core-user-3.4.6/peek_core_user/_private/storage/InternalUserTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/storage/LdapSetting.py` & `peek-core-user-3.4.6/peek_core_user/_private/storage/LdapSetting.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/storage/Setting.py` & `peek-core-user-3.4.6/peek_core_user/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/storage/UserLoggedIn.py` & `peek-core-user-3.4.6/peek_core_user/_private/storage/UserLoggedIn.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/tuples/InternalGroupImportResultTuple.py` & `peek-core-user-3.4.6/peek_core_user/_private/tuples/InternalGroupImportResultTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/tuples/InternalUserImportResultTuple.py` & `peek-core-user-3.4.6/peek_core_user/_private/tuples/InternalUserImportResultTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/tuples/LdapLoggedInUserTuple.py` & `peek-core-user-3.4.6/peek_core_user/_private/tuples/LdapLoggedInUserTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/tuples/LoggedInUserStatusTuple.py` & `peek-core-user-3.4.6/peek_core_user/_private/tuples/LoggedInUserStatusTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/tuples/UserLoggedInTuple.py` & `peek-core-user-3.4.6/peek_core_user/_private/tuples/UserLoggedInTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/worker/WorkerEntryHook.py` & `peek-core-user-3.4.6/peek_core_user/_private/worker/WorkerEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/worker/tasks/UserImportInternalGroupTask.py` & `peek-core-user-3.4.6/peek_core_user/_private/worker/tasks/UserImportInternalGroupTask.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/_private/worker/tasks/UserImportInternalUserTask.py` & `peek-core-user-3.4.6/peek_core_user/_private/worker/tasks/UserImportInternalUserTask.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/admin-doc/configuration/add_group.png` & `peek-core-user-3.4.6/peek_core_user/admin-doc/configuration/add_group.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/admin-doc/configuration/add_user.png` & `peek-core-user-3.4.6/peek_core_user/admin-doc/configuration/add_user.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/admin-doc/configuration/configuration.rst` & `peek-core-user-3.4.6/peek_core_user/admin-doc/configuration/configuration.rst`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/admin-doc/configuration/edit-internal-groups.png` & `peek-core-user-3.4.6/peek_core_user/admin-doc/configuration/edit-internal-groups.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/admin-doc/configuration/edit-internal-user.png` & `peek-core-user-3.4.6/peek_core_user/admin-doc/configuration/edit-internal-user.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/admin-doc/configuration/settings-general.png` & `peek-core-user-3.4.6/peek_core_user/admin-doc/configuration/settings-general.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/admin-doc/configuration/settings-ldap.png` & `peek-core-user-3.4.6/peek_core_user/admin-doc/configuration/settings-ldap.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/admin-doc/logged_in/logged_in.rst` & `peek-core-user-3.4.6/peek_core_user/admin-doc/logged_in/logged_in.rst`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/admin-doc/logged_in/logout_user.png` & `peek-core-user-3.4.6/peek_core_user/admin-doc/logged_in/logout_user.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/admin-doc/logged_in/logout_yes.png` & `peek-core-user-3.4.6/peek_core_user/admin-doc/logged_in/logout_yes.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/admin-doc/logged_in/manage-logged-in-users.png` & `peek-core-user-3.4.6/peek_core_user/admin-doc/logged_in/manage-logged-in-users.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/admin-doc/overview.rst` & `peek-core-user-3.4.6/peek_core_user/admin-doc/overview.rst`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/both-doc/login.png` & `peek-core-user-3.4.6/peek_core_user/both-doc/login.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/both-doc/login_logout.png` & `peek-core-user-3.4.6/peek_core_user/both-doc/login_logout.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/both-doc/login_logout.rst` & `peek-core-user-3.4.6/peek_core_user/both-doc/login_logout.rst`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/both-doc/user_button.png` & `peek-core-user-3.4.6/peek_core_user/both-doc/user_button.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/plugin-module/_private/tuples/LoggedInUserStatusTuple.ts` & `peek-core-user-3.4.6/peek_core_user/plugin-module/_private/tuples/LoggedInUserStatusTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/plugin-module/_private/tuples/UserLoggedInTuple.ts` & `peek-core-user-3.4.6/peek_core_user/plugin-module/_private/tuples/UserLoggedInTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/plugin-module/_private/user-tuple.service.ts` & `peek-core-user-3.4.6/peek_core_user/plugin-module/_private/user-tuple.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/plugin-module/index.ts` & `peek-core-user-3.4.6/peek_core_user/plugin-module/index.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/plugin-module/services/logged-in.guard.ts` & `peek-core-user-3.4.6/peek_core_user/plugin-module/services/logged-in.guard.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/plugin-module/services/user.service.ts` & `peek-core-user-3.4.6/peek_core_user/plugin-module/services/user.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/plugin-module/tuples/UserDetailTuple.ts` & `peek-core-user-3.4.6/peek_core_user/plugin-module/tuples/UserDetailTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/plugin-module/tuples/UserListItemTuple.ts` & `peek-core-user-3.4.6/peek_core_user/plugin-module/tuples/UserListItemTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/plugin-module/tuples/login/UserLoginAction.ts` & `peek-core-user-3.4.6/peek_core_user/plugin-module/tuples/login/UserLoginAction.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/plugin-module/tuples/login/UserLoginResponseTuple.ts` & `peek-core-user-3.4.6/peek_core_user/plugin-module/tuples/login/UserLoginResponseTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/plugin-module/tuples/login/UserLogoutAction.ts` & `peek-core-user-3.4.6/peek_core_user/plugin-module/tuples/login/UserLogoutAction.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/plugin-module/tuples/login/UserLogoutResponseTuple.ts` & `peek-core-user-3.4.6/peek_core_user/plugin-module/tuples/login/UserLogoutResponseTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/plugin_package.json` & `peek-core-user-3.4.6/peek_core_user/plugin_package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967532467532468%*

 * *Differences: {"'plugin'": "{'version': '3.4.6'}"}*

```diff
@@ -74,15 +74,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_core_user",
         "title": "Users",
-        "version": "3.4.5",
+        "version": "3.4.6",
         "website": "www.synerty.com"
     },
     "requiresServices": [
         "logic",
         "storage",
         "field",
         "office",
```

### Comparing `peek-core-user-3.4.5/peek_core_user/server/UserApiABC.py` & `peek-core-user-3.4.6/peek_core_user/server/UserApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/server/UserDbErrors.py` & `peek-core-user-3.4.6/peek_core_user/server/UserDbErrors.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/server/UserFieldHookApiABC.py` & `peek-core-user-3.4.6/peek_core_user/server/UserFieldHookApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/server/UserImportApiABC.py` & `peek-core-user-3.4.6/peek_core_user/server/UserImportApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/server/UserInfoApiABC.py` & `peek-core-user-3.4.6/peek_core_user/server/UserInfoApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/server/UserLoginApiABC.py` & `peek-core-user-3.4.6/peek_core_user/server/UserLoginApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/tuples/DeviceWithUserDetails.py` & `peek-core-user-3.4.6/peek_core_user/tuples/DeviceWithUserDetails.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/tuples/UserDetailTuple.py` & `peek-core-user-3.4.6/peek_core_user/tuples/UserDetailTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/tuples/UserListItemTuple.py` & `peek-core-user-3.4.6/peek_core_user/tuples/UserListItemTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/tuples/UserLoggedInInfoTuple.py` & `peek-core-user-3.4.6/peek_core_user/tuples/UserLoggedInInfoTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/tuples/import_/ImportInternalUserTuple.py` & `peek-core-user-3.4.6/peek_core_user/tuples/import_/ImportInternalUserTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/tuples/login/UserLoginAction.py` & `peek-core-user-3.4.6/peek_core_user/tuples/login/UserLoginAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/tuples/login/UserLoginResponseTuple.py` & `peek-core-user-3.4.6/peek_core_user/tuples/login/UserLoginResponseTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/tuples/login/UserLogoutAction.py` & `peek-core-user-3.4.6/peek_core_user/tuples/login/UserLogoutAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user/tuples/login/UserLogoutResponseTuple.py` & `peek-core-user-3.4.6/peek_core_user/tuples/login/UserLogoutResponseTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/peek_core_user.egg-info/SOURCES.txt` & `peek-core-user-3.4.6/peek_core_user.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.4.5/setup.py` & `peek-core-user-3.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_core_user"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Plugin ENAMC Email Incidents."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

