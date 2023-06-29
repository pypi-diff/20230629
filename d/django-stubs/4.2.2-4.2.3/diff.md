# Comparing `tmp/django-stubs-4.2.2.tar.gz` & `tmp/django-stubs-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-stubs-4.2.2.tar", last modified: Tue Jun 27 17:51:06 2023, max compression
+gzip compressed data, was "django-stubs-4.2.3.tar", last modified: Thu Jun 29 17:11:02 2023, max compression
```

## Comparing `django-stubs-4.2.2.tar` & `django-stubs-4.2.3.tar`

### file list

```diff
@@ -1,837 +1,837 @@
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.593821 django-stubs-4.2.2/
--rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-06-02 14:08:54.000000 django-stubs-4.2.2/LICENSE.md
--rw-r--r--   0 marti     (1000) marti      (121)    15867 2023-06-27 17:51:06.593821 django-stubs-4.2.2/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)    14909 2023-06-27 17:49:10.000000 django-stubs-4.2.2/README.md
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.480488 django-stubs-4.2.2/django-stubs/
--rw-r--r--   0 marti     (1000) marti      (121)      157 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.480488 django-stubs-4.2.2/django-stubs/apps/
--rw-r--r--   0 marti     (1000) marti      (121)       78 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/apps/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      960 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/apps/config.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1963 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/apps/registry.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.483821 django-stubs-4.2.2/django-stubs/conf/
--rw-r--r--   0 marti     (1000) marti      (121)     1438 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/conf/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    17261 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/conf/global_settings.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.483821 django-stubs-4.2.2/django-stubs/conf/locale/
--rw-r--r--   0 marti     (1000) marti      (121)       50 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/conf/locale/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.483821 django-stubs-4.2.2/django-stubs/conf/urls/
--rw-r--r--   0 marti     (1000) marti      (121)     1073 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/conf/urls/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      231 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/conf/urls/i18n.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      193 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/conf/urls/static.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.483821 django-stubs-4.2.2/django-stubs/contrib/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.487155 django-stubs-4.2.2/django-stubs/contrib/admin/
--rw-r--r--   0 marti     (1000) marti      (121)     1157 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      313 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/actions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      136 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1068 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/admin/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2208 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      175 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3887 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/filters.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      237 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/forms.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5562 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/helpers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.487155 django-stubs-4.2.2/django-stubs/contrib/admin/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1032 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    16372 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/admin/options.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4088 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/admin/sites.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.487155 django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1981 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/admin_list.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      690 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/admin_modify.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      503 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/admin_urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      605 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      441 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/log.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1629 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/tests.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3665 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/admin/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.490488 django-stubs-4.2.2/django-stubs/contrib/admin/views/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/views/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      374 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/views/autocomplete.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      383 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/views/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3055 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/admin/views/main.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5652 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/admin/widgets.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.490488 django-stubs-4.2.2/django-stubs/contrib/admindocs/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admindocs/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admindocs/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      478 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admindocs/middleware.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admindocs/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      840 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admindocs/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1018 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admindocs/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.493821 django-stubs-4.2.2/django-stubs/contrib/auth/
--rw-r--r--   0 marti     (1000) marti      (121)     1272 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      496 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       68 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1891 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/backends.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1503 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/auth/base_user.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      662 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/context_processors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      934 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3944 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/contrib/auth/forms.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.493821 django-stubs-4.2.2/django-stubs/contrib/auth/handlers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/handlers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/handlers/modwsgi.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1962 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/hashers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.493821 django-stubs-4.2.2/django-stubs/contrib/auth/management/
--rw-r--r--   0 marti     (1000) marti      (121)      406 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/auth/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.493821 django-stubs-4.2.2/django-stubs/contrib/auth/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      125 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/management/commands/changepassword.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      208 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/management/commands/createsuperuser.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      739 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.493821 django-stubs-4.2.2/django-stubs/contrib/auth/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1228 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4613 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/auth/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2081 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/password_validation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/signals.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      735 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/contrib/auth/tokens.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      153 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/validators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2387 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.497155 django-stubs-4.2.2/django-stubs/contrib/contenttypes/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      655 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       76 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      414 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3851 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1421 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/forms.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.497155 django-stubs-4.2.2/django-stubs/contrib/contenttypes/management/
--rw-r--r--   0 marti     (1000) marti      (121)     1305 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.497155 django-stubs-4.2.2/django-stubs/contrib/contenttypes/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      467 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/management/commands/remove_stale_contenttypes.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.497155 django-stubs-4.2.2/django-stubs/contrib/contenttypes/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1020 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      213 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.497155 django-stubs-4.2.2/django-stubs/contrib/flatpages/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      196 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      136 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/forms.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      293 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.497155 django-stubs-4.2.2/django-stubs/contrib/flatpages/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      402 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       81 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/sitemaps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.497155 django-stubs-4.2.2/django-stubs/contrib/flatpages/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      484 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/templatetags/flatpages.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      309 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.500488 django-stubs-4.2.2/django-stubs/contrib/gis/
--rw-r--r--   0 marti     (1000) marti      (121)       24 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.500488 django-stubs-4.2.2/django-stubs/contrib/gis/admin/
--rw-r--r--   0 marti     (1000) marti      (121)      872 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/admin/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1174 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/admin/options.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      272 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/admin/widgets.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       67 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.500488 django-stubs-4.2.2/django-stubs/contrib/gis/db/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.500488 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.500488 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      200 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/adapter.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1443 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      836 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1348 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/operations.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.503821 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      251 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      781 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      333 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1134 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      699 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/schema.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.503821 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      226 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/adapter.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      254 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      444 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      287 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      729 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1440 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      826 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/schema.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.503821 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      399 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/adapter.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      351 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      189 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/const.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      407 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      360 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      798 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2189 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/pgraster.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      340 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/schema.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.507155 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      182 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/adapter.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      835 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      127 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      358 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      451 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      808 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1286 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1103 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      656 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.507155 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/
--rw-r--r--   0 marti     (1000) marti      (121)      847 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      800 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/aggregates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6077 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6232 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/functions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2955 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/lookups.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      345 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/proxy.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.507155 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/sql/
--rw-r--r--   0 marti     (1000) marti      (121)      166 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/sql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      829 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/sql/conversion.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      866 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/feeds.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.507155 django-stubs-4.2.2/django-stubs/contrib/gis/forms/
--rw-r--r--   0 marti     (1000) marti      (121)      642 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/forms/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      840 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/forms/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      951 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/forms/widgets.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.510488 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/
--rw-r--r--   0 marti     (1000) marti      (121)     1070 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      137 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      574 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/datasource.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      324 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/driver.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      688 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/envelope.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      200 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/error.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      947 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/feature.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1460 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/field.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4844 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/geometries.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      304 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/geomtype.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1692 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/layer.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      510 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/libgdal.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.510488 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1036 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/ds.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      961 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1077 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/generation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      970 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/geom.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1053 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/raster.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      614 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/srs.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.510488 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/raster/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/raster/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1565 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/raster/band.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      225 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/raster/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      252 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/raster/const.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2329 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/raster/source.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2191 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/srs.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.510488 django-stubs-4.2.2/django-stubs/contrib/gis/geoip2/
--rw-r--r--   0 marti     (1000) marti      (121)      106 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geoip2/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1202 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geoip2/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       99 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geoip2/resources.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       97 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geometry.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.513821 django-stubs-4.2.2/django-stubs/contrib/gis/geos/
--rw-r--r--   0 marti     (1000) marti      (121)      883 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      185 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      604 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/collections.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1250 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/coordseq.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       36 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/error.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      276 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/factory.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5258 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/geometry.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      467 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/io.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      896 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/libgeos.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      766 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/linestring.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1148 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/mutable_list.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      816 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/point.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      713 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/polygon.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      737 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prepared.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.513821 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/
--rw-r--r--   0 marti     (1000) marti      (121)     4249 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      795 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      474 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/errcheck.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      792 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/geom.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2975 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/io.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      232 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/misc.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      553 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/predicates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      434 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/prepared.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      496 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/threadsafe.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      609 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/topology.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1418 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/measure.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      252 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/ptr.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.517155 django-stubs-4.2.2/django-stubs/contrib/gis/serializers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/serializers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      493 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/serializers/geojson.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      244 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/shortcuts.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.517155 django-stubs-4.2.2/django-stubs/contrib/gis/sitemaps/
--rw-r--r--   0 marti     (1000) marti      (121)      138 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/sitemaps/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      328 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/sitemaps/kml.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      352 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/sitemaps/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.517155 django-stubs-4.2.2/django-stubs/contrib/gis/utils/
--rw-r--r--   0 marti     (1000) marti      (121)      436 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/utils/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2526 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/utils/layermapping.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      129 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/utils/ogrinfo.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      320 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/utils/ogrinspect.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      199 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/utils/srs.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      202 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.517155 django-stubs-4.2.2/django-stubs/contrib/humanize/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/humanize/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/humanize/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.517155 django-stubs-4.2.2/django-stubs/contrib/humanize/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/humanize/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      859 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/humanize/templatetags/humanize.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.517155 django-stubs-4.2.2/django-stubs/contrib/messages/
--rw-r--r--   0 marti     (1000) marti      (121)      715 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1294 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/api.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/constants.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      225 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/context_processors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      349 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.520488 django-stubs-4.2.2/django-stubs/contrib/messages/storage/
--rw-r--r--   0 marti     (1000) marti      (121)      168 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/messages/storage/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      906 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/storage/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      463 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/storage/cookie.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      228 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/storage/fallback.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      468 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/storage/session.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       44 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      347 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.520488 django-stubs-4.2.2/django-stubs/contrib/postgres/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.520488 django-stubs-4.2.2/django-stubs/contrib/postgres/aggregates/
--rw-r--r--   0 marti     (1000) marti      (121)      826 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/aggregates/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      357 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/aggregates/general.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       29 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/aggregates/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      470 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/aggregates/statistics.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      270 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      847 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/constraints.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.523821 django-stubs-4.2.2/django-stubs/contrib/postgres/fields/
--rw-r--r--   0 marti     (1000) marti      (121)      759 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/fields/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1897 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/fields/array.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/fields/citext.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      573 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/fields/hstore.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      376 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/fields/jsonb.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3009 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/fields/ranges.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      106 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/fields/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.523821 django-stubs-4.2.2/django-stubs/contrib/postgres/forms/
--rw-r--r--   0 marti     (1000) marti      (121)       86 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/forms/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2341 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/forms/array.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      462 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/forms/hstore.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      207 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/forms/jsonb.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1486 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/forms/ranges.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       95 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/functions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3972 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/indexes.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      631 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/lookups.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2045 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3653 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/search.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      152 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/serializers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      230 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/signals.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      177 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      635 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/validators.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.523821 django-stubs-4.2.2/django-stubs/contrib/redirects/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/redirects/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      185 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/redirects/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/redirects/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      379 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/redirects/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.523821 django-stubs-4.2.2/django-stubs/contrib/redirects/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/redirects/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      150 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/redirects/models.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.527155 django-stubs-4.2.2/django-stubs/contrib/sessions/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.527155 django-stubs-4.2.2/django-stubs/contrib/sessions/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1869 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      280 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/backends/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/backends/cached_db.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      490 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/backends/db.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      239 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/backends/file.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/backends/signed_cookies.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      676 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/base_session.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      156 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/exceptions.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.527155 django-stubs-4.2.2/django-stubs/contrib/sessions/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.527155 django-stubs-4.2.2/django-stubs/contrib/sessions/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/management/commands/clearsessions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      447 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.527155 django-stubs-4.2.2/django-stubs/contrib/sessions/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      243 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      337 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/serializers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.527155 django-stubs-4.2.2/django-stubs/contrib/sitemaps/
--rw-r--r--   0 marti     (1000) marti      (121)     1909 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/sitemaps/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sitemaps/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.527155 django-stubs-4.2.2/django-stubs/contrib/sitemaps/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sitemaps/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.527155 django-stubs-4.2.2/django-stubs/contrib/sitemaps/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sitemaps/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sitemaps/management/commands/ping_google.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      694 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/sitemaps/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.530488 django-stubs-4.2.2/django-stubs/contrib/sites/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sites/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      138 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sites/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       69 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sites/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      247 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/sites/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      289 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/sites/management.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sites/managers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      209 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sites/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.530488 django-stubs-4.2.2/django-stubs/contrib/sites/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sites/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      585 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sites/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      307 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/sites/requests.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      221 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sites/shortcuts.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.530488 django-stubs-4.2.2/django-stubs/contrib/staticfiles/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      263 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2489 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/finders.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1674 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/handlers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.530488 django-stubs-4.2.2/django-stubs/contrib/staticfiles/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.533821 django-stubs-4.2.2/django-stubs/contrib/staticfiles/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1055 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       87 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/management/commands/findstatic.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/management/commands/runserver.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2292 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/storage.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/testing.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      152 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      345 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.533821 django-stubs-4.2.2/django-stubs/contrib/syndication/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/syndication/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      131 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/syndication/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1889 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/syndication/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.533821 django-stubs-4.2.2/django-stubs/core/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       98 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/asgi.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.533821 django-stubs-4.2.2/django-stubs/core/cache/
--rw-r--r--   0 marti     (1000) marti      (121)      624 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/cache/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.537155 django-stubs-4.2.2/django-stubs/core/cache/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/cache/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4121 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/cache/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      593 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/cache/backends/db.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      182 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/cache/backends/dummy.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      204 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/cache/backends/filebased.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      180 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/cache/backends/locmem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      782 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/cache/backends/memcached.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/cache/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.537155 django-stubs-4.2.2/django-stubs/core/checks/
--rw-r--r--   0 marti     (1000) marti      (121)      652 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      265 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/async_checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      529 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/caches.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.537155 django-stubs-4.2.2/django-stubs/core/checks/compatibility/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/compatibility/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      256 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/checks/compatibility/django_4_0.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      229 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/database.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      268 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/checks/files.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1084 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/messages.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      389 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/model_checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1837 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/checks/registry.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.537155 django-stubs-4.2.2/django-stubs/core/checks/security/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/security/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2087 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/checks/security/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      514 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/checks/security/csrf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      577 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/security/sessions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      565 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/checks/templates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      625 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/translation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      706 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1883 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/exceptions.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.540488 django-stubs-4.2.2/django-stubs/core/files/
--rw-r--r--   0 marti     (1000) marti      (121)       68 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/files/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1606 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/files/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      359 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/files/images.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      296 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/files/locks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      130 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/files/move.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.540488 django-stubs-4.2.2/django-stubs/core/files/storage/
--rw-r--r--   0 marti     (1000) marti      (121)      634 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/core/files/storage/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1073 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/core/files/storage/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      751 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/core/files/storage/filesystem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      450 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/core/files/storage/handler.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      725 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/core/files/storage/memory.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      338 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/files/storage/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/files/temp.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1450 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/files/uploadedfile.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3017 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/files/uploadhandler.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      736 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/files/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.540488 django-stubs-4.2.2/django-stubs/core/handlers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/handlers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2043 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/handlers/asgi.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1220 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/handlers/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      770 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/handlers/exception.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1405 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/handlers/wsgi.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.540488 django-stubs-4.2.2/django-stubs/core/mail/
--rw-r--r--   0 marti     (1000) marti      (121)     1714 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/core/mail/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.543821 django-stubs-4.2.2/django-stubs/core/mail/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/mail/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      668 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/mail/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      303 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/mail/backends/console.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/mail/backends/dummy.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/mail/backends/filebased.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/mail/backends/locmem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      395 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/mail/backends/smtp.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4640 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/mail/message.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       95 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/mail/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.543821 django-stubs-4.2.2/django-stubs/core/management/
--rw-r--r--   0 marti     (1000) marti      (121)      829 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3617 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/management/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1099 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/color.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.547154 django-stubs-4.2.2/django-stubs/core/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      179 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/check.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      430 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/compilemessages.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      284 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/createcachetable.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/dbshell.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      519 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/diffsettings.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      123 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/dumpdata.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      177 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/flush.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      789 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/inspectdb.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1140 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/loaddata.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1227 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/makemessages.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      467 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/makemigrations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      643 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/migrate.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      515 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/runserver.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      111 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/sendtestemail.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      268 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/shell.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      371 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/showmigrations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      110 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/sqlflush.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      203 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/sqlmigrate.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       83 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/sqlsequencereset.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      330 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/squashmigrations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      124 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/startapp.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      124 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/startproject.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      232 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/test.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/testserver.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      488 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/sql.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      964 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/templates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      850 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2229 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/paginator.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.550488 django-stubs-4.2.2/django-stubs/core/serializers/
--rw-r--r--   0 marti     (1000) marti      (121)     1437 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/serializers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3193 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/serializers/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      577 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/serializers/json.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/serializers/jsonl.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      490 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/serializers/python.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      831 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/serializers/pyyaml.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2321 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/serializers/xml_serializer.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.550488 django-stubs-4.2.2/django-stubs/core/servers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/servers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1165 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/servers/basehttp.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      139 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/signals.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1846 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/signing.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4218 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/validators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       98 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/wsgi.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.550488 django-stubs-4.2.2/django-stubs/db/
--rw-r--r--   0 marti     (1000) marti      (121)     1047 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.550488 django-stubs-4.2.2/django-stubs/db/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.550488 django-stubs-4.2.2/django-stubs/db/backends/base/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/base/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5296 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/db/backends/base/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      555 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/base/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1132 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/base/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5118 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/base/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1870 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/base/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     7157 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/base/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3557 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/base/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      389 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/base/validation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3134 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/ddl_references.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.553821 django-stubs-4.2.2/django-stubs/db/backends/dummy/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/dummy/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      924 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/dummy/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      176 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/dummy/features.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.553821 django-stubs-4.2.2/django-stubs/db/backends/mysql/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2493 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      473 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      734 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/compiler.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      255 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3434 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      568 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2872 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      902 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      354 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/validation.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.553821 django-stubs-4.2.2/django-stubs/db/backends/oracle/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2711 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      546 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      373 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1923 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/functions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      351 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3990 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      924 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      511 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      308 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/validation.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.557154 django-stubs-4.2.2/django-stubs/db/backends/postgresql/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/postgresql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1382 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/postgresql/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      524 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/postgresql/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      208 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/postgresql/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2197 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/postgresql/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      304 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/postgresql/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      529 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/postgresql/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      809 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/postgresql/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       63 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/signals.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.557154 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1052 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      441 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      322 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      205 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      432 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1014 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      215 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2876 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.560488 django-stubs-4.2.2/django-stubs/db/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)      265 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2830 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/autodetector.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      664 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1739 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/executor.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2404 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/migrations/graph.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1960 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/loader.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1111 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/migration.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.560488 django-stubs-4.2.2/django-stubs/db/migrations/operations/
--rw-r--r--   0 marti     (1000) marti      (121)     1159 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/migrations/operations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1522 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/migrations/operations/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1251 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/migrations/operations/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5342 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/migrations/operations/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2043 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/migrations/operations/special.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      974 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/migrations/operations/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      290 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/optimizer.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1109 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/questioner.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      755 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/recorder.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1835 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/serializer.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4952 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/migrations/state.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      195 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1235 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/writer.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.563821 django-stubs-4.2.2/django-stubs/db/models/
--rw-r--r--   0 marti     (1000) marti      (121)     5016 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      684 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/aggregates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3699 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       96 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/constants.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2248 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/constraints.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3475 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/deletion.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1074 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/enums.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10062 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/expressions.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.563821 django-stubs-4.2.2/django-stubs/db/models/fields/
--rw-r--r--   0 marti     (1000) marti      (121)    21191 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/fields/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4001 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/db/models/fields/files.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3504 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/fields/json.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      515 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/fields/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      161 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/fields/proxy.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10684 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/fields/related.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3463 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/fields/related_descriptors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1393 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/fields/related_lookups.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4576 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/fields/reverse_related.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.567154 django-stubs-4.2.2/django-stubs/db/models/functions/
--rw-r--r--   0 marti     (1000) marti      (121)     3378 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/functions/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      547 2023-04-27 12:45:58.000000 django-stubs-4.2.2/django-stubs/db/models/functions/comparison.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1343 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/functions/datetime.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1222 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/functions/math.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/functions/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4623 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/functions/text.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      918 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/functions/window.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2228 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/indexes.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5850 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/lookups.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     8468 2023-04-27 12:45:58.000000 django-stubs-4.2.2/django-stubs/db/models/manager.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5363 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/options.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10883 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/query.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3277 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/query_utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      888 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/signals.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.567154 django-stubs-4.2.2/django-stubs/db/models/sql/
--rw-r--r--   0 marti     (1000) marti      (121)      284 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/sql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6507 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/sql/compiler.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      286 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/sql/constants.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1791 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/sql/datastructures.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     9499 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/sql/query.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1619 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/sql/subqueries.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2075 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/sql/where.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      473 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2178 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/db/transaction.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2061 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.567154 django-stubs-4.2.2/django-stubs/dispatch/
--rw-r--r--   0 marti     (1000) marti      (121)      116 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/dispatch/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1251 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/dispatch/dispatcher.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.570488 django-stubs-4.2.2/django-stubs/forms/
--rw-r--r--   0 marti     (1000) marti      (121)     4083 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/forms/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2874 2023-04-27 12:45:58.000000 django-stubs-4.2.2/django-stubs/forms/boundfield.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    20422 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/forms/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3196 2023-04-27 12:45:58.000000 django-stubs-4.2.2/django-stubs/forms/forms.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3777 2023-04-27 12:45:58.000000 django-stubs-4.2.2/django-stubs/forms/formsets.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    12444 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/forms/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1125 2023-04-27 12:45:58.000000 django-stubs-4.2.2/django-stubs/forms/renderers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2337 2023-04-27 12:45:58.000000 django-stubs-4.2.2/django-stubs/forms/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10456 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/forms/widgets.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.570488 django-stubs-4.2.2/django-stubs/http/
--rw-r--r--   0 marti     (1000) marti      (121)     1332 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/http/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       96 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/http/cookie.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1979 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/http/multipartparser.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     8346 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/http/request.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5819 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/http/response.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.570488 django-stubs-4.2.2/django-stubs/middleware/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/middleware/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1063 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/middleware/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      387 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/middleware/clickjacking.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      968 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/middleware/common.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1098 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/middleware/csrf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      339 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/middleware/gzip.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      369 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/middleware/http.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      417 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/middleware/locale.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      645 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/middleware/security.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1514 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/shortcuts.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.573821 django-stubs-4.2.2/django-stubs/template/
--rw-r--r--   0 marti     (1000) marti      (121)      756 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.573821 django-stubs-4.2.2/django-stubs/template/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      876 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/template/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1062 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/backends/django.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      432 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/backends/dummy.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      575 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/backends/jinja2.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      215 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/backends/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5644 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/template/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3401 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/template/context.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      631 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/context_processors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3483 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/defaultfilters.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6912 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/defaulttags.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2158 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/engine.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      511 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3244 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/library.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      684 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/loader.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2267 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/template/loader_tags.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.577154 django-stubs-4.2.2/django-stubs/template/loaders/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/loaders/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       88 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/loaders/app_directories.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      488 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/loaders/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      554 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/loaders/cached.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      518 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/loaders/filesystem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      323 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/loaders/locmem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2564 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/response.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1246 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/smartif.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      589 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.577154 django-stubs-4.2.2/django-stubs/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      629 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/templatetags/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3492 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/templatetags/i18n.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      410 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/templatetags/l10n.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1123 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/templatetags/static.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1076 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/templatetags/tz.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.577154 django-stubs-4.2.2/django-stubs/test/
--rw-r--r--   0 marti     (1000) marti      (121)      848 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/test/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     9121 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/test/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1148 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/test/html.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6591 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/test/runner.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      539 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/test/selenium.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      905 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/test/signals.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10511 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/test/testcases.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6314 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/test/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.580487 django-stubs-4.2.2/django-stubs/urls/
--rw-r--r--   0 marti     (1000) marti      (121)     1576 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/urls/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      857 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/urls/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1349 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/urls/conf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      778 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/urls/converters.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      102 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/urls/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4722 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/urls/resolvers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      157 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/urls/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.583821 django-stubs-4.2.2/django-stubs/utils/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/_os.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1485 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/archive.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      230 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/asyncio.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2872 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/autoreload.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      591 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/baseconv.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1287 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1300 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/connection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      570 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/crypto.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4679 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/datastructures.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2033 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/dateformat.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      505 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/dateparse.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      156 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/dates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      547 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/datetime_safe.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      325 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/deconstruct.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      876 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1746 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/deprecation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/duration.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3177 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/encoding.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2676 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/feedgenerator.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1814 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/formats.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4544 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/functional.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       66 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/hashable.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2481 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/html.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1283 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/http.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      483 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/inspect.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      175 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/ipv6.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       61 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/itercompat.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      714 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/jslex.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1692 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/log.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      242 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/lorem_ipsum.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      312 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/module_loading.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      319 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/numberformat.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      917 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/regex_helper.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      616 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/safestring.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      557 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/termcolors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1933 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/text.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      423 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/timesince.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2011 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/timezone.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      309 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/topological_sort.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.587154 django-stubs-4.2.2/django-stubs/utils/translation/
--rw-r--r--   0 marti     (1000) marti      (121)     2033 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/translation/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/translation/reloader.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      335 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/translation/template.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      801 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/translation/trans_null.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2986 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/translation/trans_real.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      986 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/tree.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      518 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/version.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      379 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/xmlutils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.587154 django-stubs-4.2.2/django-stubs/views/
--rw-r--r--   0 marti     (1000) marti      (121)       39 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/csrf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2741 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/views/debug.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.590487 django-stubs-4.2.2/django-stubs/views/decorators/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/decorators/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      347 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/views/decorators/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/decorators/clickjacking.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      162 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/decorators/common.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      427 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/decorators/csrf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      259 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/views/decorators/debug.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      146 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/decorators/gzip.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      718 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/views/decorators/http.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      218 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/decorators/vary.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      782 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/defaults.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.590487 django-stubs-4.2.2/django-stubs/views/generic/
--rw-r--r--   0 marti     (1000) marti      (121)      797 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/generic/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2272 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/generic/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4525 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/generic/dates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1109 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/generic/detail.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3393 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/views/generic/edit.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1819 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/views/generic/list.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1035 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/i18n.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      482 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/static.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.590487 django-stubs-4.2.2/django_stubs.egg-info/
--rw-r--r--   0 marti     (1000) marti      (121)    15867 2023-06-27 17:51:06.000000 django-stubs-4.2.2/django_stubs.egg-info/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)    30431 2023-06-27 17:51:06.000000 django-stubs-4.2.2/django_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 marti     (1000) marti      (121)        1 2023-06-27 17:51:06.000000 django-stubs-4.2.2/django_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 marti     (1000) marti      (121)      150 2023-06-27 17:51:06.000000 django-stubs-4.2.2/django_stubs.egg-info/requires.txt
--rw-r--r--   0 marti     (1000) marti      (121)       32 2023-06-27 17:51:06.000000 django-stubs-4.2.2/django_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.590487 django-stubs-4.2.2/mypy_django_plugin/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/mypy_django_plugin/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)     4295 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/config.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.590487 django-stubs-4.2.2/mypy_django_plugin/django/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/mypy_django_plugin/django/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)    21306 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/django/context.py
--rw-r--r--   0 marti     (1000) marti      (121)      227 2023-03-15 16:53:32.000000 django-stubs-4.2.2/mypy_django_plugin/errorcodes.py
--rw-r--r--   0 marti     (1000) marti      (121)       89 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/exceptions.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.593821 django-stubs-4.2.2/mypy_django_plugin/lib/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/mypy_django_plugin/lib/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)     2289 2023-04-27 12:45:58.000000 django-stubs-4.2.2/mypy_django_plugin/lib/fullnames.py
--rw-r--r--   0 marti     (1000) marti      (121)    13634 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/lib/helpers.py
--rw-r--r--   0 marti     (1000) marti      (121)    15544 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/main.py
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/mypy_django_plugin/py.typed
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.593821 django-stubs-4.2.2/mypy_django_plugin/transformers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)     9704 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/fields.py
--rw-r--r--   0 marti     (1000) marti      (121)     1787 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/forms.py
--rw-r--r--   0 marti     (1000) marti      (121)     1313 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/functional.py
--rw-r--r--   0 marti     (1000) marti      (121)     3104 2023-03-15 16:53:32.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/init_create.py
--rw-r--r--   0 marti     (1000) marti      (121)    20857 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/managers.py
--rw-r--r--   0 marti     (1000) marti      (121)     1938 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/meta.py
--rw-r--r--   0 marti     (1000) marti      (121)    32277 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/models.py
--rw-r--r--   0 marti     (1000) marti      (121)     2826 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/orm_lookups.py
--rw-r--r--   0 marti     (1000) marti      (121)    13086 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/querysets.py
--rw-r--r--   0 marti     (1000) marti      (121)     2048 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/request.py
--rw-r--r--   0 marti     (1000) marti      (121)     2495 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/settings.py
--rw-r--r--   0 marti     (1000) marti      (121)      458 2023-06-27 17:49:10.000000 django-stubs-4.2.2/pyproject.toml
--rw-r--r--   0 marti     (1000) marti      (121)      308 2023-06-27 17:51:06.593821 django-stubs-4.2.2/setup.cfg
--rw-r--r--   0 marti     (1000) marti      (121)     2233 2023-06-27 17:49:10.000000 django-stubs-4.2.2/setup.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.593821 django-stubs-4.2.2/tests/
--rw-r--r--   0 marti     (1000) marti      (121)     5766 2023-06-27 17:49:10.000000 django-stubs-4.2.2/tests/test_error_handling.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.949514 django-stubs-4.2.3/
+-rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-06-02 14:08:54.000000 django-stubs-4.2.3/LICENSE.md
+-rw-r--r--   0 marti     (1000) marti      (121)    15960 2023-06-29 17:11:02.949514 django-stubs-4.2.3/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)    15002 2023-06-29 17:05:25.000000 django-stubs-4.2.3/README.md
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.806182 django-stubs-4.2.3/django-stubs/
+-rw-r--r--   0 marti     (1000) marti      (121)      157 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.809515 django-stubs-4.2.3/django-stubs/apps/
+-rw-r--r--   0 marti     (1000) marti      (121)       78 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/apps/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1094 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/apps/config.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1963 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/apps/registry.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.809515 django-stubs-4.2.3/django-stubs/conf/
+-rw-r--r--   0 marti     (1000) marti      (121)     1434 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/conf/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    17261 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/conf/global_settings.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.809515 django-stubs-4.2.3/django-stubs/conf/locale/
+-rw-r--r--   0 marti     (1000) marti      (121)       50 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/conf/locale/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.809515 django-stubs-4.2.3/django-stubs/conf/urls/
+-rw-r--r--   0 marti     (1000) marti      (121)     1073 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/conf/urls/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      231 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/conf/urls/i18n.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      193 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/conf/urls/static.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.809515 django-stubs-4.2.3/django-stubs/contrib/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.816182 django-stubs-4.2.3/django-stubs/contrib/admin/
+-rw-r--r--   0 marti     (1000) marti      (121)     1157 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      313 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/actions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      136 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1068 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/admin/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2208 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      175 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3887 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/filters.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      237 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/forms.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5562 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/helpers.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.816182 django-stubs-4.2.3/django-stubs/contrib/admin/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1032 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    16372 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/admin/options.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4088 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/admin/sites.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.816182 django-stubs-4.2.3/django-stubs/contrib/admin/templatetags/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1981 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/templatetags/admin_list.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      690 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/templatetags/admin_modify.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      503 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/templatetags/admin_urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      605 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/templatetags/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      441 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/templatetags/log.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1629 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/tests.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3665 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/admin/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.816182 django-stubs-4.2.3/django-stubs/contrib/admin/views/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/views/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      374 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/views/autocomplete.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      383 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admin/views/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3055 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/admin/views/main.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5652 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/admin/widgets.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.816182 django-stubs-4.2.3/django-stubs/contrib/admindocs/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admindocs/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admindocs/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      478 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admindocs/middleware.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admindocs/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      840 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admindocs/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1018 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/admindocs/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.822848 django-stubs-4.2.3/django-stubs/contrib/auth/
+-rw-r--r--   0 marti     (1000) marti      (121)     1272 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      496 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       68 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1891 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/backends.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1503 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/auth/base_user.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      662 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/context_processors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      955 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/contrib/auth/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3944 2023-06-02 14:08:54.000000 django-stubs-4.2.3/django-stubs/contrib/auth/forms.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.822848 django-stubs-4.2.3/django-stubs/contrib/auth/handlers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/handlers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/handlers/modwsgi.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1962 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/hashers.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.822848 django-stubs-4.2.3/django-stubs/contrib/auth/management/
+-rw-r--r--   0 marti     (1000) marti      (121)      406 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/auth/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.822848 django-stubs-4.2.3/django-stubs/contrib/auth/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      125 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/management/commands/changepassword.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      208 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/management/commands/createsuperuser.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      739 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.822848 django-stubs-4.2.3/django-stubs/contrib/auth/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1228 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4613 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/auth/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2081 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/password_validation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/signals.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      735 2023-06-02 14:08:54.000000 django-stubs-4.2.3/django-stubs/contrib/auth/tokens.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      153 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/validators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2387 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/auth/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.822848 django-stubs-4.2.3/django-stubs/contrib/contenttypes/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/contenttypes/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      655 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/contenttypes/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       76 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/contenttypes/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      414 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/contenttypes/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3851 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/contenttypes/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1421 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/contenttypes/forms.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.822848 django-stubs-4.2.3/django-stubs/contrib/contenttypes/management/
+-rw-r--r--   0 marti     (1000) marti      (121)     1305 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/contenttypes/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.822848 django-stubs-4.2.3/django-stubs/contrib/contenttypes/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/contenttypes/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      467 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/contenttypes/management/commands/remove_stale_contenttypes.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.826182 django-stubs-4.2.3/django-stubs/contrib/contenttypes/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/contenttypes/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1020 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/contenttypes/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      213 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/contenttypes/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.826182 django-stubs-4.2.3/django-stubs/contrib/flatpages/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/flatpages/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      196 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/flatpages/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/flatpages/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      136 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/flatpages/forms.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      293 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/flatpages/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.826182 django-stubs-4.2.3/django-stubs/contrib/flatpages/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/flatpages/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      402 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/flatpages/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       81 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/flatpages/sitemaps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.826182 django-stubs-4.2.3/django-stubs/contrib/flatpages/templatetags/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/flatpages/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      484 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/flatpages/templatetags/flatpages.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/flatpages/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      309 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/flatpages/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.829515 django-stubs-4.2.3/django-stubs/contrib/gis/
+-rw-r--r--   0 marti     (1000) marti      (121)       24 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.829515 django-stubs-4.2.3/django-stubs/contrib/gis/admin/
+-rw-r--r--   0 marti     (1000) marti      (121)      872 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/admin/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1174 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/admin/options.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      272 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/admin/widgets.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       67 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.829515 django-stubs-4.2.3/django-stubs/contrib/gis/db/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.829515 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.829515 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/base/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/base/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      200 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/base/adapter.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1443 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/base/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      836 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/base/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1348 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/base/operations.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.829515 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/mysql/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/mysql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      251 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/mysql/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      781 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/mysql/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      333 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/mysql/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1134 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/mysql/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      699 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/mysql/schema.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.832848 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/oracle/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/oracle/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      226 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/oracle/adapter.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      254 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/oracle/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      444 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/oracle/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      287 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/oracle/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      729 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/oracle/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1440 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/oracle/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      826 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/oracle/schema.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.832848 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/postgis/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/postgis/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      399 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/postgis/adapter.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      351 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/postgis/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      189 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/postgis/const.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      407 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/postgis/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      360 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/postgis/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      798 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/postgis/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2189 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/postgis/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/postgis/pgraster.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      340 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/postgis/schema.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.836182 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/spatialite/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/spatialite/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      182 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/spatialite/adapter.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      835 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/spatialite/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      127 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/spatialite/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      358 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/spatialite/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      451 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/spatialite/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      808 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/spatialite/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1286 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1103 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      656 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.836182 django-stubs-4.2.3/django-stubs/contrib/gis/db/models/
+-rw-r--r--   0 marti     (1000) marti      (121)      847 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/models/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      800 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/models/aggregates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6077 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/models/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6232 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/models/functions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2955 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/models/lookups.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      345 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/models/proxy.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.836182 django-stubs-4.2.3/django-stubs/contrib/gis/db/models/sql/
+-rw-r--r--   0 marti     (1000) marti      (121)      166 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/models/sql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      829 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/db/models/sql/conversion.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      866 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/feeds.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.836182 django-stubs-4.2.3/django-stubs/contrib/gis/forms/
+-rw-r--r--   0 marti     (1000) marti      (121)      642 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/forms/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      840 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/forms/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      951 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/forms/widgets.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.839515 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/
+-rw-r--r--   0 marti     (1000) marti      (121)     1070 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      137 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      574 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/datasource.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      324 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/driver.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      688 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/envelope.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      200 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/error.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      947 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/feature.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1460 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/field.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4844 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/geometries.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      304 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/geomtype.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1692 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/layer.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      510 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/libgdal.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.839515 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/prototypes/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/prototypes/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1036 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/prototypes/ds.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      961 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1077 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/prototypes/generation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      970 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/prototypes/geom.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1053 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/prototypes/raster.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      614 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/prototypes/srs.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.842848 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/raster/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/raster/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1565 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/raster/band.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      225 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/raster/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      252 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/raster/const.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2329 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/raster/source.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2193 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/contrib/gis/gdal/srs.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.842848 django-stubs-4.2.3/django-stubs/contrib/gis/geoip2/
+-rw-r--r--   0 marti     (1000) marti      (121)      106 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geoip2/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1202 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geoip2/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       99 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geoip2/resources.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       97 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geometry.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.846182 django-stubs-4.2.3/django-stubs/contrib/gis/geos/
+-rw-r--r--   0 marti     (1000) marti      (121)      883 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      185 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      604 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/collections.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1252 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/coordseq.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       36 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/error.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      276 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/factory.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5248 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/geometry.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      467 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/io.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      896 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/libgeos.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      766 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/linestring.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1126 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/mutable_list.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      816 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/point.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      713 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/polygon.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      737 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/prepared.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.849515 django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/
+-rw-r--r--   0 marti     (1000) marti      (121)     4249 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      795 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      474 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/errcheck.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      792 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/geom.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2975 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/io.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      232 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/misc.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      553 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/predicates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      434 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/prepared.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      496 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/threadsafe.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      609 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/topology.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1343 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/contrib/gis/measure.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      252 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/ptr.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.849515 django-stubs-4.2.3/django-stubs/contrib/gis/serializers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/serializers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      493 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/serializers/geojson.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      244 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/shortcuts.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.849515 django-stubs-4.2.3/django-stubs/contrib/gis/sitemaps/
+-rw-r--r--   0 marti     (1000) marti      (121)      138 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/sitemaps/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      328 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/sitemaps/kml.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      352 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/sitemaps/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.849515 django-stubs-4.2.3/django-stubs/contrib/gis/utils/
+-rw-r--r--   0 marti     (1000) marti      (121)      436 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/utils/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2526 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/utils/layermapping.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      129 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/gis/utils/ogrinfo.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      320 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/utils/ogrinspect.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      199 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/utils/srs.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      202 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/gis/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.849515 django-stubs-4.2.3/django-stubs/contrib/humanize/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/humanize/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/humanize/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.849515 django-stubs-4.2.3/django-stubs/contrib/humanize/templatetags/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/humanize/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      859 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/humanize/templatetags/humanize.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.852848 django-stubs-4.2.3/django-stubs/contrib/messages/
+-rw-r--r--   0 marti     (1000) marti      (121)      715 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/messages/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1294 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/messages/api.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/messages/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/messages/constants.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      225 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/messages/context_processors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      349 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/messages/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.852848 django-stubs-4.2.3/django-stubs/contrib/messages/storage/
+-rw-r--r--   0 marti     (1000) marti      (121)      168 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/messages/storage/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      906 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/messages/storage/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      463 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/messages/storage/cookie.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      228 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/messages/storage/fallback.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      468 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/messages/storage/session.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       44 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/messages/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      347 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/messages/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.856181 django-stubs-4.2.3/django-stubs/contrib/postgres/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.856181 django-stubs-4.2.3/django-stubs/contrib/postgres/aggregates/
+-rw-r--r--   0 marti     (1000) marti      (121)      826 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/aggregates/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      357 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/aggregates/general.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       29 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/aggregates/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      470 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/aggregates/statistics.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      270 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      847 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/constraints.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.856181 django-stubs-4.2.3/django-stubs/contrib/postgres/fields/
+-rw-r--r--   0 marti     (1000) marti      (121)      759 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/fields/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1897 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/fields/array.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/fields/citext.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      573 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/fields/hstore.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      376 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/fields/jsonb.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3009 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/fields/ranges.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      106 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/fields/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.859515 django-stubs-4.2.3/django-stubs/contrib/postgres/forms/
+-rw-r--r--   0 marti     (1000) marti      (121)       86 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/forms/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2341 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/forms/array.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      462 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/forms/hstore.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      207 2023-06-02 14:08:54.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/forms/jsonb.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1486 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/forms/ranges.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       95 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/functions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3972 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/indexes.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      631 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/lookups.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2045 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3602 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/search.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      152 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/serializers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      230 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/signals.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      177 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      635 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/postgres/validators.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.859515 django-stubs-4.2.3/django-stubs/contrib/redirects/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/redirects/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      185 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/redirects/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/redirects/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      379 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/redirects/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.859515 django-stubs-4.2.3/django-stubs/contrib/redirects/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/redirects/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      150 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/redirects/models.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.862848 django-stubs-4.2.3/django-stubs/contrib/sessions/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.862848 django-stubs-4.2.3/django-stubs/contrib/sessions/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/backends/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1869 2023-06-02 14:08:54.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/backends/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      280 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/backends/cache.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/backends/cached_db.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      490 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/backends/db.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      239 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/backends/file.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/backends/signed_cookies.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      676 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/base_session.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      156 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/exceptions.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.862848 django-stubs-4.2.3/django-stubs/contrib/sessions/management/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.862848 django-stubs-4.2.3/django-stubs/contrib/sessions/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/management/commands/clearsessions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      447 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.862848 django-stubs-4.2.3/django-stubs/contrib/sessions/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      243 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      337 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sessions/serializers.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.862848 django-stubs-4.2.3/django-stubs/contrib/sitemaps/
+-rw-r--r--   0 marti     (1000) marti      (121)     1909 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/sitemaps/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sitemaps/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.866181 django-stubs-4.2.3/django-stubs/contrib/sitemaps/management/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sitemaps/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.866181 django-stubs-4.2.3/django-stubs/contrib/sitemaps/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sitemaps/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sitemaps/management/commands/ping_google.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      694 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/sitemaps/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.866181 django-stubs-4.2.3/django-stubs/contrib/sites/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sites/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      138 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sites/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       69 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sites/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      247 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/sites/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      289 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/sites/management.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sites/managers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      209 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sites/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.866181 django-stubs-4.2.3/django-stubs/contrib/sites/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sites/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      585 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sites/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      307 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/sites/requests.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      221 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/sites/shortcuts.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.869515 django-stubs-4.2.3/django-stubs/contrib/staticfiles/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/staticfiles/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/staticfiles/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      263 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/staticfiles/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2489 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/staticfiles/finders.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1674 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/staticfiles/handlers.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.869515 django-stubs-4.2.3/django-stubs/contrib/staticfiles/management/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/staticfiles/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.869515 django-stubs-4.2.3/django-stubs/contrib/staticfiles/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/staticfiles/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1055 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       87 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/staticfiles/management/commands/findstatic.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/staticfiles/management/commands/runserver.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2292 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/staticfiles/storage.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/staticfiles/testing.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      152 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/staticfiles/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      345 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/staticfiles/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/staticfiles/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.869515 django-stubs-4.2.3/django-stubs/contrib/syndication/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/syndication/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      131 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/contrib/syndication/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1889 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/contrib/syndication/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.872848 django-stubs-4.2.3/django-stubs/core/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       98 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/asgi.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.872848 django-stubs-4.2.3/django-stubs/core/cache/
+-rw-r--r--   0 marti     (1000) marti      (121)      624 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/cache/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.876181 django-stubs-4.2.3/django-stubs/core/cache/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/cache/backends/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4121 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/core/cache/backends/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      593 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/cache/backends/db.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      182 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/cache/backends/dummy.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      204 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/cache/backends/filebased.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      180 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/cache/backends/locmem.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      782 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/cache/backends/memcached.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/cache/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.876181 django-stubs-4.2.3/django-stubs/core/checks/
+-rw-r--r--   0 marti     (1000) marti      (121)      652 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/checks/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      265 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/checks/async_checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      529 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/checks/caches.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.876181 django-stubs-4.2.3/django-stubs/core/checks/compatibility/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/checks/compatibility/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      256 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/core/checks/compatibility/django_4_0.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      229 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/checks/database.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      268 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/core/checks/files.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1084 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/checks/messages.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      389 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/checks/model_checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1837 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/core/checks/registry.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.879515 django-stubs-4.2.3/django-stubs/core/checks/security/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/checks/security/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2087 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/core/checks/security/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      514 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/core/checks/security/csrf.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      577 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/checks/security/sessions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      565 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/core/checks/templates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      625 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/checks/translation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      706 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/checks/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1883 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/core/exceptions.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.879515 django-stubs-4.2.3/django-stubs/core/files/
+-rw-r--r--   0 marti     (1000) marti      (121)       68 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/files/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1596 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/core/files/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      359 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/files/images.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      296 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/files/locks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      130 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/files/move.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.882848 django-stubs-4.2.3/django-stubs/core/files/storage/
+-rw-r--r--   0 marti     (1000) marti      (121)      634 2023-06-02 14:08:54.000000 django-stubs-4.2.3/django-stubs/core/files/storage/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1073 2023-06-02 14:08:54.000000 django-stubs-4.2.3/django-stubs/core/files/storage/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      751 2023-06-02 14:08:54.000000 django-stubs-4.2.3/django-stubs/core/files/storage/filesystem.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      450 2023-06-02 14:08:54.000000 django-stubs-4.2.3/django-stubs/core/files/storage/handler.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      725 2023-06-02 14:08:54.000000 django-stubs-4.2.3/django-stubs/core/files/storage/memory.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      338 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/core/files/storage/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/files/temp.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1446 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/core/files/uploadedfile.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3017 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/files/uploadhandler.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      736 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/files/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.882848 django-stubs-4.2.3/django-stubs/core/handlers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/handlers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2043 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/handlers/asgi.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1220 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/handlers/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      770 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/handlers/exception.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1405 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/handlers/wsgi.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.882848 django-stubs-4.2.3/django-stubs/core/mail/
+-rw-r--r--   0 marti     (1000) marti      (121)     1714 2023-06-02 14:08:54.000000 django-stubs-4.2.3/django-stubs/core/mail/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.882848 django-stubs-4.2.3/django-stubs/core/mail/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/mail/backends/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      670 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/core/mail/backends/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      303 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/core/mail/backends/console.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/mail/backends/dummy.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/mail/backends/filebased.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/mail/backends/locmem.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      395 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/mail/backends/smtp.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4640 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/core/mail/message.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       95 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/mail/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.886181 django-stubs-4.2.3/django-stubs/core/management/
+-rw-r--r--   0 marti     (1000) marti      (121)      829 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3617 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/core/management/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1099 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/color.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.889515 django-stubs-4.2.3/django-stubs/core/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      179 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/check.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      430 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/compilemessages.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      284 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/createcachetable.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/dbshell.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      519 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/diffsettings.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      123 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/dumpdata.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      177 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/flush.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      789 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/inspectdb.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1140 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/loaddata.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1227 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/makemessages.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      467 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/makemigrations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      643 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/migrate.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      515 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/runserver.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      111 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/sendtestemail.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      268 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/shell.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      371 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/showmigrations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      110 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/sqlflush.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      203 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/sqlmigrate.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       83 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/sqlsequencereset.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      330 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/squashmigrations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      124 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/startapp.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      124 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/startproject.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      232 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/test.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/commands/testserver.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      488 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/sql.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      964 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/templates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      850 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/management/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2229 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/core/paginator.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.892848 django-stubs-4.2.3/django-stubs/core/serializers/
+-rw-r--r--   0 marti     (1000) marti      (121)     1437 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/serializers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3193 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/core/serializers/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      577 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/serializers/json.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/serializers/jsonl.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      490 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/serializers/python.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      831 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/serializers/pyyaml.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2321 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/core/serializers/xml_serializer.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.892848 django-stubs-4.2.3/django-stubs/core/servers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/servers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1165 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/servers/basehttp.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      139 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/signals.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1846 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/signing.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4218 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/core/validators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       98 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/core/wsgi.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.892848 django-stubs-4.2.3/django-stubs/db/
+-rw-r--r--   0 marti     (1000) marti      (121)     1047 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.892848 django-stubs-4.2.3/django-stubs/db/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.896181 django-stubs-4.2.3/django-stubs/db/backends/base/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/base/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5269 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/db/backends/base/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      555 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/base/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1132 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/base/creation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5118 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/backends/base/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1870 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/backends/base/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     7157 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/backends/base/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3559 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/db/backends/base/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      389 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/base/validation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3134 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/ddl_references.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.896181 django-stubs-4.2.3/django-stubs/db/backends/dummy/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/dummy/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      924 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/backends/dummy/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      176 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/dummy/features.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.896181 django-stubs-4.2.3/django-stubs/db/backends/mysql/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/mysql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2493 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/backends/mysql/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      473 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/backends/mysql/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      734 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/mysql/compiler.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      255 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/mysql/creation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3434 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/mysql/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      568 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/backends/mysql/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2872 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/backends/mysql/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      902 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/mysql/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      354 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/mysql/validation.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.899515 django-stubs-4.2.3/django-stubs/db/backends/oracle/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/oracle/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2711 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/oracle/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      546 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/oracle/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      373 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/oracle/creation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1923 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/oracle/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/oracle/functions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      351 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/backends/oracle/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3990 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/backends/oracle/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      924 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/oracle/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      511 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/oracle/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      308 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/oracle/validation.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.899515 django-stubs-4.2.3/django-stubs/db/backends/postgresql/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/postgresql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1382 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/postgresql/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      524 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/postgresql/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      208 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/postgresql/creation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2197 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/postgresql/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      304 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/backends/postgresql/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      529 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/backends/postgresql/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      809 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/postgresql/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       63 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/signals.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.902848 django-stubs-4.2.3/django-stubs/db/backends/sqlite3/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/sqlite3/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1052 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/sqlite3/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      441 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/sqlite3/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      322 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/sqlite3/creation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      205 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/sqlite3/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      432 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/sqlite3/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1014 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/backends/sqlite3/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      215 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/backends/sqlite3/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2849 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/db/backends/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.906181 django-stubs-4.2.3/django-stubs/db/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)      265 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2830 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/migrations/autodetector.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      664 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/migrations/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1739 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/migrations/executor.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2404 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/migrations/graph.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1960 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/migrations/loader.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1107 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/db/migrations/migration.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.906181 django-stubs-4.2.3/django-stubs/db/migrations/operations/
+-rw-r--r--   0 marti     (1000) marti      (121)     1159 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/migrations/operations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1522 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/migrations/operations/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1251 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/migrations/operations/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5342 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/migrations/operations/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2043 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/migrations/operations/special.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      974 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/migrations/operations/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      290 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/migrations/optimizer.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1109 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/migrations/questioner.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      755 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/migrations/recorder.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1835 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/migrations/serializer.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4952 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/migrations/state.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      195 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/migrations/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1235 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/migrations/writer.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.912848 django-stubs-4.2.3/django-stubs/db/models/
+-rw-r--r--   0 marti     (1000) marti      (121)     5016 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/models/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      684 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/models/aggregates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3677 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/db/models/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       96 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/models/constants.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2250 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/db/models/constraints.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3475 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/models/deletion.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1074 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/models/enums.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    10011 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/db/models/expressions.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.912848 django-stubs-4.2.3/django-stubs/db/models/fields/
+-rw-r--r--   0 marti     (1000) marti      (121)    21217 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/db/models/fields/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3997 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/db/models/fields/files.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3500 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/db/models/fields/json.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      515 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/models/fields/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      161 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/models/fields/proxy.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    10666 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/db/models/fields/related.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3463 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/models/fields/related_descriptors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1393 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/models/fields/related_lookups.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4576 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/models/fields/reverse_related.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.916181 django-stubs-4.2.3/django-stubs/db/models/functions/
+-rw-r--r--   0 marti     (1000) marti      (121)     3378 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/models/functions/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      547 2023-04-27 12:45:58.000000 django-stubs-4.2.3/django-stubs/db/models/functions/comparison.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1343 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/models/functions/datetime.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1222 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/models/functions/math.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/models/functions/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4623 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/models/functions/text.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      918 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/models/functions/window.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2228 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/models/indexes.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5852 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/db/models/lookups.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     8444 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/db/models/manager.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5363 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/models/options.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    10730 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/db/models/query.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3277 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/models/query_utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      888 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/models/signals.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.919515 django-stubs-4.2.3/django-stubs/db/models/sql/
+-rw-r--r--   0 marti     (1000) marti      (121)      284 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/models/sql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6507 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/models/sql/compiler.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      286 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/models/sql/constants.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1791 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/models/sql/datastructures.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     9499 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/models/sql/query.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1619 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/db/models/sql/subqueries.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2075 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/models/sql/where.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      473 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/models/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2178 2023-06-02 14:08:54.000000 django-stubs-4.2.3/django-stubs/db/transaction.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2061 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/db/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.919515 django-stubs-4.2.3/django-stubs/dispatch/
+-rw-r--r--   0 marti     (1000) marti      (121)      116 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/dispatch/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1251 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/dispatch/dispatcher.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.919515 django-stubs-4.2.3/django-stubs/forms/
+-rw-r--r--   0 marti     (1000) marti      (121)     4083 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/forms/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2874 2023-04-27 12:45:58.000000 django-stubs-4.2.3/django-stubs/forms/boundfield.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    20422 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/forms/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3196 2023-04-27 12:45:58.000000 django-stubs-4.2.3/django-stubs/forms/forms.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3777 2023-04-27 12:45:58.000000 django-stubs-4.2.3/django-stubs/forms/formsets.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    12444 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/forms/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1125 2023-04-27 12:45:58.000000 django-stubs-4.2.3/django-stubs/forms/renderers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2337 2023-04-27 12:45:58.000000 django-stubs-4.2.3/django-stubs/forms/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    10456 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/forms/widgets.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.922848 django-stubs-4.2.3/django-stubs/http/
+-rw-r--r--   0 marti     (1000) marti      (121)     1332 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/http/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       96 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/http/cookie.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1979 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/http/multipartparser.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     8313 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/http/request.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5819 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/http/response.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.922848 django-stubs-4.2.3/django-stubs/middleware/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/middleware/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1063 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/middleware/cache.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      387 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/middleware/clickjacking.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      968 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/middleware/common.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1098 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/middleware/csrf.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      339 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/middleware/gzip.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      369 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/middleware/http.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      417 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/middleware/locale.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      645 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/middleware/security.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1514 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/shortcuts.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.926181 django-stubs-4.2.3/django-stubs/template/
+-rw-r--r--   0 marti     (1000) marti      (121)      756 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.926181 django-stubs-4.2.3/django-stubs/template/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/backends/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      876 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/template/backends/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1062 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/backends/django.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      432 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/backends/dummy.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      872 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/template/backends/jinja2.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      215 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/backends/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5644 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/template/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3368 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/template/context.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      631 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/context_processors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3483 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/defaultfilters.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6912 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/defaulttags.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2158 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/engine.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      511 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3244 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/library.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      684 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/loader.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2267 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/template/loader_tags.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.929514 django-stubs-4.2.3/django-stubs/template/loaders/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/loaders/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       88 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/loaders/app_directories.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      488 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/loaders/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      554 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/loaders/cached.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      518 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/loaders/filesystem.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      323 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/loaders/locmem.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2564 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/response.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1246 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/smartif.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      589 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/template/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.929514 django-stubs-4.2.3/django-stubs/templatetags/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      629 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/templatetags/cache.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3492 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/templatetags/i18n.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      410 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/templatetags/l10n.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1123 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/templatetags/static.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1076 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/templatetags/tz.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.929514 django-stubs-4.2.3/django-stubs/test/
+-rw-r--r--   0 marti     (1000) marti      (121)      848 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/test/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     9121 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/test/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1148 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/test/html.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6591 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/test/runner.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      539 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/test/selenium.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      905 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/test/signals.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    10489 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/test/testcases.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6287 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/test/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.932848 django-stubs-4.2.3/django-stubs/urls/
+-rw-r--r--   0 marti     (1000) marti      (121)     1576 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/urls/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      857 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/urls/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1349 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/urls/conf.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      778 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/urls/converters.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      102 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/urls/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4722 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/urls/resolvers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      157 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/urls/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.939514 django-stubs-4.2.3/django-stubs/utils/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/_os.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1487 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/utils/archive.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      230 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/asyncio.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2872 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/autoreload.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      591 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/baseconv.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1287 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/cache.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1300 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/connection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      570 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/crypto.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4673 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/utils/datastructures.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2033 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/dateformat.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      505 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/dateparse.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      156 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/dates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      547 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/datetime_safe.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      325 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/deconstruct.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      876 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1776 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/utils/deprecation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/duration.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3177 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/encoding.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2676 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/feedgenerator.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1814 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/formats.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4505 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/utils/functional.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       66 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/hashable.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2481 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/html.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1283 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/http.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      483 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/inspect.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      175 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/ipv6.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       61 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/itercompat.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      714 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/jslex.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1692 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/log.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      242 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/lorem_ipsum.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      312 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/module_loading.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      319 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/numberformat.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      917 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/regex_helper.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      589 2023-06-29 17:05:25.000000 django-stubs-4.2.3/django-stubs/utils/safestring.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      557 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/termcolors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1933 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/text.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      423 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/timesince.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2011 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/timezone.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      309 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/topological_sort.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.939514 django-stubs-4.2.3/django-stubs/utils/translation/
+-rw-r--r--   0 marti     (1000) marti      (121)     2033 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/translation/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/translation/reloader.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      335 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/translation/template.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      801 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/translation/trans_null.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2986 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/translation/trans_real.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      986 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/tree.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      518 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/utils/version.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      379 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/utils/xmlutils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.942848 django-stubs-4.2.3/django-stubs/views/
+-rw-r--r--   0 marti     (1000) marti      (121)       39 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/views/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/views/csrf.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2741 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/views/debug.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.942848 django-stubs-4.2.3/django-stubs/views/decorators/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/views/decorators/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      347 2023-06-02 14:08:54.000000 django-stubs-4.2.3/django-stubs/views/decorators/cache.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/views/decorators/clickjacking.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      162 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/views/decorators/common.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      427 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/views/decorators/csrf.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      259 2023-06-02 14:08:54.000000 django-stubs-4.2.3/django-stubs/views/decorators/debug.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      146 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/views/decorators/gzip.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      718 2023-06-02 14:08:54.000000 django-stubs-4.2.3/django-stubs/views/decorators/http.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      218 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/views/decorators/vary.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      782 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/views/defaults.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.946181 django-stubs-4.2.3/django-stubs/views/generic/
+-rw-r--r--   0 marti     (1000) marti      (121)      797 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/views/generic/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2272 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/views/generic/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4525 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/views/generic/dates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1109 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/views/generic/detail.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3393 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/views/generic/edit.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1819 2023-06-27 17:49:10.000000 django-stubs-4.2.3/django-stubs/views/generic/list.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1035 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/views/i18n.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      482 2023-03-15 16:53:32.000000 django-stubs-4.2.3/django-stubs/views/static.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.946181 django-stubs-4.2.3/django_stubs.egg-info/
+-rw-r--r--   0 marti     (1000) marti      (121)    15960 2023-06-29 17:11:02.000000 django-stubs-4.2.3/django_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)    30431 2023-06-29 17:11:02.000000 django-stubs-4.2.3/django_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 marti     (1000) marti      (121)        1 2023-06-29 17:11:02.000000 django-stubs-4.2.3/django_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 marti     (1000) marti      (121)      150 2023-06-29 17:11:02.000000 django-stubs-4.2.3/django_stubs.egg-info/requires.txt
+-rw-r--r--   0 marti     (1000) marti      (121)       32 2023-06-29 17:11:02.000000 django-stubs-4.2.3/django_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.946181 django-stubs-4.2.3/mypy_django_plugin/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/mypy_django_plugin/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)     4295 2023-06-27 17:49:10.000000 django-stubs-4.2.3/mypy_django_plugin/config.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.946181 django-stubs-4.2.3/mypy_django_plugin/django/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/mypy_django_plugin/django/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)    21278 2023-06-29 17:05:25.000000 django-stubs-4.2.3/mypy_django_plugin/django/context.py
+-rw-r--r--   0 marti     (1000) marti      (121)      227 2023-03-15 16:53:32.000000 django-stubs-4.2.3/mypy_django_plugin/errorcodes.py
+-rw-r--r--   0 marti     (1000) marti      (121)       89 2023-06-27 17:49:10.000000 django-stubs-4.2.3/mypy_django_plugin/exceptions.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.946181 django-stubs-4.2.3/mypy_django_plugin/lib/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/mypy_django_plugin/lib/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)     2289 2023-04-27 12:45:58.000000 django-stubs-4.2.3/mypy_django_plugin/lib/fullnames.py
+-rw-r--r--   0 marti     (1000) marti      (121)    13634 2023-06-27 17:49:10.000000 django-stubs-4.2.3/mypy_django_plugin/lib/helpers.py
+-rw-r--r--   0 marti     (1000) marti      (121)    15544 2023-06-27 17:49:10.000000 django-stubs-4.2.3/mypy_django_plugin/main.py
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/mypy_django_plugin/py.typed
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.949514 django-stubs-4.2.3/mypy_django_plugin/transformers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.3/mypy_django_plugin/transformers/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)     9704 2023-06-27 17:49:10.000000 django-stubs-4.2.3/mypy_django_plugin/transformers/fields.py
+-rw-r--r--   0 marti     (1000) marti      (121)     1787 2023-06-27 17:49:10.000000 django-stubs-4.2.3/mypy_django_plugin/transformers/forms.py
+-rw-r--r--   0 marti     (1000) marti      (121)     1313 2023-06-27 17:49:10.000000 django-stubs-4.2.3/mypy_django_plugin/transformers/functional.py
+-rw-r--r--   0 marti     (1000) marti      (121)     3104 2023-03-15 16:53:32.000000 django-stubs-4.2.3/mypy_django_plugin/transformers/init_create.py
+-rw-r--r--   0 marti     (1000) marti      (121)    20857 2023-06-27 17:49:10.000000 django-stubs-4.2.3/mypy_django_plugin/transformers/managers.py
+-rw-r--r--   0 marti     (1000) marti      (121)     1938 2023-06-27 17:49:10.000000 django-stubs-4.2.3/mypy_django_plugin/transformers/meta.py
+-rw-r--r--   0 marti     (1000) marti      (121)    32337 2023-06-29 17:05:25.000000 django-stubs-4.2.3/mypy_django_plugin/transformers/models.py
+-rw-r--r--   0 marti     (1000) marti      (121)     2826 2023-06-27 17:49:10.000000 django-stubs-4.2.3/mypy_django_plugin/transformers/orm_lookups.py
+-rw-r--r--   0 marti     (1000) marti      (121)    13086 2023-06-27 17:49:10.000000 django-stubs-4.2.3/mypy_django_plugin/transformers/querysets.py
+-rw-r--r--   0 marti     (1000) marti      (121)     2048 2023-06-27 17:49:10.000000 django-stubs-4.2.3/mypy_django_plugin/transformers/request.py
+-rw-r--r--   0 marti     (1000) marti      (121)     2495 2023-06-27 17:49:10.000000 django-stubs-4.2.3/mypy_django_plugin/transformers/settings.py
+-rw-r--r--   0 marti     (1000) marti      (121)      723 2023-06-29 17:05:25.000000 django-stubs-4.2.3/pyproject.toml
+-rw-r--r--   0 marti     (1000) marti      (121)      308 2023-06-29 17:11:02.952848 django-stubs-4.2.3/setup.cfg
+-rw-r--r--   0 marti     (1000) marti      (121)     2233 2023-06-29 17:05:25.000000 django-stubs-4.2.3/setup.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-29 17:11:02.949514 django-stubs-4.2.3/tests/
+-rw-r--r--   0 marti     (1000) marti      (121)     5766 2023-06-27 17:49:10.000000 django-stubs-4.2.3/tests/test_error_handling.py
```

### Comparing `django-stubs-4.2.2/LICENSE.md` & `django-stubs-4.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/PKG-INFO` & `django-stubs-4.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-stubs
-Version: 4.2.2
+Version: 4.2.3
 Summary: Mypy stubs for Django
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
@@ -72,14 +72,15 @@
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
 | django-stubs   | Mypy version | Django version | Django partial support | Python version |
 |----------------|--------------|----------------|------------------------|----------------|
+| 4.2.3          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.2          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.1          | 1.3.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.0          | 1.2.x        | 4.2            | 4.1, 4.0, 3.2          | 3.7 - 3.11     |
 | 1.16.0         | 1.1.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 | 1.15.0         | 1.0.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 | 1.14.0         | 0.990+       | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
```

### Comparing `django-stubs-4.2.2/README.md` & `django-stubs-4.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
 | django-stubs   | Mypy version | Django version | Django partial support | Python version |
 |----------------|--------------|----------------|------------------------|----------------|
+| 4.2.3          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.2          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.1          | 1.3.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.0          | 1.2.x        | 4.2            | 4.1, 4.0, 3.2          | 3.7 - 3.11     |
 | 1.16.0         | 1.1.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 | 1.15.0         | 1.0.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 | 1.14.0         | 0.990+       | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
```

### Comparing `django-stubs-4.2.2/django-stubs/apps/config.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/base/creation.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-import types
-from collections.abc import Iterator
+from typing import Any
 
-from django.apps.registry import Apps
-from django.db.models.base import Model
-from django.utils.functional import _StrOrPromise, cached_property
+from django.db.backends.base.base import BaseDatabaseWrapper
 
-APPS_MODULE_NAME: str
-MODELS_MODULE_NAME: str
+TEST_DATABASE_PREFIX: str
 
-class AppConfig:
-    name: str
-    module: types.ModuleType | None
-    apps: Apps | None
-    label: str
-    verbose_name: _StrOrPromise
-    path: str
-    models_module: str | None
-    models: dict[str, type[Model]]
-    def __init__(self, app_name: str, app_module: types.ModuleType | None) -> None: ...
-    @cached_property
-    def default_auto_field(self) -> str: ...
-    @classmethod
-    def create(cls, entry: str) -> AppConfig: ...
-    def get_model(self, model_name: str, require_ready: bool = ...) -> type[Model]: ...
-    def get_models(self, include_auto_created: bool = ..., include_swapped: bool = ...) -> Iterator[type[Model]]: ...
-    def import_models(self) -> None: ...
-    def ready(self) -> None: ...
+class BaseDatabaseCreation:
+    connection: BaseDatabaseWrapper
+    def __init__(self, connection: BaseDatabaseWrapper) -> None: ...
+    def create_test_db(
+        self, verbosity: int = ..., autoclobber: bool = ..., serialize: bool = ..., keepdb: bool = ...
+    ) -> str: ...
+    def set_as_test_mirror(self, primary_settings_dict: dict[str, dict[str, None] | int | str | None]) -> None: ...
+    def serialize_db_to_string(self) -> str: ...
+    def deserialize_db_from_string(self, data: str) -> None: ...
+    def clone_test_db(self, suffix: Any, verbosity: int = ..., autoclobber: bool = ..., keepdb: bool = ...) -> None: ...
+    def get_test_db_clone_settings(self, suffix: str) -> dict[str, Any]: ...
+    def destroy_test_db(
+        self,
+        old_database_name: str | None = ...,
+        verbosity: int = ...,
+        keepdb: bool = ...,
+        suffix: str | None = ...,
+    ) -> None: ...
+    def sql_table_creation_suffix(self) -> str: ...
+    def test_db_signature(self) -> tuple[str, str, str, str]: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/apps/registry.pyi` & `django-stubs-4.2.3/django-stubs/apps/registry.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/conf/__init__.pyi` & `django-stubs-4.2.3/django-stubs/conf/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Literal
 
-from _typeshed import Self
 from django.utils.functional import LazyObject
+from typing_extensions import Self
 
 # explicit dependency on standard settings to make it loaded
 from . import global_settings  # noqa: F401
 
 ENVIRONMENT_VARIABLE: Literal["DJANGO_SETTINGS_MODULE"]
 DEFAULT_STORAGE_ALIAS: Literal["default"]
 STATICFILES_STORAGE_ALIAS: Literal["staticfiles"]
@@ -32,9 +32,9 @@
     def __init__(self, default_settings: Any) -> None: ...
     def __getattr__(self, name: str) -> Any: ...
     def __setattr__(self, name: str, value: Any) -> None: ...
     def __delattr__(self, name: str) -> None: ...
     def is_overridden(self, setting: str) -> bool: ...
 
 class SettingsReference(str):
-    def __new__(self: type[Self], value: Any, setting_name: str) -> Self: ...
+    def __new__(self, value: Any, setting_name: str) -> Self: ...
     def __init__(self, value: str, setting_name: str) -> None: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/conf/global_settings.pyi` & `django-stubs-4.2.3/django-stubs/conf/global_settings.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/conf/urls/__init__.pyi` & `django-stubs-4.2.3/django-stubs/conf/urls/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admin/__init__.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admin/checks.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admin/checks.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admin/decorators.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admin/decorators.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admin/filters.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admin/filters.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admin/helpers.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admin/helpers.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admin/models.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admin/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admin/options.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admin/options.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admin/sites.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admin/sites.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/admin_list.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admin/templatetags/admin_list.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/admin_modify.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admin/templatetags/admin_modify.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/base.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admin/templatetags/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admin/tests.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admin/tests.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admin/utils.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admin/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admin/views/main.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admin/views/main.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admin/widgets.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admin/widgets.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admindocs/utils.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admindocs/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/admindocs/views.pyi` & `django-stubs-4.2.3/django-stubs/contrib/admindocs/views.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/auth/__init__.pyi` & `django-stubs-4.2.3/django-stubs/contrib/auth/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/auth/backends.pyi` & `django-stubs-4.2.3/django-stubs/contrib/auth/backends.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/auth/base_user.pyi` & `django-stubs-4.2.3/django-stubs/contrib/auth/base_user.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/auth/context_processors.pyi` & `django-stubs-4.2.3/django-stubs/contrib/auth/context_processors.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/auth/decorators.pyi` & `django-stubs-4.2.3/django-stubs/contrib/auth/decorators.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from django.http.response import HttpResponseBase
 
 _VIEW = TypeVar("_VIEW", bound=Callable[..., HttpResponseBase])
 
 def user_passes_test(
     test_func: Callable[[AbstractBaseUser | AnonymousUser], bool],
     login_url: str | None = ...,
-    redirect_field_name: str = ...,
+    redirect_field_name: str | None = ...,
 ) -> Callable[[_VIEW], _VIEW]: ...
 
 # There are two ways of calling @login_required: @with(arguments) and @bare
 @overload
-def login_required(redirect_field_name: str = ..., login_url: str | None = ...) -> Callable[[_VIEW], _VIEW]: ...
+def login_required(redirect_field_name: str | None = ..., login_url: str | None = ...) -> Callable[[_VIEW], _VIEW]: ...
 @overload
-def login_required(function: _VIEW, redirect_field_name: str = ..., login_url: str | None = ...) -> _VIEW: ...
+def login_required(function: _VIEW, redirect_field_name: str | None = ..., login_url: str | None = ...) -> _VIEW: ...
 def permission_required(
     perm: Iterable[str] | str, login_url: str | None = ..., raise_exception: bool = ...
 ) -> Callable[[_VIEW], _VIEW]: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/contrib/auth/forms.pyi` & `django-stubs-4.2.3/django-stubs/contrib/auth/forms.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/auth/hashers.pyi` & `django-stubs-4.2.3/django-stubs/contrib/auth/hashers.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/auth/middleware.pyi` & `django-stubs-4.2.3/django-stubs/contrib/auth/middleware.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/auth/mixins.pyi` & `django-stubs-4.2.3/django-stubs/contrib/auth/mixins.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/auth/models.pyi` & `django-stubs-4.2.3/django-stubs/contrib/auth/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/auth/password_validation.pyi` & `django-stubs-4.2.3/django-stubs/contrib/auth/password_validation.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/auth/tokens.pyi` & `django-stubs-4.2.3/django-stubs/contrib/auth/tokens.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/auth/views.pyi` & `django-stubs-4.2.3/django-stubs/contrib/auth/views.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/contenttypes/admin.pyi` & `django-stubs-4.2.3/django-stubs/contrib/contenttypes/admin.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/contenttypes/fields.pyi` & `django-stubs-4.2.3/django-stubs/contrib/contenttypes/fields.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/contenttypes/forms.pyi` & `django-stubs-4.2.3/django-stubs/contrib/contenttypes/forms.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/contenttypes/management/__init__.pyi` & `django-stubs-4.2.3/django-stubs/contrib/contenttypes/management/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/contenttypes/models.pyi` & `django-stubs-4.2.3/django-stubs/contrib/contenttypes/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/admin/__init__.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/admin/options.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/admin/options.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/features.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/base/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/models.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/base/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/operations.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/base/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/features.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/mysql/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/operations.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/mysql/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/schema.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/mysql/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/models.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/oracle/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/operations.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/oracle/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/schema.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/oracle/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/models.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/postgis/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/operations.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/postgis/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/base.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/spatialite/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/models.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/spatialite/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/utils.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/backends/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/models/__init__.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/models/aggregates.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/models/aggregates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/models/fields.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/models/fields.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/models/functions.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/models/functions.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/models/lookups.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/models/lookups.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/db/models/sql/conversion.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/db/models/sql/conversion.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/feeds.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/feeds.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/forms/__init__.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/forms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/forms/fields.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/forms/fields.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/forms/widgets.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/forms/widgets.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/__init__.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/gdal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/datasource.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/gdal/datasource.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/envelope.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/gdal/envelope.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/feature.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/gdal/feature.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/field.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/gdal/field.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/geometries.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/gdal/geometries.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/layer.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/gdal/layer.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/ds.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/gdal/prototypes/ds.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/generation.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/gdal/prototypes/generation.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/geom.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/gdal/prototypes/geom.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/raster.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/gdal/prototypes/raster.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/srs.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/gdal/prototypes/srs.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/raster/band.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/gdal/raster/band.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/raster/source.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/gdal/raster/source.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/srs.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/gdal/srs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from enum import IntEnum
 from typing import Any, AnyStr
 
-from _typeshed import Self
 from django.contrib.gis.gdal.base import GDALBase
+from typing_extensions import Self
 
 class AxisOrder(IntEnum):
     TRADITIONAL: int
     AUTHORITY: int
 
 class SpatialReference(GDALBase):
     destructor: Any
     axis_order: AxisOrder
     ptr: Any
     def __init__(self, srs_input: str | int = ..., srs_type: str = ..., axis_order: AxisOrder | None = ...) -> None: ...
     def __getitem__(self, target: str | tuple[str, int]) -> str: ...
     def attr_value(self, target: AnyStr, index: int = ...) -> str: ...
     def auth_name(self, target: AnyStr) -> str: ...
     def auth_code(self, target: AnyStr) -> str: ...
-    def clone(self: Self) -> Self: ...
+    def clone(self) -> Self: ...
     def from_esri(self) -> None: ...
     def identify_epsg(self) -> None: ...
     def to_esri(self) -> None: ...
     def validate(self) -> None: ...
     @property
     def name(self) -> str | None: ...
     @property
```

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geoip2/base.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geoip2/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geos/__init__.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geos/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geos/collections.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geos/collections.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geos/coordseq.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geos/coordseq.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections.abc import Iterator
 from typing import Any
 
-from _typeshed import Self
 from django.contrib.gis.geos.base import GEOSBase
+from typing_extensions import Self
 
 class GEOSCoordSeq(GEOSBase):
     ptr_type: Any
     def __init__(self, ptr: Any, z: bool = ...) -> None: ...
     def __iter__(self) -> Iterator[tuple[float, ...]]: ...
     def __len__(self) -> int: ...
     def __getitem__(self, index: int) -> Any: ...
@@ -21,14 +21,14 @@
     def setZ(self, index: int, value: float) -> None: ...
     @property
     def size(self) -> int: ...
     @property
     def dims(self) -> int: ...
     @property
     def hasz(self) -> bool: ...
-    def clone(self: Self) -> Self: ...
+    def clone(self) -> Self: ...
     @property
     def kml(self) -> str: ...
     @property
     def tuple(self) -> tuple[Any, ...]: ...
     @property
     def is_counterclockwise(self) -> bool: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geos/geometry.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geos/geometry.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Any
 
-from _typeshed import Self
 from django.contrib.gis.gdal import CoordTransform, SpatialReference
 from django.contrib.gis.gdal.geometries import OGRGeometry
 from django.contrib.gis.geos.base import GEOSBase
 from django.contrib.gis.geos.coordseq import GEOSCoordSeq
 from django.contrib.gis.geos.mutable_list import ListMixin
 from django.contrib.gis.geos.point import Point
 from django.contrib.gis.geos.prepared import PreparedGeometry
+from typing_extensions import Self
 
 class GEOSGeometryBase(GEOSBase):
     ptr_type: Any
     destructor: Any
     has_cs: bool
     def __init__(self, ptr: Any, cls: Any) -> None: ...
-    def __copy__(self: Self) -> Self: ...
-    def __deepcopy__(self: Self, memodict: Any) -> Self: ...
+    def __copy__(self) -> Self: ...
+    def __deepcopy__(self, memodict: Any) -> Self: ...
     @staticmethod
     def from_ewkt(ewkt: str) -> GEOSGeometry: ...
     @classmethod
     def from_gml(cls, gml_string: str) -> GEOSGeometry: ...
     def __eq__(self, other: object) -> bool: ...
     def __hash__(self) -> int: ...
     def __or__(self, other: GEOSGeometry) -> GEOSGeometry: ...
@@ -125,15 +125,15 @@
     @property
     def area(self) -> float: ...
     def distance(self, other: GEOSGeometry) -> float: ...
     @property
     def extent(self) -> tuple[float, float, float, float]: ...
     @property
     def length(self) -> float: ...
-    def clone(self: Self) -> Self: ...
+    def clone(self) -> Self: ...
 
 class LinearGeometryMixin:
     def interpolate(self, distance: float) -> Point: ...
     def interpolate_normalized(self, distance: float) -> Point: ...
     def project(self, point: Point) -> float: ...
     def project_normalized(self, point: Point) -> float: ...
     @property
```

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geos/libgeos.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geos/libgeos.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geos/linestring.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geos/linestring.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geos/mutable_list.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geos/mutable_list.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Any
 
-from _typeshed import Self
+from typing_extensions import Self
 
 class ListMixin:
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
     def __getitem__(self, index: int | slice) -> Any: ...
     def __delitem__(self, index: int | slice) -> None: ...
     def __setitem__(self, index: int | slice, val: Any) -> None: ...
-    def __add__(self: Self, other: Any) -> Self: ...
+    def __add__(self, other: Any) -> Self: ...
     def __radd__(self, other: Any) -> Any: ...
-    def __iadd__(self: Self, other: Any) -> Self: ...
-    def __mul__(self: Self, n: int) -> Self: ...
-    def __rmul__(self: Self, n: int) -> Self: ...
-    def __imul__(self: Self, n: int) -> Self: ...
+    def __iadd__(self, other: Any) -> Self: ...
+    def __mul__(self, n: int) -> Self: ...
+    def __rmul__(self, n: int) -> Self: ...
+    def __imul__(self, n: int) -> Self: ...
     def __eq__(self, other: object) -> bool: ...
     def __lt__(self, other: Any) -> bool: ...
     def count(self, val: Any) -> int: ...
     def index(self, val: Any) -> int: ...
     def append(self, val: Any) -> None: ...
     def extend(self, vals: Any) -> None: ...
     def insert(self, index: int, val: Any) -> None: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geos/point.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geos/point.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geos/polygon.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geos/polygon.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geos/prepared.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geos/prepared.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/__init__.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/geom.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/geom.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/io.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/io.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/predicates.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/predicates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/topology.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/geos/prototypes/topology.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/measure.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/measure.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from decimal import Decimal
 from typing import Any
 
-from _typeshed import Self
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 _NUMERIC_TYPES: TypeAlias = int | float | Decimal
 
 class MeasureBase:
     STANDARD_UNIT: str | None
     UNITS: dict[str, float]
     ALIAS: dict[str, str]
     LALIAS: dict[str, str]
     def __init__(self, default_unit: str | None = ..., **kwargs: Any) -> None: ...
     standard: Any
     def __getattr__(self, name: str) -> float: ...
     def __eq__(self, other: object) -> bool: ...
-    def __lt__(self: Self, other: Self) -> bool: ...
-    def __add__(self: Self, other: Self) -> Self: ...
-    def __iadd__(self: Self, other: Self) -> Self: ...
-    def __sub__(self: Self, other: Self) -> Self: ...
-    def __isub__(self: Self, other: Self) -> Self: ...
+    def __lt__(self, other: Self) -> bool: ...
+    def __add__(self, other: Self) -> Self: ...
+    def __iadd__(self, other: Self) -> Self: ...
+    def __sub__(self, other: Self) -> Self: ...
+    def __isub__(self, other: Self) -> Self: ...
     def __mul__(self, other: _NUMERIC_TYPES) -> Any: ...
-    def __imul__(self: Self, other: _NUMERIC_TYPES) -> Self: ...
-    def __rmul__(self: Self, other: Any) -> Self: ...
-    def __truediv__(self: Self, other: _NUMERIC_TYPES) -> Self: ...
-    def __itruediv__(self: Self, other: _NUMERIC_TYPES) -> Self: ...
+    def __imul__(self, other: _NUMERIC_TYPES) -> Self: ...
+    def __rmul__(self, other: Any) -> Self: ...
+    def __truediv__(self, other: _NUMERIC_TYPES) -> Self: ...
+    def __itruediv__(self, other: _NUMERIC_TYPES) -> Self: ...
     def __bool__(self) -> bool: ...
     def default_units(self, kwargs: dict[str, Any]) -> tuple[float, str]: ...
     @classmethod
     def unit_attname(cls, unit_str: str) -> str: ...
 
 class Distance(MeasureBase):
     STANDARD_UNIT: str
```

### Comparing `django-stubs-4.2.2/django-stubs/contrib/gis/utils/layermapping.pyi` & `django-stubs-4.2.3/django-stubs/contrib/gis/utils/layermapping.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/humanize/templatetags/humanize.pyi` & `django-stubs-4.2.3/django-stubs/contrib/humanize/templatetags/humanize.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/messages/__init__.pyi` & `django-stubs-4.2.3/django-stubs/contrib/messages/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/messages/api.pyi` & `django-stubs-4.2.3/django-stubs/contrib/messages/api.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/messages/storage/base.pyi` & `django-stubs-4.2.3/django-stubs/contrib/messages/storage/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/postgres/aggregates/__init__.pyi` & `django-stubs-4.2.3/django-stubs/contrib/postgres/aggregates/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/postgres/constraints.pyi` & `django-stubs-4.2.3/django-stubs/contrib/postgres/constraints.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/postgres/fields/__init__.pyi` & `django-stubs-4.2.3/django-stubs/contrib/postgres/fields/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/postgres/fields/array.pyi` & `django-stubs-4.2.3/django-stubs/contrib/postgres/fields/array.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/postgres/fields/hstore.pyi` & `django-stubs-4.2.3/django-stubs/contrib/postgres/fields/hstore.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/postgres/fields/ranges.pyi` & `django-stubs-4.2.3/django-stubs/contrib/postgres/fields/ranges.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/postgres/forms/array.pyi` & `django-stubs-4.2.3/django-stubs/contrib/postgres/forms/array.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/postgres/forms/ranges.pyi` & `django-stubs-4.2.3/django-stubs/contrib/postgres/forms/ranges.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/postgres/indexes.pyi` & `django-stubs-4.2.3/django-stubs/contrib/postgres/indexes.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/postgres/lookups.pyi` & `django-stubs-4.2.3/django-stubs/contrib/postgres/lookups.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/postgres/operations.pyi` & `django-stubs-4.2.3/django-stubs/contrib/postgres/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/postgres/search.pyi` & `django-stubs-4.2.3/django-stubs/contrib/postgres/search.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Any
 
-from _typeshed import Self
 from django.db.models import Expression, Field
 from django.db.models.expressions import Combinable, CombinedExpression, Func
 from django.db.models.lookups import Lookup
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 _Expression: TypeAlias = str | Combinable | SearchQueryCombinable
 
 class SearchVectorExact(Lookup): ...
 class SearchVectorField(Field): ...
 class SearchQueryField(Field): ...
 
@@ -39,31 +38,31 @@
         config: _Expression | None,
         output_field: Field | None = ...,
     ) -> None: ...
 
 class SearchQueryCombinable:
     BITAND: str
     BITOR: str
-    def __or__(self: Self, other: SearchQueryCombinable) -> Self: ...
-    def __ror__(self: Self, other: SearchQueryCombinable) -> Self: ...
-    def __and__(self: Self, other: SearchQueryCombinable) -> Self: ...
-    def __rand__(self: Self, other: SearchQueryCombinable) -> Self: ...
+    def __or__(self, other: SearchQueryCombinable) -> Self: ...
+    def __ror__(self, other: SearchQueryCombinable) -> Self: ...
+    def __and__(self, other: SearchQueryCombinable) -> Self: ...
+    def __rand__(self, other: SearchQueryCombinable) -> Self: ...
 
 class SearchQuery(SearchQueryCombinable, Func):  # type: ignore
     SEARCH_TYPES: dict[str, str]
     def __init__(
         self,
         value: _Expression,
         output_field: Field | None = ...,
         *,
         config: _Expression | None = ...,
         invert: bool = ...,
         search_type: str = ...,
     ) -> None: ...
-    def __invert__(self: Self) -> Self: ...  # type: ignore[override]
+    def __invert__(self) -> Self: ...  # type: ignore[override]
 
 class CombinedSearchQuery(SearchQueryCombinable, CombinedExpression):  # type: ignore
     def __init__(
         self,
         lhs: Combinable,
         connector: str,
         rhs: Combinable,
```

### Comparing `django-stubs-4.2.2/django-stubs/contrib/postgres/validators.pyi` & `django-stubs-4.2.3/django-stubs/contrib/postgres/validators.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/sessions/backends/base.pyi` & `django-stubs-4.2.3/django-stubs/contrib/sessions/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/sessions/base_session.pyi` & `django-stubs-4.2.3/django-stubs/contrib/sessions/base_session.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/sitemaps/__init__.pyi` & `django-stubs-4.2.3/django-stubs/contrib/sitemaps/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/sitemaps/views.pyi` & `django-stubs-4.2.3/django-stubs/contrib/sitemaps/views.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/sites/models.pyi` & `django-stubs-4.2.3/django-stubs/contrib/sites/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/staticfiles/finders.pyi` & `django-stubs-4.2.3/django-stubs/contrib/staticfiles/finders.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/staticfiles/handlers.pyi` & `django-stubs-4.2.3/django-stubs/contrib/staticfiles/handlers.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi` & `django-stubs-4.2.3/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/staticfiles/storage.pyi` & `django-stubs-4.2.3/django-stubs/contrib/staticfiles/storage.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/contrib/syndication/views.pyi` & `django-stubs-4.2.3/django-stubs/contrib/syndication/views.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/cache/__init__.pyi` & `django-stubs-4.2.3/django-stubs/core/cache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/cache/backends/base.pyi` & `django-stubs-4.2.3/django-stubs/core/cache/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/cache/backends/db.pyi` & `django-stubs-4.2.3/django-stubs/core/cache/backends/db.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/cache/backends/memcached.pyi` & `django-stubs-4.2.3/django-stubs/core/cache/backends/memcached.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/checks/__init__.pyi` & `django-stubs-4.2.3/django-stubs/core/checks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/checks/caches.pyi` & `django-stubs-4.2.3/django-stubs/core/checks/caches.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/checks/messages.pyi` & `django-stubs-4.2.3/django-stubs/core/checks/messages.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/checks/registry.pyi` & `django-stubs-4.2.3/django-stubs/core/checks/registry.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/checks/security/base.pyi` & `django-stubs-4.2.3/django-stubs/core/checks/security/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/checks/security/csrf.pyi` & `django-stubs-4.2.3/django-stubs/core/checks/security/csrf.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/checks/security/sessions.pyi` & `django-stubs-4.2.3/django-stubs/core/checks/security/sessions.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/checks/templates.pyi` & `django-stubs-4.2.3/django-stubs/core/checks/templates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/checks/translation.pyi` & `django-stubs-4.2.3/django-stubs/core/checks/translation.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/checks/urls.pyi` & `django-stubs-4.2.3/django-stubs/core/checks/urls.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/exceptions.pyi` & `django-stubs-4.2.3/django-stubs/core/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/files/base.pyi` & `django-stubs-4.2.3/django-stubs/core/files/base.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from collections.abc import Iterator
 from types import TracebackType
 from typing import IO, AnyStr, type_check_only
 
-from _typeshed import Self
 from django.core.files.utils import FileProxyMixin
+from typing_extensions import Self
 
 class File(FileProxyMixin[AnyStr], IO[AnyStr]):
     DEFAULT_CHUNK_SIZE: int
     file: IO[AnyStr] | None
     name: str | None  # type: ignore[assignment]
     mode: str
     def __init__(self, file: IO[AnyStr] | None, name: str | None = ...) -> None: ...
     def __bool__(self) -> bool: ...
     def __len__(self) -> int: ...
     @property
     def size(self) -> int: ...
     def chunks(self, chunk_size: int | None = ...) -> Iterator[AnyStr]: ...
     def multiple_chunks(self, chunk_size: int | None = ...) -> bool | None: ...
     def __iter__(self) -> Iterator[AnyStr]: ...
-    def __enter__(self: Self) -> Self: ...
+    def __enter__(self) -> Self: ...
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None: ...
-    def open(self: Self, mode: str | None = ...) -> Self: ...
+    def open(self, mode: str | None = ...) -> Self: ...
     def close(self) -> None: ...
     @type_check_only
     def __next__(self) -> AnyStr: ...
 
 class ContentFile(File[AnyStr]):
     file: IO[AnyStr]
     size: int
     def __init__(self, content: AnyStr, name: str | None = ...) -> None: ...
     def __bool__(self) -> bool: ...
-    def open(self: Self, mode: str | None = ...) -> Self: ...
+    def open(self, mode: str | None = ...) -> Self: ...
     def close(self) -> None: ...
     def write(self, data: AnyStr) -> int: ...
 
 def endswith_cr(line: bytes | str) -> bool: ...
 def endswith_lf(line: bytes | str) -> bool: ...
 def equals_lf(line: bytes | str) -> bool: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/core/files/storage/__init__.pyi` & `django-stubs-4.2.3/django-stubs/core/files/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/files/storage/base.pyi` & `django-stubs-4.2.3/django-stubs/core/files/storage/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/files/storage/filesystem.pyi` & `django-stubs-4.2.3/django-stubs/core/files/storage/filesystem.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/files/storage/memory.pyi` & `django-stubs-4.2.3/django-stubs/core/files/storage/memory.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/files/uploadedfile.pyi` & `django-stubs-4.2.3/django-stubs/core/files/uploadedfile.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import IO
 
-from _typeshed import Self
 from django.core.files.base import File
+from typing_extensions import Self
 
 class UploadedFile(File):
     content_type: str | None
     charset: str | None
     content_type_extra: dict[str, str] | None
     size: int | None  # type: ignore[assignment]
     name: str | None
@@ -42,8 +42,8 @@
         charset: str | None,
         content_type_extra: dict[str, str] = ...,
     ) -> None: ...
 
 class SimpleUploadedFile(InMemoryUploadedFile):
     def __init__(self, name: str, content: bytes | None, content_type: str = ...) -> None: ...
     @classmethod
-    def from_dict(cls: type[Self], file_dict: dict[str, str | bytes]) -> Self: ...
+    def from_dict(cls, file_dict: dict[str, str | bytes]) -> Self: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/core/files/uploadhandler.pyi` & `django-stubs-4.2.3/django-stubs/core/files/uploadhandler.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/files/utils.pyi` & `django-stubs-4.2.3/django-stubs/core/files/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/handlers/asgi.pyi` & `django-stubs-4.2.3/django-stubs/core/handlers/asgi.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/handlers/base.pyi` & `django-stubs-4.2.3/django-stubs/core/handlers/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/handlers/exception.pyi` & `django-stubs-4.2.3/django-stubs/core/handlers/exception.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/handlers/wsgi.pyi` & `django-stubs-4.2.3/django-stubs/core/handlers/wsgi.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/mail/__init__.pyi` & `django-stubs-4.2.3/django-stubs/core/mail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/mail/backends/base.pyi` & `django-stubs-4.2.3/django-stubs/core/mail/backends/base.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from collections.abc import Sequence
 from types import TracebackType
 from typing import Any
 
-from _typeshed import Self
 from django.core.mail.message import EmailMessage
+from typing_extensions import Self
 
 class BaseEmailBackend:
     fail_silently: bool
     def __init__(self, fail_silently: bool = ..., **kwargs: Any) -> None: ...
     def open(self) -> bool | None: ...
     def close(self) -> None: ...
-    def __enter__(self: Self) -> Self: ...
+    def __enter__(self) -> Self: ...
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None: ...
     def send_messages(self, email_messages: Sequence[EmailMessage]) -> int: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/core/mail/message.pyi` & `django-stubs-4.2.3/django-stubs/core/mail/message.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/management/__init__.pyi` & `django-stubs-4.2.3/django-stubs/core/management/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/management/base.pyi` & `django-stubs-4.2.3/django-stubs/core/management/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/management/color.pyi` & `django-stubs-4.2.3/django-stubs/core/management/color.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/management/commands/diffsettings.pyi` & `django-stubs-4.2.3/django-stubs/core/management/commands/diffsettings.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/management/commands/inspectdb.pyi` & `django-stubs-4.2.3/django-stubs/core/management/commands/inspectdb.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/management/commands/loaddata.pyi` & `django-stubs-4.2.3/django-stubs/core/management/commands/loaddata.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/management/commands/makemessages.pyi` & `django-stubs-4.2.3/django-stubs/core/management/commands/makemessages.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/management/commands/migrate.pyi` & `django-stubs-4.2.3/django-stubs/core/management/commands/migrate.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/management/commands/runserver.pyi` & `django-stubs-4.2.3/django-stubs/core/management/commands/runserver.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/management/templates.pyi` & `django-stubs-4.2.3/django-stubs/core/management/templates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/management/utils.pyi` & `django-stubs-4.2.3/django-stubs/core/management/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/paginator.pyi` & `django-stubs-4.2.3/django-stubs/core/paginator.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/serializers/__init__.pyi` & `django-stubs-4.2.3/django-stubs/core/serializers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/serializers/base.pyi` & `django-stubs-4.2.3/django-stubs/core/serializers/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/serializers/json.pyi` & `django-stubs-4.2.3/django-stubs/core/serializers/json.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/serializers/pyyaml.pyi` & `django-stubs-4.2.3/django-stubs/core/serializers/pyyaml.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/serializers/xml_serializer.pyi` & `django-stubs-4.2.3/django-stubs/core/serializers/xml_serializer.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/servers/basehttp.pyi` & `django-stubs-4.2.3/django-stubs/core/servers/basehttp.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/signing.pyi` & `django-stubs-4.2.3/django-stubs/core/signing.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/core/validators.pyi` & `django-stubs-4.2.3/django-stubs/core/validators.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/__init__.pyi` & `django-stubs-4.2.3/django-stubs/db/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/base/base.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/base/base.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from collections.abc import Callable, Generator, Iterator, MutableMapping
 from contextlib import contextmanager
 from datetime import tzinfo
 from typing import Any
 
-from _typeshed import Self
 from django.db.backends.base.client import BaseDatabaseClient
 from django.db.backends.base.creation import BaseDatabaseCreation
 from django.db.backends.base.features import BaseDatabaseFeatures
 from django.db.backends.base.introspection import BaseDatabaseIntrospection
 from django.db.backends.base.operations import BaseDatabaseOperations
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 from django.db.backends.base.validation import BaseDatabaseValidation
 from django.db.backends.utils import CursorDebugWrapper, CursorWrapper
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 NO_DB_ALIAS: str
 RAN_DB_VERSION_CHECK: set[str]
 
 _ExecuteWrapper: TypeAlias = Callable[
     [Callable[[str, Any, bool, dict[str, Any]], Any], str, Any, bool, dict[str, Any]], Any
 ]
@@ -115,8 +114,8 @@
     @contextmanager
     def _nodb_cursor(self) -> Generator[CursorWrapper, None, None]: ...
     def schema_editor(self, *args: Any, **kwargs: Any) -> BaseDatabaseSchemaEditor: ...
     def on_commit(self, func: Callable[[], object], robust: bool = ...) -> None: ...
     def run_and_clear_commit_hooks(self) -> None: ...
     @contextmanager
     def execute_wrapper(self, wrapper: _ExecuteWrapper) -> Generator[None, None, None]: ...
-    def copy(self: Self, alias: str | None = ...) -> Self: ...
+    def copy(self, alias: str | None = ...) -> Self: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/base/client.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/base/client.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/base/creation.pyi` & `django-stubs-4.2.3/django-stubs/utils/log.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,53 @@
+import logging.config
+from collections.abc import Callable
+from logging import Logger, LogRecord
 from typing import Any
 
-from django.db.backends.base.base import BaseDatabaseWrapper
+from django.core.management.color import Style
+from django.http import HttpRequest, HttpResponse
+from django.utils.functional import _StrOrPromise
 
-TEST_DATABASE_PREFIX: str
+request_logger: Logger
+DEFAULT_LOGGING: Any
 
-class BaseDatabaseCreation:
-    connection: BaseDatabaseWrapper
-    def __init__(self, connection: BaseDatabaseWrapper) -> None: ...
-    def create_test_db(
-        self, verbosity: int = ..., autoclobber: bool = ..., serialize: bool = ..., keepdb: bool = ...
-    ) -> str: ...
-    def set_as_test_mirror(self, primary_settings_dict: dict[str, dict[str, None] | int | str | None]) -> None: ...
-    def serialize_db_to_string(self) -> str: ...
-    def deserialize_db_from_string(self, data: str) -> None: ...
-    def clone_test_db(self, suffix: Any, verbosity: int = ..., autoclobber: bool = ..., keepdb: bool = ...) -> None: ...
-    def get_test_db_clone_settings(self, suffix: str) -> dict[str, Any]: ...
-    def destroy_test_db(
+def configure_logging(logging_config: str, logging_settings: dict[str, Any]) -> None: ...
+
+class AdminEmailHandler(logging.Handler):
+    include_html: bool
+    email_backend: str | None
+    def __init__(
         self,
-        old_database_name: str | None = ...,
-        verbosity: int = ...,
-        keepdb: bool = ...,
-        suffix: str | None = ...,
+        include_html: bool = ...,
+        email_backend: str | None = ...,
+        reporter_class: str | None = ...,
     ) -> None: ...
-    def sql_table_creation_suffix(self) -> str: ...
-    def test_db_signature(self) -> tuple[str, str, str, str]: ...
+    def send_mail(self, subject: _StrOrPromise, message: _StrOrPromise, *args: Any, **kwargs: Any) -> None: ...
+    def connection(self) -> Any: ...
+    def format_subject(self, subject: str) -> str: ...
+
+class CallbackFilter(logging.Filter):
+    callback: Callable
+    def __init__(self, callback: Callable) -> None: ...
+    def filter(self, record: str | LogRecord) -> bool: ...
+
+class RequireDebugFalse(logging.Filter):
+    def filter(self, record: str | LogRecord) -> bool: ...
+
+class RequireDebugTrue(logging.Filter):
+    def filter(self, record: str | LogRecord) -> bool: ...
+
+class ServerFormatter(logging.Formatter):
+    default_time_format: str
+    style: Style
+    def __init__(self, *args: Any, **kwargs: Any) -> None: ...
+    def uses_server_time(self) -> bool: ...
+
+def log_response(
+    message: str,
+    *args: Any,
+    response: HttpResponse | None = ...,
+    request: HttpRequest | None = ...,
+    logger: Logger = ...,
+    level: str | None = ...,
+    exception: BaseException | None = ...,
+) -> None: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/base/features.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/base/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/base/introspection.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/base/introspection.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/base/operations.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/base/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/base/schema.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/base/schema.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from collections.abc import Sequence
 from contextlib import AbstractContextManager
 from logging import Logger
 from types import TracebackType
 from typing import Any
 
-from _typeshed import Self
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.backends.ddl_references import Statement
 from django.db.models.base import Model
 from django.db.models.fields import Field
 from django.db.models.indexes import Index
+from typing_extensions import Self
 
 logger: Logger
 
 class BaseDatabaseSchemaEditor(AbstractContextManager[Any]):
     sql_create_table: str
     sql_rename_table: str
     sql_retablespace_table: str
@@ -46,15 +46,15 @@
     connection: BaseDatabaseWrapper
     collect_sql: bool
     collected_sql: Any
     atomic_migration: Any
     def __init__(self, connection: BaseDatabaseWrapper, collect_sql: bool = ..., atomic: bool = ...) -> None: ...
     deferred_sql: Any
     atomic: Any
-    def __enter__(self: Self) -> Self: ...
+    def __enter__(self) -> Self: ...
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None: ...
     def execute(self, sql: Statement | str, params: Sequence[Any] | None = ...) -> None: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/ddl_references.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/ddl_references.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/dummy/base.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/dummy/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/mysql/base.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/mysql/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/mysql/compiler.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/mysql/compiler.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/mysql/features.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/mysql/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/mysql/introspection.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/mysql/introspection.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/mysql/operations.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/mysql/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/mysql/schema.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/mysql/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/oracle/base.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/oracle/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/oracle/client.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/oracle/client.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/oracle/features.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/oracle/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/oracle/operations.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/oracle/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/oracle/schema.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/oracle/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/postgresql/base.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/postgresql/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/postgresql/client.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/postgresql/client.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/postgresql/features.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/postgresql/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/postgresql/operations.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/postgresql/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/postgresql/schema.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/postgresql/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/sqlite3/base.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/sqlite3/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/sqlite3/operations.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/sqlite3/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/backends/utils.pyi` & `django-stubs-4.2.3/django-stubs/db/backends/utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from contextlib import contextmanager
 from decimal import Decimal
 from logging import Logger
 from types import TracebackType
 from typing import Any, Literal, Protocol, overload
 from uuid import UUID
 
-from _typeshed import Self
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 logger: Logger
 
 # Protocol matching psycopg2.sql.Composable, to avoid depending psycopg2
 class _Composable(Protocol):
     def as_string(self, context: Any) -> str: ...
     def __add__(self, other: _Composable) -> _Composable: ...
@@ -40,15 +39,15 @@
 class CursorWrapper:
     cursor: Any
     db: Any
     def __init__(self, cursor: Any, db: Any) -> None: ...
     WRAP_ERROR_ATTRS: Any
     def __getattr__(self, attr: str) -> Any: ...
     def __iter__(self) -> Iterator[tuple[Any, ...]]: ...
-    def __enter__(self: Self) -> Self: ...
+    def __enter__(self) -> Self: ...
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None: ...
     def callproc(
```

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/autodetector.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/autodetector.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/exceptions.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/executor.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/executor.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/graph.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/graph.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/loader.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/loader.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/migration.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/migration.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from _typeshed import Self
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 from django.db.migrations.operations.base import Operation
 from django.db.migrations.state import ProjectState
+from typing_extensions import Self
 
 class Migration:
     operations: list[Operation]
     dependencies: list[tuple[str, str]]
     run_before: list[tuple[str, str]]
     replaces: list[tuple[str, str]]
     initial: bool | None
@@ -19,10 +19,10 @@
     ) -> ProjectState: ...
     def unapply(
         self, project_state: ProjectState, schema_editor: BaseDatabaseSchemaEditor, collect_sql: bool = ...
     ) -> ProjectState: ...
 
 class SwappableTuple(tuple[str, str]):
     setting: str
-    def __new__(cls: type[Self], value: tuple[str, str], setting: str) -> Self: ...
+    def __new__(cls, value: tuple[str, str], setting: str) -> Self: ...
 
 def swappable_dependency(value: str) -> SwappableTuple: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/operations/__init__.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/operations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/operations/base.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/operations/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/operations/fields.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/operations/fields.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/operations/models.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/operations/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/operations/special.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/operations/special.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/operations/utils.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/operations/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/questioner.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/questioner.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/recorder.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/recorder.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/serializer.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/serializer.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/state.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/state.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/migrations/writer.pyi` & `django-stubs-4.2.3/django-stubs/db/migrations/writer.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/__init__.pyi` & `django-stubs-4.2.3/django-stubs/db/models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/aggregates.pyi` & `django-stubs-4.2.3/django-stubs/db/models/aggregates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/base.pyi` & `django-stubs-4.2.3/django-stubs/db/models/base.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from collections.abc import Collection, Iterable, Sequence
 from typing import Any, Final, TypeVar
 
-from _typeshed import Self
 from django.core.checks.messages import CheckMessage
 from django.core.exceptions import MultipleObjectsReturned as BaseMultipleObjectsReturned
 from django.core.exceptions import ObjectDoesNotExist, ValidationError
 from django.db.models import BaseConstraint, Field
 from django.db.models.manager import BaseManager
 from django.db.models.options import Options
+from typing_extensions import Self
 
 _Self = TypeVar("_Self", bound=Model)
 
 class ModelStateFieldsCacheDescriptor: ...
 
 class ModelState:
     db: str | None
@@ -30,19 +30,19 @@
     DoesNotExist: Final[type[ObjectDoesNotExist]]
     MultipleObjectsReturned: Final[type[BaseMultipleObjectsReturned]]
 
     class Meta: ...
     _meta: Options[Any]
     pk: Any
     _state: ModelState
-    def __init__(self: Self, *args: Any, **kwargs: Any) -> None: ...
+    def __init__(self, *args: Any, **kwargs: Any) -> None: ...
     @classmethod
     def add_to_class(cls, name: str, value: Any) -> Any: ...
     @classmethod
-    def from_db(cls: type[Self], db: str | None, field_names: Collection[str], values: Collection[Any]) -> Self: ...
+    def from_db(cls, db: str | None, field_names: Collection[str], values: Collection[Any]) -> Self: ...
     def delete(self, using: Any = ..., keep_parents: bool = ...) -> tuple[int, dict[str, int]]: ...
     async def adelete(self, using: Any = ..., keep_parents: bool = ...) -> tuple[int, dict[str, int]]: ...
     def full_clean(
         self, exclude: Iterable[str] | None = ..., validate_unique: bool = ..., validate_constraints: bool = ...
     ) -> None: ...
     def clean(self) -> None: ...
     def clean_fields(self, exclude: Collection[str] | None = ...) -> None: ...
@@ -69,16 +69,16 @@
         self,
         raw: bool = ...,
         force_insert: bool = ...,
         force_update: bool = ...,
         using: str | None = ...,
         update_fields: Iterable[str] | None = ...,
     ) -> None: ...
-    def refresh_from_db(self: Self, using: str | None = ..., fields: Sequence[str] | None = ...) -> None: ...
-    async def arefresh_from_db(self: Self, using: str | None = ..., fields: Sequence[str] | None = ...) -> None: ...
+    def refresh_from_db(self, using: str | None = ..., fields: Sequence[str] | None = ...) -> None: ...
+    async def arefresh_from_db(self, using: str | None = ..., fields: Sequence[str] | None = ...) -> None: ...
     def serializable_value(self, field_name: str) -> Any: ...
     def prepare_database_save(self, field: Field) -> Any: ...
     def get_deferred_fields(self) -> set[str]: ...
     @classmethod
     def check(cls, **kwargs: Any) -> list[CheckMessage]: ...
     def __getstate__(self) -> dict: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/db/models/constraints.pyi` & `django-stubs-4.2.3/django-stubs/db/models/constraints.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from collections.abc import Sequence
 from enum import Enum
 from typing import Any, overload
 
-from _typeshed import Self
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 from django.db.models.base import Model
 from django.db.models.expressions import BaseExpression, Combinable
 from django.db.models.query_utils import Q
 from django.utils.functional import _StrOrPromise
+from typing_extensions import Self
 
 class Deferrable(Enum):
     DEFERRED: str
     IMMEDIATE: str
 
 class BaseConstraint:
     name: str
     violation_error_message: _StrOrPromise | None
     default_violation_error_message: _StrOrPromise
     def __init__(self, name: str, violation_error_message: _StrOrPromise | None = ...) -> None: ...
     def constraint_sql(self, model: type[Model] | None, schema_editor: BaseDatabaseSchemaEditor | None) -> str: ...
     def create_sql(self, model: type[Model] | None, schema_editor: BaseDatabaseSchemaEditor | None) -> str: ...
     def remove_sql(self, model: type[Model] | None, schema_editor: BaseDatabaseSchemaEditor | None) -> str: ...
     def deconstruct(self) -> Any: ...
-    def clone(self: Self) -> Self: ...
+    def clone(self) -> Self: ...
 
 class CheckConstraint(BaseConstraint):
     check: Q | BaseExpression
     def __init__(
         self, *, check: Q | BaseExpression, name: str, violation_error_message: _StrOrPromise | None = ...
     ) -> None: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/db/models/deletion.pyi` & `django-stubs-4.2.3/django-stubs/db/models/deletion.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/enums.pyi` & `django-stubs-4.2.3/django-stubs/db/models/enums.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/expressions.pyi` & `django-stubs-4.2.3/django-stubs/db/models/expressions.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import datetime
 from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
 from decimal import Decimal
 from typing import Any, Generic, Literal, TypeVar
 
-from _typeshed import Self
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import Q
 from django.db.models.fields import Field
 from django.db.models.lookups import Lookup, Transform
 from django.db.models.query import QuerySet
 from django.db.models.sql.compiler import SQLCompiler, _AsSqlType
 from django.db.models.sql.query import Query
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 class SQLiteNumericMixin:
     def as_sqlite(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 _Numeric: TypeAlias = float | Decimal
 
 class Combinable:
@@ -67,15 +66,15 @@
     @property
     def contains_aggregate(self) -> bool: ...
     @property
     def contains_over_clause(self) -> bool: ...
     @property
     def contains_column_references(self) -> bool: ...
     def resolve_expression(
-        self: Self,
+        self,
         query: Any = ...,
         allow_joins: bool = ...,
         reuse: set[str] | None = ...,
         summarize: bool = ...,
         for_save: bool = ...,
     ) -> Self: ...
     @property
@@ -84,17 +83,17 @@
     def field(self) -> Field: ...
     @property
     def output_field(self) -> Field: ...
     @property
     def convert_value(self) -> Callable: ...
     def get_lookup(self, lookup: str) -> type[Lookup] | None: ...
     def get_transform(self, name: str) -> type[Transform] | None: ...
-    def relabeled_clone(self: Self, change_map: dict[str | None, str]) -> Self: ...
-    def copy(self: Self) -> Self: ...
-    def get_group_by_cols(self: Self) -> list[Self]: ...
+    def relabeled_clone(self, change_map: dict[str | None, str]) -> Self: ...
+    def copy(self) -> Self: ...
+    def get_group_by_cols(self) -> list[Self]: ...
     def get_source_fields(self) -> list[Field | None]: ...
     def asc(
         self,
         *,
         descending: bool = ...,
         nulls_first: bool | None = ...,
         nulls_last: bool | None = ...,
@@ -152,15 +151,15 @@
     def copy(self) -> F: ...
 
 class ResolvedOuterRef(F): ...
 
 class OuterRef(F):
     def __init__(self, name: str | OuterRef) -> None: ...
     contains_aggregate: bool
-    def relabeled_clone(self: Self, relabels: Any) -> Self: ...
+    def relabeled_clone(self, relabels: Any) -> Self: ...
 
 class Func(SQLiteNumericMixin, Expression):
     function: str
     name: str
     template: str
     arg_joiner: str
     arity: int | None
```

### Comparing `django-stubs-4.2.2/django-stubs/db/models/fields/__init__.pyi` & `django-stubs-4.2.3/django-stubs/db/models/fields/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import decimal
 import uuid
 from collections.abc import Callable, Iterable, Sequence
 from datetime import date, time, timedelta
 from datetime import datetime as real_datetime
-from typing import Any, Generic, Protocol, TypeVar, overload
+from typing import Any, ClassVar, Generic, Protocol, TypeVar, overload
 
 from django.core import validators  # due to weird mypy.stubtest error
 from django.core.checks import CheckMessage
 from django.core.exceptions import FieldDoesNotExist as FieldDoesNotExist
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import Model
 from django.db.models.expressions import Col, Combinable
@@ -178,21 +178,21 @@
         auto_created: bool = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
     ) -> None: ...
     def __set__(self, instance: Any, value: _ST) -> None: ...
     # class access
     @overload
-    def __get__(self: Self, instance: None, owner: Any) -> _FieldDescriptor[Self]: ...
+    def __get__(self, instance: None, owner: Any) -> _FieldDescriptor[Self]: ...
     # Model instance access
     @overload
     def __get__(self, instance: Model, owner: Any) -> _GT: ...
     # non-Model instances
     @overload
-    def __get__(self: Self, instance: Any, owner: Any) -> Self: ...
+    def __get__(self, instance: Any, owner: Any) -> Self: ...
     def deconstruct(self) -> Any: ...
     def set_attributes_from_name(self, name: str) -> None: ...
     def db_type_parameters(self, connection: BaseDatabaseWrapper) -> DictWrapper: ...
     def db_check(self, connection: BaseDatabaseWrapper) -> str | None: ...
     def db_type(self, connection: BaseDatabaseWrapper) -> str | None: ...
     def db_parameters(self, connection: BaseDatabaseWrapper) -> dict[str, str | None]: ...
     def pre_save(self, model_instance: Model, add: bool) -> Any: ...
@@ -235,15 +235,18 @@
     _pyi_private_get_type: int
     _pyi_lookup_exact_type: str | int
 
 class PositiveIntegerRelDbTypeMixin:
     def rel_db_type(self, connection: BaseDatabaseWrapper) -> str: ...
 
 class SmallIntegerField(IntegerField[_ST, _GT]): ...
-class BigIntegerField(IntegerField[_ST, _GT]): ...
+
+class BigIntegerField(IntegerField[_ST, _GT]):
+    MAX_BIGINT: ClassVar[int]
+
 class PositiveIntegerField(PositiveIntegerRelDbTypeMixin, IntegerField[_ST, _GT]): ...
 class PositiveSmallIntegerField(PositiveIntegerRelDbTypeMixin, SmallIntegerField[_ST, _GT]): ...
 class PositiveBigIntegerField(PositiveIntegerRelDbTypeMixin, BigIntegerField[_ST, _GT]): ...
 
 class FloatField(Field[_ST, _GT]):
     _pyi_private_set_type: float | int | str | Combinable
     _pyi_private_get_type: float
```

### Comparing `django-stubs-4.2.2/django-stubs/db/models/fields/files.pyi` & `django-stubs-4.2.3/django-stubs/db/models/fields/files.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from collections.abc import Callable, Iterable
 from typing import Any, Protocol, TypeVar, overload
 
-from _typeshed import Self
 from django.core import validators  # due to weird mypy.stubtest error
 from django.core.files.base import File
 from django.core.files.images import ImageFile
 from django.core.files.storage import Storage
 from django.db.models.base import Model
 from django.db.models.fields import Field, _ErrorMessagesT, _FieldChoices
 from django.db.models.query_utils import DeferredAttribute
 from django.utils._os import _PathCompatible
 from django.utils.functional import _StrOrPromise
+from typing_extensions import Self
 
 class FieldFile(File):
     instance: Model
     field: FileField
     storage: Storage
     name: str | None
     def __init__(self, instance: Model, field: FileField, name: str | None) -> None: ...
@@ -74,15 +74,15 @@
     @overload
     def __get__(self, instance: None, owner: Any) -> FileDescriptor: ...
     # Model instance access
     @overload
     def __get__(self, instance: Model, owner: Any) -> Any: ...
     # non-Model instances
     @overload
-    def __get__(self: Self, instance: Any, owner: Any) -> Self: ...
+    def __get__(self, instance: Any, owner: Any) -> Self: ...
     def generate_filename(self, instance: Model | None, filename: _PathCompatible) -> str: ...
 
 class ImageFileDescriptor(FileDescriptor):
     field: ImageField
     def __set__(self, instance: Model, value: str | None) -> None: ...
 
 class ImageFieldFile(ImageFile, FieldFile):
@@ -102,9 +102,9 @@
     @overload
     def __get__(self, instance: None, owner: Any) -> ImageFileDescriptor: ...
     # Model instance access
     @overload
     def __get__(self, instance: Model, owner: Any) -> Any: ...
     # non-Model instances
     @overload
-    def __get__(self: Self, instance: Any, owner: Any) -> Self: ...
+    def __get__(self, instance: Any, owner: Any) -> Self: ...
     def update_dimension_fields(self, instance: Model, force: bool = ..., *args: Any, **kwargs: Any) -> None: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/db/models/fields/json.pyi` & `django-stubs-4.2.3/django-stubs/db/models/fields/json.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 from collections.abc import Callable
 from typing import Any
 
-from _typeshed import Self
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import lookups
 from django.db.models.lookups import PostgresOperatorLookup, Transform
 from django.db.models.sql.compiler import SQLCompiler
 from django.utils.functional import _StrOrPromise
+from typing_extensions import Self
 
 from . import Field
 from .mixins import CheckFieldDefaultMixin
 
 class JSONField(CheckFieldDefaultMixin, Field):
     encoder: type[json.JSONEncoder] | None
     decoder: type[json.JSONDecoder] | None
@@ -54,15 +54,15 @@
     def __init__(self, key_name: Any, *args: Any, **kwargs: Any) -> None: ...
     def preprocess_lhs(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> Any: ...
 
 class KeyTextTransform(KeyTransform):
     postgres_operator: str
     postgres_nested_operator: str
     @classmethod
-    def from_lookup(cls: type[Self], lookup: str) -> Self: ...
+    def from_lookup(cls, lookup: str) -> Self: ...
 
 KT: Callable[[str], KeyTextTransform]
 
 class KeyTransformTextLookupMixin:
     def __init__(self, key_transform: Any, *args: Any, **kwargs: Any) -> None: ...
 
 class KeyTransformIsNull(lookups.IsNull): ...
```

### Comparing `django-stubs-4.2.2/django-stubs/db/models/fields/mixins.pyi` & `django-stubs-4.2.3/django-stubs/db/models/fields/mixins.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/fields/related.pyi` & `django-stubs-4.2.3/django-stubs/db/models/fields/related.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     @overload
     def __get__(self, instance: None, owner: Any) -> ForwardManyToOneDescriptor[Self]: ...
     # Model instance access
     @overload
     def __get__(self, instance: Model, owner: Any) -> _GT: ...
     # non-Model instances
     @overload
-    def __get__(self: Self, instance: Any, owner: Any) -> Self: ...
+    def __get__(self, instance: Any, owner: Any) -> Self: ...
     def resolve_related_fields(self) -> list[tuple[Field, Field]]: ...
     @property
     def related_fields(self) -> list[tuple[Field, Field]]: ...
     @property
     def reverse_related_fields(self) -> list[tuple[Field, Field]]: ...
     @property
     def local_related_fields(self) -> tuple[Field, ...]: ...
@@ -198,15 +198,15 @@
     @overload
     def __get__(self, instance: None, owner: Any) -> ForwardOneToOneDescriptor[Self]: ...
     # Model instance access
     @overload
     def __get__(self, instance: Model, owner: Any) -> _GT: ...
     # non-Model instances
     @overload
-    def __get__(self: Self, instance: Any, owner: Any) -> Self: ...
+    def __get__(self, instance: Any, owner: Any) -> Self: ...
 
 class ManyToManyField(RelatedField[_ST, _GT]):
     _pyi_private_set_type: Sequence[Any]
     _pyi_private_get_type: RelatedManager[Any]
 
     description: str
     has_null_arg: bool
@@ -259,15 +259,15 @@
     @overload
     def __get__(self, instance: None, owner: Any) -> ManyToManyDescriptor[Self]: ...
     # Model instance access
     @overload
     def __get__(self, instance: Model, owner: Any) -> _GT: ...
     # non-Model instances
     @overload
-    def __get__(self: Self, instance: Any, owner: Any) -> Self: ...
+    def __get__(self, instance: Any, owner: Any) -> Self: ...
     def get_path_info(self, filtered_relation: FilteredRelation | None = ...) -> list[PathInfo]: ...
     def get_reverse_path_info(self, filtered_relation: FilteredRelation | None = ...) -> list[PathInfo]: ...
     def contribute_to_related_class(self, cls: type[Model], related: RelatedField) -> None: ...
     def m2m_db_table(self) -> str: ...
     def m2m_column_name(self) -> str: ...
     def m2m_reverse_name(self) -> str: ...
     def m2m_reverse_field_name(self) -> str: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/db/models/fields/related_descriptors.pyi` & `django-stubs-4.2.3/django-stubs/db/models/fields/related_descriptors.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/fields/related_lookups.pyi` & `django-stubs-4.2.3/django-stubs/db/models/fields/related_lookups.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/fields/reverse_related.pyi` & `django-stubs-4.2.3/django-stubs/db/models/fields/reverse_related.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/functions/__init__.pyi` & `django-stubs-4.2.3/django-stubs/db/models/functions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/functions/comparison.pyi` & `django-stubs-4.2.3/django-stubs/db/models/functions/comparison.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/functions/datetime.pyi` & `django-stubs-4.2.3/django-stubs/db/models/functions/datetime.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/functions/math.pyi` & `django-stubs-4.2.3/django-stubs/db/models/functions/math.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/functions/text.pyi` & `django-stubs-4.2.3/django-stubs/db/models/functions/text.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/functions/window.pyi` & `django-stubs-4.2.3/django-stubs/db/models/functions/window.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/indexes.pyi` & `django-stubs-4.2.3/django-stubs/db/models/indexes.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/lookups.pyi` & `django-stubs-4.2.3/django-stubs/db/models/lookups.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections.abc import Iterable, Mapping
 from typing import Any, Generic, Literal, TypeVar
 
-from _typeshed import Self
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.expressions import Expression, Func
 from django.db.models.query_utils import RegisterLookupMixin
 from django.db.models.sql.compiler import SQLCompiler, _AsSqlType, _ParamT
 from django.utils.datastructures import OrderedSet
+from typing_extensions import Self
 
 _T = TypeVar("_T")
 
 class Lookup(Generic[_T]):
     lookup_name: str
     prepare_rhs: bool
     can_use_none_as_rhs: bool
@@ -27,15 +27,15 @@
     def get_prep_lookup(self) -> Any: ...
     def get_db_prep_lookup(self, value: _ParamT, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
     def process_lhs(
         self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, lhs: Expression | None = ...
     ) -> _AsSqlType: ...
     def process_rhs(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
     def rhs_is_direct_value(self) -> bool: ...
-    def relabeled_clone(self: Self, relabels: Mapping[str, str]) -> Self: ...
+    def relabeled_clone(self, relabels: Mapping[str, str]) -> Self: ...
     def get_group_by_cols(self) -> list[Expression]: ...
     def as_sql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
     @property
     def contains_aggregate(self) -> bool: ...
     @property
     def contains_over_clause(self) -> bool: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/db/models/manager.pyi` & `django-stubs-4.2.3/django-stubs/db/models/manager.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 from collections.abc import AsyncIterator, Collection, Iterable, Iterator, MutableMapping, Sequence
 from typing import Any, Generic, NoReturn, TypeVar, overload
 
-from _typeshed import Self
 from django.db.models import Combinable
 from django.db.models.base import Model
 from django.db.models.query import QuerySet, RawQuerySet
+from typing_extensions import Self
 
 from django_stubs_ext import ValuesQuerySet
 
 _T = TypeVar("_T", bound=Model, covariant=True)
 
 class BaseManager(Generic[_T]):
     creation_counter: int
@@ -20,21 +20,19 @@
     _db: str | None
     def __init__(self) -> None: ...
     def deconstruct(
         self,
     ) -> tuple[bool, str | None, str | None, tuple[Any, ...] | None, dict[str, Any] | None]: ...
     def check(self, **kwargs: Any) -> list[Any]: ...
     @classmethod
-    def from_queryset(
-        cls: type[Self], queryset_class: type[QuerySet[_T]], class_name: str | None = ...
-    ) -> type[Self]: ...
+    def from_queryset(cls, queryset_class: type[QuerySet[_T]], class_name: str | None = ...) -> type[Self]: ...
     @classmethod
     def _get_queryset_methods(cls, queryset_class: type) -> dict[str, Any]: ...
     def contribute_to_class(self, cls: type[Model], name: str) -> None: ...
-    def db_manager(self: Self, using: str | None = ..., hints: dict[str, Model] | None = ...) -> Self: ...
+    def db_manager(self, using: str | None = ..., hints: dict[str, Model] | None = ...) -> Self: ...
     @property
     def db(self) -> str: ...
     def get_queryset(self) -> QuerySet[_T]: ...
     # NOTE: The following methods are in common with QuerySet, but note that the use of QuerySet as a return type
     # rather than a self-type (_QS), since Manager's QuerySet-like methods return QuerySets and not Managers.
     def iterator(self, chunk_size: int = ...) -> Iterator[_T]: ...
     def aiterator(self, chunk_size: int = ...) -> AsyncIterator[_T]: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/db/models/options.pyi` & `django-stubs-4.2.3/django-stubs/db/models/options.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/query.pyi` & `django-stubs-4.2.3/django-stubs/db/models/query.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import datetime
 from collections.abc import AsyncIterator, Collection, Iterable, Iterator, MutableMapping, Reversible, Sequence, Sized
 from typing import Any, Generic, NamedTuple, TypeVar, overload
 
-from _typeshed import Self
 from django.db.models import Manager
 from django.db.models.base import Model
 from django.db.models.expressions import Combinable
 from django.db.models.sql.query import Query, RawQuery
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 _T = TypeVar("_T", bound=Model, covariant=True)
 _Row = TypeVar("_Row", covariant=True)
 _QS = TypeVar("_QS", bound=_QuerySet)
 _TupleT = TypeVar("_TupleT", bound=tuple[Any, ...], covariant=True)
 
 MAX_GET_RESULTS: int
@@ -56,16 +55,16 @@
     @classmethod
     def as_manager(cls) -> Manager[_T]: ...
     def __len__(self) -> int: ...
     def __bool__(self) -> bool: ...
     def __class_getitem__(cls: type[_QS], item: type[_T]) -> type[_QS]: ...
     def __getstate__(self) -> dict[str, Any]: ...
     # Technically, the other QuerySet must be of the same type _T, but _T is covariant
-    def __and__(self: Self, other: _QuerySet[_T, _Row]) -> Self: ...
-    def __or__(self: Self, other: _QuerySet[_T, _Row]) -> Self: ...
+    def __and__(self, other: _QuerySet[_T, _Row]) -> Self: ...
+    def __or__(self, other: _QuerySet[_T, _Row]) -> Self: ...
     # IMPORTANT: When updating any of the following methods' signatures, please ALSO modify
     # the corresponding method in BaseManager.
     def iterator(self, chunk_size: int = ...) -> Iterator[_Row]: ...
     def aiterator(self, chunk_size: int = ...) -> AsyncIterator[_Row]: ...
     def aggregate(self, *args: Any, **kwargs: Any) -> dict[str, Any]: ...
     async def aaggregate(self, *args: Any, **kwargs: Any) -> dict[str, Any]: ...
     def get(self, *args: Any, **kwargs: Any) -> _Row: ...
@@ -131,60 +130,60 @@
     def values(self, *fields: str | Combinable, **expressions: Any) -> _QuerySet[_T, dict[str, Any]]: ...
     # The type of values_list may be overridden to be more specific in the mypy plugin, depending on the fields param
     def values_list(self, *fields: str | Combinable, flat: bool = ..., named: bool = ...) -> _QuerySet[_T, Any]: ...
     def dates(self, field_name: str, kind: str, order: str = ...) -> _QuerySet[_T, datetime.date]: ...
     def datetimes(
         self, field_name: str, kind: str, order: str = ..., tzinfo: datetime.tzinfo | None = ...
     ) -> _QuerySet[_T, datetime.datetime]: ...
-    def none(self: Self) -> Self: ...
-    def all(self: Self) -> Self: ...
-    def filter(self: Self, *args: Any, **kwargs: Any) -> Self: ...
-    def exclude(self: Self, *args: Any, **kwargs: Any) -> Self: ...
-    def complex_filter(self: Self, filter_obj: Any) -> Self: ...
+    def none(self) -> Self: ...
+    def all(self) -> Self: ...
+    def filter(self, *args: Any, **kwargs: Any) -> Self: ...
+    def exclude(self, *args: Any, **kwargs: Any) -> Self: ...
+    def complex_filter(self, filter_obj: Any) -> Self: ...
     def count(self) -> int: ...
     async def acount(self) -> int: ...
-    def union(self: Self, *other_qs: Any, all: bool = ...) -> Self: ...
-    def intersection(self: Self, *other_qs: Any) -> Self: ...
-    def difference(self: Self, *other_qs: Any) -> Self: ...
+    def union(self, *other_qs: Any, all: bool = ...) -> Self: ...
+    def intersection(self, *other_qs: Any) -> Self: ...
+    def difference(self, *other_qs: Any) -> Self: ...
     def select_for_update(
-        self: Self, nowait: bool = ..., skip_locked: bool = ..., of: Sequence[str] = ..., no_key: bool = ...
+        self, nowait: bool = ..., skip_locked: bool = ..., of: Sequence[str] = ..., no_key: bool = ...
     ) -> Self: ...
-    def select_related(self: Self, *fields: Any) -> Self: ...
-    def prefetch_related(self: Self, *lookups: Any) -> Self: ...
-    def annotate(self: Self, *args: Any, **kwargs: Any) -> Self: ...
-    def alias(self: Self, *args: Any, **kwargs: Any) -> Self: ...
-    def order_by(self: Self, *field_names: Any) -> Self: ...
-    def distinct(self: Self, *field_names: Any) -> Self: ...
+    def select_related(self, *fields: Any) -> Self: ...
+    def prefetch_related(self, *lookups: Any) -> Self: ...
+    def annotate(self, *args: Any, **kwargs: Any) -> Self: ...
+    def alias(self, *args: Any, **kwargs: Any) -> Self: ...
+    def order_by(self, *field_names: Any) -> Self: ...
+    def distinct(self, *field_names: Any) -> Self: ...
     # extra() return type won't be supported any time soon
     def extra(
         self,
         select: dict[str, Any] | None = ...,
         where: Sequence[str] | None = ...,
         params: Sequence[Any] | None = ...,
         tables: Sequence[str] | None = ...,
         order_by: Sequence[str] | None = ...,
         select_params: Sequence[Any] | None = ...,
     ) -> _QuerySet[Any, Any]: ...
-    def reverse(self: Self) -> Self: ...
-    def defer(self: Self, *fields: Any) -> Self: ...
-    def only(self: Self, *fields: Any) -> Self: ...
-    def using(self: Self, alias: str | None) -> Self: ...
+    def reverse(self) -> Self: ...
+    def defer(self, *fields: Any) -> Self: ...
+    def only(self, *fields: Any) -> Self: ...
+    def using(self, alias: str | None) -> Self: ...
     @property
     def ordered(self) -> bool: ...
     @property
     def db(self) -> str: ...
     def _fetch_all(self) -> None: ...
     def resolve_expression(self, *args: Any, **kwargs: Any) -> Any: ...
     def __iter__(self) -> Iterator[_Row]: ...
     def __aiter__(self) -> AsyncIterator[_Row]: ...
     def __contains__(self, x: object) -> bool: ...
     @overload
     def __getitem__(self, i: int) -> _Row: ...
     @overload
-    def __getitem__(self: Self, s: slice) -> Self: ...
+    def __getitem__(self, s: slice) -> Self: ...
     def __reversed__(self) -> Iterator[_Row]: ...
 
 class RawQuerySet(Iterable[_T], Sized):
     query: RawQuery
     def __init__(
         self,
         raw_query: RawQuery | str,
```

### Comparing `django-stubs-4.2.2/django-stubs/db/models/query_utils.pyi` & `django-stubs-4.2.3/django-stubs/db/models/query_utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/signals.pyi` & `django-stubs-4.2.3/django-stubs/db/models/signals.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/sql/compiler.pyi` & `django-stubs-4.2.3/django-stubs/db/models/sql/compiler.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/sql/datastructures.pyi` & `django-stubs-4.2.3/django-stubs/db/models/sql/datastructures.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/sql/query.pyi` & `django-stubs-4.2.3/django-stubs/db/models/sql/query.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/sql/subqueries.pyi` & `django-stubs-4.2.3/django-stubs/db/models/sql/subqueries.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/models/sql/where.pyi` & `django-stubs-4.2.3/django-stubs/db/models/sql/where.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/transaction.pyi` & `django-stubs-4.2.3/django-stubs/db/transaction.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/db/utils.pyi` & `django-stubs-4.2.3/django-stubs/db/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/dispatch/dispatcher.pyi` & `django-stubs-4.2.3/django-stubs/dispatch/dispatcher.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/forms/__init__.pyi` & `django-stubs-4.2.3/django-stubs/forms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/forms/boundfield.pyi` & `django-stubs-4.2.3/django-stubs/forms/boundfield.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/forms/fields.pyi` & `django-stubs-4.2.3/django-stubs/forms/fields.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/forms/forms.pyi` & `django-stubs-4.2.3/django-stubs/forms/forms.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/forms/formsets.pyi` & `django-stubs-4.2.3/django-stubs/forms/formsets.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/forms/models.pyi` & `django-stubs-4.2.3/django-stubs/forms/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/forms/renderers.pyi` & `django-stubs-4.2.3/django-stubs/forms/renderers.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/forms/utils.pyi` & `django-stubs-4.2.3/django-stubs/forms/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/forms/widgets.pyi` & `django-stubs-4.2.3/django-stubs/forms/widgets.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/http/__init__.pyi` & `django-stubs-4.2.3/django-stubs/http/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/http/multipartparser.pyi` & `django-stubs-4.2.3/django-stubs/http/multipartparser.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/http/request.pyi` & `django-stubs-4.2.3/django-stubs/http/request.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from collections.abc import Iterable, Mapping
 from io import BytesIO
 from re import Pattern
 from typing import Any, BinaryIO, Literal, NoReturn, TypeVar, overload
 
-from _typeshed import Self
 from django.contrib.auth.base_user import AbstractBaseUser
 from django.contrib.auth.models import AnonymousUser
 from django.contrib.sessions.backends.base import SessionBase
 from django.contrib.sites.models import Site
 from django.core.files import uploadedfile, uploadhandler
 from django.urls import ResolverMatch
 from django.utils.datastructures import CaseInsensitiveMapping, ImmutableList, MultiValueDict
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 RAISE_ERROR: object
 host_validation_re: Pattern[str]
 
 class UnreadablePostError(OSError): ...
 class RawPostDataException(Exception): ...
 
@@ -128,15 +127,15 @@
         self: _ImmutableQueryDict,
         query_string: str | bytes | None = ...,
         mutable: bool = ...,
         encoding: str | None = ...,
     ) -> None: ...
     @classmethod
     def fromkeys(  # type: ignore
-        cls: type[Self],
+        cls,
         iterable: Iterable[bytes | str],
         value: str | bytes = ...,
         mutable: bool = ...,
         encoding: str | None = ...,
     ) -> Self: ...
     @property
     def encoding(self) -> str: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/http/response.pyi` & `django-stubs-4.2.3/django-stubs/http/response.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/middleware/cache.pyi` & `django-stubs-4.2.3/django-stubs/middleware/cache.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/middleware/common.pyi` & `django-stubs-4.2.3/django-stubs/middleware/common.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/middleware/csrf.pyi` & `django-stubs-4.2.3/django-stubs/middleware/csrf.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/middleware/security.pyi` & `django-stubs-4.2.3/django-stubs/middleware/security.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/shortcuts.pyi` & `django-stubs-4.2.3/django-stubs/shortcuts.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/template/__init__.pyi` & `django-stubs-4.2.3/django-stubs/template/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/template/backends/base.pyi` & `django-stubs-4.2.3/django-stubs/template/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/template/backends/django.pyi` & `django-stubs-4.2.3/django-stubs/template/backends/django.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/template/backends/jinja2.pyi` & `django-stubs-4.2.3/django-stubs/template/utils.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-from collections.abc import Callable
+from collections.abc import Iterator
 from typing import Any
 
-from django.template.exceptions import TemplateSyntaxError
+from django.core.exceptions import ImproperlyConfigured
+from django.template.backends.base import BaseEngine
 
-from .base import BaseEngine
+class InvalidTemplateEngineError(ImproperlyConfigured): ...
 
-class Jinja2(BaseEngine):
-    env: Any
-    context_processors: list[str]
-    def __init__(self, params: dict[str, Any]) -> None: ...
+class EngineHandler:
+    def __init__(self, templates: list[dict[str, Any]] = ...) -> None: ...
     @property
-    def template_context_processors(self) -> list[Callable]: ...
+    def templates(self) -> dict[str, Any]: ...
+    def __getitem__(self, alias: str) -> BaseEngine: ...
+    def __iter__(self) -> Iterator[Any]: ...
+    def all(self) -> list[BaseEngine]: ...
 
-class Origin:
-    name: str
-    template_name: str | None
-    def __init__(self, name: str, template_name: str | None) -> None: ...
-
-def get_exception_info(exception: TemplateSyntaxError) -> dict[str, Any]: ...
+def get_app_template_dirs(dirname: str) -> tuple: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/template/base.pyi` & `django-stubs-4.2.3/django-stubs/template/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/template/context.pyi` & `django-stubs-4.2.3/django-stubs/template/context.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 from collections.abc import Callable, Iterable, Iterator
 from contextlib import contextmanager
 from types import TracebackType
 from typing import Any
 
-from _typeshed import Self
 from django.http.request import HttpRequest
 from django.template.base import Node, Origin, Template
 from django.template.loader_tags import IncludeNode
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 _ContextKeys: TypeAlias = int | str | Node
 
 _ContextValues: TypeAlias = dict[str, Any] | Context
 
 class ContextPopException(Exception): ...
 
 class ContextDict(dict):
     context: BaseContext
     def __init__(self, context: BaseContext, *args: Any, **kwargs: Any) -> None: ...
-    def __enter__(self: Self) -> Self: ...
+    def __enter__(self) -> Self: ...
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None: ...
 
 class BaseContext(Iterable[Any]):
     def __init__(self, dict_: Any = ...) -> None: ...
-    def __copy__(self: Self) -> Self: ...
+    def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[Any]: ...
     def push(self, *args: Any, **kwargs: Any) -> ContextDict: ...
     def pop(self) -> ContextDict: ...
     def __setitem__(self, key: _ContextKeys, value: Any) -> None: ...
     def set_upward(self, key: _ContextKeys, value: int | str) -> None: ...
     def __getitem__(self, key: _ContextKeys) -> Any: ...
     def __delitem__(self, key: _ContextKeys) -> None: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/template/context_processors.pyi` & `django-stubs-4.2.3/django-stubs/template/context_processors.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/template/defaultfilters.pyi` & `django-stubs-4.2.3/django-stubs/template/defaultfilters.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/template/defaulttags.pyi` & `django-stubs-4.2.3/django-stubs/template/defaulttags.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/template/engine.pyi` & `django-stubs-4.2.3/django-stubs/template/engine.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/template/library.pyi` & `django-stubs-4.2.3/django-stubs/template/library.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/template/loader.pyi` & `django-stubs-4.2.3/django-stubs/template/loader.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/template/loader_tags.pyi` & `django-stubs-4.2.3/django-stubs/template/loader_tags.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/template/loaders/cached.pyi` & `django-stubs-4.2.3/django-stubs/template/loaders/cached.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/template/loaders/filesystem.pyi` & `django-stubs-4.2.3/django-stubs/template/loaders/filesystem.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/template/response.pyi` & `django-stubs-4.2.3/django-stubs/template/response.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/template/smartif.pyi` & `django-stubs-4.2.3/django-stubs/template/smartif.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/templatetags/cache.pyi` & `django-stubs-4.2.3/django-stubs/templatetags/cache.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/templatetags/i18n.pyi` & `django-stubs-4.2.3/django-stubs/templatetags/i18n.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/templatetags/static.pyi` & `django-stubs-4.2.3/django-stubs/templatetags/static.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/templatetags/tz.pyi` & `django-stubs-4.2.3/django-stubs/templatetags/tz.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/test/__init__.pyi` & `django-stubs-4.2.3/django-stubs/test/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/test/client.pyi` & `django-stubs-4.2.3/django-stubs/test/client.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/test/html.pyi` & `django-stubs-4.2.3/django-stubs/test/html.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/test/runner.pyi` & `django-stubs-4.2.3/django-stubs/test/runner.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/test/selenium.pyi` & `django-stubs-4.2.3/django-stubs/test/selenium.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/test/signals.pyi` & `django-stubs-4.2.3/django-stubs/test/signals.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/test/testcases.pyi` & `django-stubs-4.2.3/django-stubs/test/testcases.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import threading
 import unittest
 from collections.abc import Callable, Collection, Generator, Iterable, Iterator, Mapping, Sequence
 from contextlib import contextmanager
 from types import TracebackType
 from typing import Any, overload
 
-from _typeshed import Self
 from django.core.exceptions import ImproperlyConfigured
 from django.core.handlers.wsgi import WSGIHandler
 from django.core.servers.basehttp import ThreadedWSGIServer, WSGIRequestHandler
 from django.db import connections  # noqa: F401
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.base import Model
 from django.db.models.query import QuerySet, RawQuerySet
@@ -18,14 +17,15 @@
 from django.http import HttpRequest
 from django.http.response import FileResponse, HttpResponseBase
 from django.template.base import Template
 from django.test.client import AsyncClient, Client
 from django.test.html import Element
 from django.test.utils import CaptureQueriesContext, ContextList
 from django.utils.functional import classproperty
+from typing_extensions import Self
 
 def to_list(value: Any) -> list[Any]: ...
 def assert_and_parse_html(self: Any, html: str, user_msg: str, msg: str) -> Element: ...
 
 class _AssertNumQueriesContext(CaptureQueriesContext):
     test_case: SimpleTestCase
     num: int
@@ -37,15 +37,15 @@
     rendered_templates: list[Template]
     rendered_template_names: list[str]
     context: ContextList
     def __init__(self, test_case: Any, template_name: Any) -> None: ...
     def on_template_render(self, sender: Any, signal: Any, template: Any, context: Any, **kwargs: Any) -> None: ...
     def test(self) -> None: ...
     def message(self) -> str: ...
-    def __enter__(self: Self) -> Self: ...
+    def __enter__(self) -> Self: ...
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None: ...
 
@@ -292,12 +292,12 @@
     def live_server_url(cls: Any) -> str: ...
     @classproperty
     def allowed_host(cls: Any) -> str: ...
 
 class SerializeMixin:
     lockfile: Any
     @classmethod
-    def setUpClass(cls: type[Self]) -> None: ...
+    def setUpClass(cls) -> None: ...
     @classmethod
-    def tearDownClass(cls: type[Self]) -> None: ...
+    def tearDownClass(cls) -> None: ...
 
 def connections_support_transactions(aliases: Iterable[str] | None = ...) -> bool: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/test/utils.pyi` & `django-stubs-4.2.3/django-stubs/test/utils.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 from contextlib import AbstractContextManager, contextmanager
 from decimal import Decimal
 from io import StringIO
 from logging import Logger
 from types import TracebackType
 from typing import Any, Protocol, SupportsIndex, TypeVar
 
-from _typeshed import Self
 from django.apps.registry import Apps
 from django.conf import LazySettings, Settings
 from django.core.checks.registry import CheckRegistry
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.lookups import Lookup, Transform
 from django.db.models.query_utils import RegisterLookupMixin
 from django.test.runner import DiscoverRunner
 from django.test.testcases import SimpleTestCase
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 _TestClass: TypeAlias = type[SimpleTestCase]
 
 _DecoratedTest: TypeAlias = Callable | _TestClass
 _DT = TypeVar("_DT", bound=_DecoratedTest)
 _C = TypeVar("_C", bound=Callable)  # Any callable
 
@@ -89,15 +88,15 @@
     final_queries: int | None
     def __init__(self, connection: BaseDatabaseWrapper) -> None: ...
     def __iter__(self) -> Iterator[dict[str, str]]: ...
     def __getitem__(self, index: int) -> dict[str, str]: ...
     def __len__(self) -> int: ...
     @property
     def captured_queries(self) -> list[dict[str, str]]: ...
-    def __enter__(self: Self) -> Self: ...
+    def __enter__(self) -> Self: ...
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/urls/__init__.pyi` & `django-stubs-4.2.3/django-stubs/urls/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/urls/base.pyi` & `django-stubs-4.2.3/django-stubs/urls/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/urls/conf.pyi` & `django-stubs-4.2.3/django-stubs/urls/conf.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/urls/converters.pyi` & `django-stubs-4.2.3/django-stubs/urls/converters.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/urls/resolvers.pyi` & `django-stubs-4.2.3/django-stubs/urls/resolvers.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/archive.pyi` & `django-stubs-4.2.3/django-stubs/utils/archive.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from collections.abc import Iterable, Sequence
 from types import TracebackType
 from typing import Any
 
-from _typeshed import Self
+from typing_extensions import Self
 
 class ArchiveException(Exception): ...
 class UnrecognizedArchiveFormat(ArchiveException): ...
 
 def extract(path: str, to_path: str) -> None: ...
 
 class Archive:
     def __init__(self, file: str) -> None: ...
-    def __enter__(self: Self) -> Self: ...
+    def __enter__(self) -> Self: ...
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
         traceback: TracebackType | None,
     ) -> None: ...
     def extract(self, to_path: str) -> None: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/utils/autoreload.pyi` & `django-stubs-4.2.3/django-stubs/utils/autoreload.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/baseconv.pyi` & `django-stubs-4.2.3/django-stubs/utils/baseconv.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/cache.pyi` & `django-stubs-4.2.3/django-stubs/utils/cache.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/connection.pyi` & `django-stubs-4.2.3/django-stubs/utils/connection.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/crypto.pyi` & `django-stubs-4.2.3/django-stubs/utils/crypto.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/datastructures.pyi` & `django-stubs-4.2.3/django-stubs/utils/datastructures.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -108,8 +108,8 @@
 
 class CaseInsensitiveMapping(Mapping[str, _V]):
     _store: dict[str, tuple[str, _V]]
     def __init__(self, data: Mapping[str, _V] | Iterable[tuple[str, _V]]) -> None: ...
     def __getitem__(self, key: str) -> _V: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[str]: ...
-    def copy(self: Self) -> Self: ...
+    def copy(self) -> Self: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/utils/dateformat.pyi` & `django-stubs-4.2.3/django-stubs/utils/dateformat.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/datetime_safe.pyi` & `django-stubs-4.2.3/django-stubs/utils/datetime_safe.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/decorators.pyi` & `django-stubs-4.2.3/django-stubs/utils/decorators.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/deprecation.pyi` & `django-stubs-4.2.3/django-stubs/utils/deprecation.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,9 +38,9 @@
 
 class MiddlewareMixin:
     sync_capable: bool
     async_capable: bool
 
     get_response: _GetResponseCallable | _AsyncGetResponseCallable
     def __init__(self, get_response: _GetResponseCallable | _AsyncGetResponseCallable) -> None: ...
-    def __call__(self, request: HttpRequest) -> HttpResponseBase: ...
+    def __call__(self, request: HttpRequest) -> HttpResponseBase | Awaitable[HttpResponseBase]: ...
     async def __acall__(self, request: HttpRequest) -> HttpResponseBase: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/utils/encoding.pyi` & `django-stubs-4.2.3/django-stubs/utils/encoding.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/feedgenerator.pyi` & `django-stubs-4.2.3/django-stubs/utils/feedgenerator.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/formats.pyi` & `django-stubs-4.2.3/django-stubs/utils/formats.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/functional.pyi` & `django-stubs-4.2.3/django-stubs/utils/functional.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from collections.abc import Callable, Sequence
 from typing import Any, Generic, Protocol, SupportsIndex, TypeVar, overload
 
-from _typeshed import Self
 from django.db.models.base import Model
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 _T = TypeVar("_T")
 
 class cached_property(Generic[_T]):
     func: Callable[..., _T]
     name: str | None
     def __init__(self, func: Callable[..., _T], name: str | None = ...) -> None: ...
     @overload
-    def __get__(self: Self, instance: None, cls: type[Any] | None = ...) -> Self: ...
+    def __get__(self, instance: None, cls: type[Any] | None = ...) -> Self: ...
     @overload
     def __get__(self, instance: object, cls: type[Any] | None = ...) -> _T: ...
     def __set_name__(self, owner: type[Any], name: str) -> None: ...
 
 # Promise is only subclassed by a proxy class defined in the lazy function
 # so it makes sense for it to have all the methods available in that proxy class
 class Promise:
     def __init__(self, args: Any, kw: Any) -> None: ...
     def __reduce__(self) -> tuple[Any, tuple[Any]]: ...
     def __lt__(self, other: Any) -> bool: ...
     def __mod__(self, rhs: Any) -> Any: ...
     def __add__(self, other: Any) -> Any: ...
     def __radd__(self, other: Any) -> Any: ...
-    def __deepcopy__(self: Self, memo: Any) -> Self: ...
+    def __deepcopy__(self, memo: Any) -> Self: ...
 
 class _StrPromise(Promise, Sequence[str]):
     def __add__(self, __s: str) -> str: ...
     # Incompatible with Sequence.__contains__
     def __contains__(self, __o: str) -> bool: ...  # type: ignore[override]
     def __ge__(self, __x: str) -> bool: ...
     def __getitem__(self, __i: SupportsIndex | slice) -> str: ...
@@ -107,10 +106,10 @@
     """Type fake to declare some read-only properties (until `property` builtin is generic)
 
     We can use something like `Union[_Getter[str], str]` in base class to avoid errors
     when redefining attribute with property or property with attribute.
     """
 
     @overload
-    def __get__(self: Self, __instance: None, __typeobj: type[Any] | None) -> Self: ...
+    def __get__(self, __instance: None, __typeobj: type[Any] | None) -> Self: ...
     @overload
     def __get__(self, __instance: Any, __typeobj: type[Any] | None) -> _Get: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/utils/html.pyi` & `django-stubs-4.2.3/django-stubs/utils/html.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/http.pyi` & `django-stubs-4.2.3/django-stubs/utils/http.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/jslex.pyi` & `django-stubs-4.2.3/django-stubs/utils/jslex.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/log.pyi` & `django-stubs-4.2.3/django-stubs/utils/translation/__init__.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,49 @@
-import logging.config
-from collections.abc import Callable
-from logging import Logger, LogRecord
+from contextlib import ContextDecorator
+from types import TracebackType
 from typing import Any
 
-from django.core.management.color import Style
-from django.http import HttpRequest, HttpResponse
-from django.utils.functional import _StrOrPromise
-
-request_logger: Logger
-DEFAULT_LOGGING: Any
-
-def configure_logging(logging_config: str, logging_settings: dict[str, Any]) -> None: ...
-
-class AdminEmailHandler(logging.Handler):
-    include_html: bool
-    email_backend: str | None
-    def __init__(
+from django.http.request import HttpRequest
+from django.utils.functional import _StrPromise
+
+class TranslatorCommentWarning(SyntaxWarning): ...
+
+def gettext_noop(message: str) -> str: ...
+def gettext(message: str) -> str: ...
+def ngettext(singular: str, plural: str, number: float) -> str: ...
+def pgettext(context: str, message: str) -> str: ...
+def npgettext(context: str, singular: str, plural: str, number: int) -> str: ...
+
+# lazy evaluated translation functions
+def gettext_lazy(message: str) -> _StrPromise: ...
+def pgettext_lazy(context: str, message: str) -> _StrPromise: ...
+def ngettext_lazy(singular: str, plural: str, number: int | str | None = ...) -> _StrPromise: ...
+def npgettext_lazy(context: str, singular: str, plural: str, number: int | str | None = ...) -> _StrPromise: ...
+def activate(language: str) -> None: ...
+def deactivate() -> None: ...
+
+class override(ContextDecorator):
+    language: str | None
+    deactivate: bool
+    def __init__(self, language: str | None, deactivate: bool = ...) -> None: ...
+    old_language: str | None
+    def __enter__(self) -> None: ...
+    def __exit__(
         self,
-        include_html: bool = ...,
-        email_backend: str | None = ...,
-        reporter_class: str | None = ...,
+        exc_type: type[BaseException] | None,
+        exc_value: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None: ...
-    def send_mail(self, subject: _StrOrPromise, message: _StrOrPromise, *args: Any, **kwargs: Any) -> None: ...
-    def connection(self) -> Any: ...
-    def format_subject(self, subject: str) -> str: ...
-
-class CallbackFilter(logging.Filter):
-    callback: Callable
-    def __init__(self, callback: Callable) -> None: ...
-    def filter(self, record: str | LogRecord) -> bool: ...
-
-class RequireDebugFalse(logging.Filter):
-    def filter(self, record: str | LogRecord) -> bool: ...
-
-class RequireDebugTrue(logging.Filter):
-    def filter(self, record: str | LogRecord) -> bool: ...
-
-class ServerFormatter(logging.Formatter):
-    default_time_format: str
-    style: Style
-    def __init__(self, *args: Any, **kwargs: Any) -> None: ...
-    def uses_server_time(self) -> bool: ...
-
-def log_response(
-    message: str,
-    *args: Any,
-    response: HttpResponse | None = ...,
-    request: HttpRequest | None = ...,
-    logger: Logger = ...,
-    level: str | None = ...,
-    exception: BaseException | None = ...,
-) -> None: ...
+
+def get_language() -> str: ...
+def get_language_from_path(path: str) -> str | None: ...
+def get_language_bidi() -> bool: ...
+def check_for_language(lang_code: str | None) -> bool: ...
+def to_language(locale: str) -> str: ...
+def to_locale(language: str) -> str: ...
+def get_language_from_request(request: HttpRequest, check_path: bool = ...) -> str: ...
+def templatize(src: str, **kwargs: Any) -> str: ...
+def deactivate_all() -> None: ...
+def get_supported_language_variant(lang_code: str, *, strict: bool = ...) -> str: ...
+def get_language_info(lang_code: str) -> Any: ...
+def trim_whitespace(s: str) -> str: ...
+def round_away_from_one(value: int) -> int: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/utils/regex_helper.pyi` & `django-stubs-4.2.3/django-stubs/utils/regex_helper.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/safestring.pyi` & `django-stubs-4.2.3/django-stubs/utils/safestring.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from collections.abc import Callable
 from typing import Any, TypeVar, overload
 
-from _typeshed import Self
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 _SD = TypeVar("_SD", bound=SafeData)
 
 class SafeData:
-    def __html__(self: Self) -> Self: ...
+    def __html__(self) -> Self: ...
 
 class SafeString(str, SafeData):
     @overload
     def __add__(self, rhs: SafeString) -> SafeString: ...
     @overload
     def __add__(self, rhs: str) -> str: ...
```

### Comparing `django-stubs-4.2.2/django-stubs/utils/termcolors.pyi` & `django-stubs-4.2.3/django-stubs/utils/termcolors.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/text.pyi` & `django-stubs-4.2.3/django-stubs/utils/text.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/timezone.pyi` & `django-stubs-4.2.3/django-stubs/utils/timezone.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/translation/trans_null.pyi` & `django-stubs-4.2.3/django-stubs/utils/translation/trans_null.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/translation/trans_real.pyi` & `django-stubs-4.2.3/django-stubs/utils/translation/trans_real.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/tree.pyi` & `django-stubs-4.2.3/django-stubs/utils/tree.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/utils/version.pyi` & `django-stubs-4.2.3/django-stubs/utils/version.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/views/debug.pyi` & `django-stubs-4.2.3/django-stubs/views/debug.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/views/decorators/http.pyi` & `django-stubs-4.2.3/django-stubs/views/decorators/http.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/views/defaults.pyi` & `django-stubs-4.2.3/django-stubs/views/defaults.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/views/generic/__init__.pyi` & `django-stubs-4.2.3/django-stubs/views/generic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/views/generic/base.pyi` & `django-stubs-4.2.3/django-stubs/views/generic/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/views/generic/dates.pyi` & `django-stubs-4.2.3/django-stubs/views/generic/dates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/views/generic/detail.pyi` & `django-stubs-4.2.3/django-stubs/views/generic/detail.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/views/generic/edit.pyi` & `django-stubs-4.2.3/django-stubs/views/generic/edit.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/views/generic/list.pyi` & `django-stubs-4.2.3/django-stubs/views/generic/list.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django-stubs/views/i18n.pyi` & `django-stubs-4.2.3/django-stubs/views/i18n.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/django_stubs.egg-info/PKG-INFO` & `django-stubs-4.2.3/django_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-stubs
-Version: 4.2.2
+Version: 4.2.3
 Summary: Mypy stubs for Django
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
@@ -72,14 +72,15 @@
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
 | django-stubs   | Mypy version | Django version | Django partial support | Python version |
 |----------------|--------------|----------------|------------------------|----------------|
+| 4.2.3          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.2          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.1          | 1.3.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.0          | 1.2.x        | 4.2            | 4.1, 4.0, 3.2          | 3.7 - 3.11     |
 | 1.16.0         | 1.1.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 | 1.15.0         | 1.0.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 | 1.14.0         | 0.990+       | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
```

### Comparing `django-stubs-4.2.2/django_stubs.egg-info/SOURCES.txt` & `django-stubs-4.2.3/django_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/mypy_django_plugin/config.py` & `django-stubs-4.2.3/mypy_django_plugin/config.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/mypy_django_plugin/django/context.py` & `django-stubs-4.2.3/mypy_django_plugin/django/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,20 +56,19 @@
 
         # add current directory to sys.path
         sys.path.append(os.getcwd())
 
         from django.apps import apps
         from django.conf import settings
 
-        apps.get_models.cache_clear()  # type: ignore
         apps.get_swappable_settings_name.cache_clear()  # type: ignore
+        apps.clear_cache()
 
         if not settings.configured:
             settings._setup()  # type: ignore
-
         apps.populate(settings.INSTALLED_APPS)
 
     assert apps.apps_ready, "Apps are not ready"
     assert settings.configured, "Settings are not configured"
 
     return apps, settings
```

### Comparing `django-stubs-4.2.2/mypy_django_plugin/lib/fullnames.py` & `django-stubs-4.2.3/mypy_django_plugin/lib/fullnames.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/mypy_django_plugin/lib/helpers.py` & `django-stubs-4.2.3/mypy_django_plugin/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/mypy_django_plugin/main.py` & `django-stubs-4.2.3/mypy_django_plugin/main.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/mypy_django_plugin/transformers/fields.py` & `django-stubs-4.2.3/mypy_django_plugin/transformers/fields.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/mypy_django_plugin/transformers/forms.py` & `django-stubs-4.2.3/mypy_django_plugin/transformers/forms.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/mypy_django_plugin/transformers/functional.py` & `django-stubs-4.2.3/mypy_django_plugin/transformers/functional.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/mypy_django_plugin/transformers/init_create.py` & `django-stubs-4.2.3/mypy_django_plugin/transformers/init_create.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/mypy_django_plugin/transformers/managers.py` & `django-stubs-4.2.3/mypy_django_plugin/transformers/managers.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/mypy_django_plugin/transformers/meta.py` & `django-stubs-4.2.3/mypy_django_plugin/transformers/meta.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/mypy_django_plugin/transformers/models.py` & `django-stubs-4.2.3/mypy_django_plugin/transformers/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -553,29 +553,29 @@
             if isinstance(field, (DateField, DateTimeField)) and not field.null:
                 return_type = Instance(self.model_classdef.info, [])
                 common.add_method(
                     self.ctx,
                     name=f"get_next_by_{field.attname}",
                     args=[
                         Argument(
-                            Var("kwargs", AnyType(TypeOfAny.explicit)),
-                            AnyType(TypeOfAny.explicit),
+                            Var("kwargs", AnyType(TypeOfAny.implementation_artifact)),
+                            AnyType(TypeOfAny.implementation_artifact),
                             initializer=None,
                             kind=ARG_STAR2,
                         )
                     ],
                     return_type=return_type,
                 )
                 common.add_method(
                     self.ctx,
                     name=f"get_previous_by_{field.attname}",
                     args=[
                         Argument(
-                            Var("kwargs", AnyType(TypeOfAny.explicit)),
-                            AnyType(TypeOfAny.explicit),
+                            Var("kwargs", AnyType(TypeOfAny.implementation_artifact)),
+                            AnyType(TypeOfAny.implementation_artifact),
                             initializer=None,
                             kind=ARG_STAR2,
                         )
                     ],
                     return_type=return_type,
                 )
```

### Comparing `django-stubs-4.2.2/mypy_django_plugin/transformers/orm_lookups.py` & `django-stubs-4.2.3/mypy_django_plugin/transformers/orm_lookups.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/mypy_django_plugin/transformers/querysets.py` & `django-stubs-4.2.3/mypy_django_plugin/transformers/querysets.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/mypy_django_plugin/transformers/request.py` & `django-stubs-4.2.3/mypy_django_plugin/transformers/request.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/mypy_django_plugin/transformers/settings.py` & `django-stubs-4.2.3/mypy_django_plugin/transformers/settings.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.2/setup.py` & `django-stubs-4.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 # Keep compatible-mypy major.minor version pinned to what we use in CI (requirements.txt)
 extras_require = {
     "compatible-mypy": ["mypy==1.4.*"],
 }
 
 setup(
     name="django-stubs",
-    version="4.2.2",
+    version="4.2.3",
     description="Mypy stubs for Django",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     license_files=["LICENSE.md"],
     url="https://github.com/typeddjango/django-stubs",
     author="Maksim Kurnikov",
```

### Comparing `django-stubs-4.2.2/tests/test_error_handling.py` & `django-stubs-4.2.3/tests/test_error_handling.py`

 * *Files identical despite different names*

