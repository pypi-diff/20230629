# Comparing `tmp/sloth-framework-0.1.8.tar.gz` & `tmp/sloth-framework-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sloth-framework-0.1.8.tar", last modified: Tue May 30 11:20:12 2023, max compression
+gzip compressed data, was "sloth-framework-0.1.9.tar", last modified: Wed Jun  7 23:17:24 2023, max compression
```

## Comparing `sloth-framework-0.1.8.tar` & `sloth-framework-0.1.9.tar`

### file list

```diff
@@ -1,314 +1,315 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/actions/
--rw-r--r--   0 runner    (1001) docker     (123)    40361 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/actions/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/actions/inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21543 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/api/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/api/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/api/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.726862 sloth-framework-0.1.8/sloth/api/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/reset_passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/selenium.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/send_web_push_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/startserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/sync_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.726862 sloth-framework-0.1.8/sloth/api/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0002_role_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0003_alter_application_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0004_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0005_task_stopped_alter_task_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0009_pushnotification.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0010_alter_pushnotification_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0011_alter_application_client_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0012_authcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0013_task_partial_task_total.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0014_email.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/api/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.726862 sloth-framework-0.1.8/sloth/api/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/all.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/bootstrap-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    33038 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/bpmn.css
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/colorpick.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.730862 sloth-framework-0.1.8/sloth/api/static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   107280 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   116316 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   112880 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   111976 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    83304 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    47832 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.eot
--rw-r--r--   0 runner    (1001) docker     (123)   133048 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.svg
--rw-r--r--   0 runner    (1001) docker     (123)    47680 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/icons.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.730862 sloth-framework-0.1.8/sloth/api/static/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/jquery-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/leaflet.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/sloth.css
--rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/trumbowyg.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/api/static/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.730862 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/
--rw-r--r--   0 runner    (1001) docker     (123)   100170 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/fontawesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)  1726692 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/fontawesome.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.730862 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.734862 sloth-framework-0.1.8/sloth/api/static/icons/materialicons/
--rw-r--r--   0 runner    (1001) docker     (123)   174176 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   127220 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   155604 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/materialicons/materialicons.css
--rw-r--r--   0 runner    (1001) docker     (123)   135988 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.734862 sloth-framework-0.1.8/sloth/api/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    57420 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/click.png
--rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/hand.png
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.734862 sloth-framework-0.1.8/sloth/api/static/images/images/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/images/badge.png
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/login.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/no-image.png
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/sloth.png
--rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/user.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.738862 sloth-framework-0.1.8/sloth/api/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/api.js
--rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)  1665279 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/bpmn.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     4098 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/colorpick.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.738862 sloth-framework-0.1.8/sloth/api/static/js/i18n/
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/i18n/pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   520714 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/jquery.binarytransport.js
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/jquery.mask.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    80794 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/jquery.timepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)   147555 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/leaflet.js
--rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/masonry.pkgd.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/qr-scanner-worker.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/qr-scanner.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/qrcode.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    17825 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/sloth.js
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/sw.js
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/tests.js
--rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/trumbowyg.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/wpn.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.738862 sloth-framework-0.1.8/sloth/api/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/api/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.738862 sloth-framework-0.1.8/sloth/api/templates/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/actions/execute_query.html
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/actions/execute_script.html
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/actions/show_icons.html
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/actions/workflow.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.738862 sloth-framework-0.1.8/sloth/api/templates/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/api/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.738862 sloth-framework-0.1.8/sloth/api/templates/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/charts/bar.html
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/charts/column.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/charts/donut.html
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/charts/legend.html
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/charts/pie.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/apps.html
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/dashboards.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/default.html
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/form.html
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/grids.html
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/header.html
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/links.html
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/messages.html
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/plus.html
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/report.html
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/shortcuts.html
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/tasks.html
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/tools.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/inputs/picker.html
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/inputs/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/inputs/select.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/queryset/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/accordion.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/queryset/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/actions/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/actions/batch.html
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/actions/global.html
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/calendar.html
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/datatable.html
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/filter.html
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/filters.html
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/queryset.html
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/rows.html
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/scroll.html
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/statistics.html
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/timeline.html
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/api/templates/renderers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/renderers/badges/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/badges/badge.html
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/badges/boolean.html
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/badges/danger.html
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/badges/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/badges/status.html
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/badges/warning.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/renderers/boolean/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/boolean/thumb.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/renderers/calendar/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/calendar/calendar.html
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/calendar/events.html
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/calendar/legend.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/renderers/documents/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/documents/document.html
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/documents/popup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/renderers/images/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/images/banner.html
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/images/group.html
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/images/image.html
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/images/round.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/links/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/links/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/links/url.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/maps/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/maps/geolocation.html
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/maps/map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/messages/custom.html
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/messages/danger.html
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/messages/message.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/messages/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/messages/success.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/messages/warning.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/photos/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/photos/photo.html
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/photos/round.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/programing/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/programing/strtable.html
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/programing/terminal.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/progress/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/progress/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/progress/success.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/statistics/cards.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/steps/check.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/tags/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/tags/tags.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/utils/formatted.html
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/utils/progress.html
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/utils/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/utils/steps.html
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/utils/table.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/themes/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/themes/dark.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/valueset/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/2-column.html
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/field.html
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/fieldset-group.html
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/fieldset-list.html
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/fieldset-tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/primitive.html
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/value.html
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/valueset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templatetags/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/cloud/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/cloud/printer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6116 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/cloud/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/conf/local_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    43817 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/core/queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/core/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/core/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21157 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/core/valueset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/db/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/test/selenium/
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/test/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/test/selenium/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/utils/formatter/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/formatter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/utils/http/
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/utils/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/icons/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    53105 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/icons/fontawesome.py
--rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/icons/materialicons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/utils/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/log/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-30 11:20:12.000000 sloth-framework-0.1.8/sloth_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-05-30 11:20:12.000000 sloth-framework-0.1.8/sloth_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:20:12.000000 sloth-framework-0.1.8/sloth_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-30 11:20:12.000000 sloth-framework-0.1.8/sloth_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 11:20:12.000000 sloth-framework-0.1.8/sloth_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.868951 sloth-framework-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-07 23:17:24.868951 sloth-framework-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 23:17:24.868951 sloth-framework-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.788951 sloth-framework-0.1.9/sloth/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.788951 sloth-framework-0.1.9/sloth/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    40361 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/actions/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/actions/inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.788951 sloth-framework-0.1.9/sloth/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21616 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.788951 sloth-framework-0.1.9/sloth/api/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.792951 sloth-framework-0.1.9/sloth/api/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.792951 sloth-framework-0.1.9/sloth/api/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.792951 sloth-framework-0.1.9/sloth/api/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/management/commands/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/management/commands/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/management/commands/reset_passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/management/commands/selenium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/management/commands/send_web_push_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/management/commands/startserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/management/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/management/commands/sync_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/management/commands/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.796951 sloth-framework-0.1.9/sloth/api/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/migrations/0002_role_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/migrations/0003_alter_application_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/migrations/0004_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/migrations/0005_task_stopped_alter_task_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/migrations/0009_pushnotification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/migrations/0010_alter_pushnotification_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/migrations/0011_alter_application_client_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/migrations/0012_authcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/migrations/0013_task_partial_task_total.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/migrations/0014_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11106 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.776951 sloth-framework-0.1.9/sloth/api/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.800951 sloth-framework-0.1.9/sloth/api/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/all.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/bootstrap-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    33038 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/bpmn.css
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/colorpick.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.804951 sloth-framework-0.1.9/sloth/api/static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   107280 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   116316 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   112880 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   111976 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    83304 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    47832 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/fonts/bpmn.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   133048 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/fonts/bpmn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    47680 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/fonts/bpmn.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/fonts/bpmn.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/fonts/bpmn.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/icons.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.804951 sloth-framework-0.1.9/sloth/api/static/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/leaflet.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/sloth.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/css/trumbowyg.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.776951 sloth-framework-0.1.9/sloth/api/static/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.808951 sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (123)   100170 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1726692 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/fontawesome.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.812951 sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.812951 sloth-framework-0.1.9/sloth/api/static/icons/materialicons/
+-rw-r--r--   0 runner    (1001) docker     (123)   174176 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   127220 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   155604 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/icons/materialicons/materialicons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   135988 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.816951 sloth-framework-0.1.9/sloth/api/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    57420 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/images/click.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/images/hand.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/images/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.816951 sloth-framework-0.1.9/sloth/api/static/images/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/images/images/badge.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/images/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/images/login.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/images/no-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/images/sloth.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/images/user.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.828951 sloth-framework-0.1.9/sloth/api/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1665279 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/bpmn.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4098 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/colorpick.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.828951 sloth-framework-0.1.9/sloth/api/static/js/i18n/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/i18n/pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   520714 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/jquery.binarytransport.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/jquery.mask.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80794 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/jquery.timepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   147555 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/leaflet.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/masonry.pkgd.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/qr-scanner-worker.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/qr-scanner.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/qrcode.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16688 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/sloth.js
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/sw.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/tests.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/trumbowyg.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/static/js/wpn.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.828951 sloth-framework-0.1.9/sloth/api/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.784951 sloth-framework-0.1.9/sloth/api/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.828951 sloth-framework-0.1.9/sloth/api/templates/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/actions/execute_query.html
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/actions/execute_script.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/actions/show_icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/actions/workflow.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.828951 sloth-framework-0.1.9/sloth/api/templates/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/api/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.828951 sloth-framework-0.1.9/sloth/api/templates/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/charts/bar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/charts/column.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/charts/donut.html
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/charts/legend.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/charts/pie.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.836951 sloth-framework-0.1.9/sloth/api/templates/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/apps.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/dashboards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/default.html
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/grids.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/links.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/plus.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/shortcuts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/tasks.html
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/dashboard/tools.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.836951 sloth-framework-0.1.9/sloth/api/templates/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/inputs/picker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/inputs/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/inputs/select.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.840951 sloth-framework-0.1.9/sloth/api/templates/queryset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/queryset/accordion.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.840951 sloth-framework-0.1.9/sloth/api/templates/queryset/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/queryset/actions/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/queryset/actions/batch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/queryset/actions/global.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/queryset/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/queryset/cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/queryset/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/queryset/datatable.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/queryset/filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/queryset/filters.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/queryset/queryset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/queryset/rows.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/queryset/scroll.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/queryset/statistics.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/queryset/timeline.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/queryset/tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.780951 sloth-framework-0.1.9/sloth/api/templates/renderers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.844951 sloth-framework-0.1.9/sloth/api/templates/renderers/badges/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/badges/badge.html
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/badges/boolean.html
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/badges/danger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/badges/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/badges/status.html
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/badges/warning.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.844951 sloth-framework-0.1.9/sloth/api/templates/renderers/boolean/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/boolean/thumb.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.844951 sloth-framework-0.1.9/sloth/api/templates/renderers/calendar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/calendar/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/calendar/events.html
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/calendar/legend.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.844951 sloth-framework-0.1.9/sloth/api/templates/renderers/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/documents/document.html
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/documents/popup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.848951 sloth-framework-0.1.9/sloth/api/templates/renderers/images/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/images/banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/images/group.html
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/images/image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/images/round.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.848951 sloth-framework-0.1.9/sloth/api/templates/renderers/links/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/links/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/links/url.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.848951 sloth-framework-0.1.9/sloth/api/templates/renderers/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/maps/geolocation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/maps/map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.848951 sloth-framework-0.1.9/sloth/api/templates/renderers/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/messages/custom.html
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/messages/danger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/messages/message.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/messages/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/messages/success.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/messages/warning.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.852951 sloth-framework-0.1.9/sloth/api/templates/renderers/photos/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/photos/photo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/photos/round.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.852951 sloth-framework-0.1.9/sloth/api/templates/renderers/programing/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/programing/strtable.html
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/programing/terminal.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.852951 sloth-framework-0.1.9/sloth/api/templates/renderers/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/progress/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/progress/success.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.852951 sloth-framework-0.1.9/sloth/api/templates/renderers/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/statistics/cards.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.852951 sloth-framework-0.1.9/sloth/api/templates/renderers/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/steps/check.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.852951 sloth-framework-0.1.9/sloth/api/templates/renderers/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/tags/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/tags/tags.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.856951 sloth-framework-0.1.9/sloth/api/templates/renderers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/utils/formatted.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/utils/progress.html
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/utils/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/utils/steps.html
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/renderers/utils/table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.856951 sloth-framework-0.1.9/sloth/api/templates/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/themes/dark.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.856951 sloth-framework-0.1.9/sloth/api/templates/valueset/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/valueset/2-column.html
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/valueset/field.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/valueset/fieldset-group.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/valueset/fieldset-list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/valueset/fieldset-tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/valueset/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/valueset/primitive.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/valueset/value.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templates/valueset/valueset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.856951 sloth-framework-0.1.9/sloth/api/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/templatetags/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.860952 sloth-framework-0.1.9/sloth/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/cloud/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/cloud/printer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6127 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/cloud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.860952 sloth-framework-0.1.9/sloth/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/conf/local_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.860952 sloth-framework-0.1.9/sloth/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21816 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43817 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/core/queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/core/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/core/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21157 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/core/valueset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.860952 sloth-framework-0.1.9/sloth/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.860952 sloth-framework-0.1.9/sloth/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.860952 sloth-framework-0.1.9/sloth/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.864951 sloth-framework-0.1.9/sloth/test/selenium/
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/test/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/test/selenium/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.864951 sloth-framework-0.1.9/sloth/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.864951 sloth-framework-0.1.9/sloth/utils/formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/utils/formatter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.864951 sloth-framework-0.1.9/sloth/utils/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/utils/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.864951 sloth-framework-0.1.9/sloth/utils/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/utils/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/utils/icons/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53105 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/utils/icons/fontawesome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/utils/icons/materialicons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.864951 sloth-framework-0.1.9/sloth/utils/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/utils/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-07 23:17:19.000000 sloth-framework-0.1.9/sloth/utils/log/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:17:24.868951 sloth-framework-0.1.9/sloth_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-07 23:17:24.000000 sloth-framework-0.1.9/sloth_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-06-07 23:17:24.000000 sloth-framework-0.1.9/sloth_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 23:17:24.000000 sloth-framework-0.1.9/sloth_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-07 23:17:24.000000 sloth-framework-0.1.9/sloth_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 23:17:24.000000 sloth-framework-0.1.9/sloth_framework.egg-info/top_level.txt
```

### Comparing `sloth-framework-0.1.8/PKG-INFO` & `sloth-framework-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sloth-framework
-Version: 0.1.8
+Version: 0.1.9
 Summary: Metadata-based web framework for the development of management information systems
 Home-page: http://sloth.aplicativo.click/
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `sloth-framework-0.1.8/setup.py` & `sloth-framework-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open(os.path.join(root_dir, 'sloth/requirements.txt')) as file:
     requirements = file.read().strip().splitlines()
 
 os.chdir(root_dir)
 
 setup(
     name='sloth-framework',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     install_requires=requirements,
     extras_require={
         'dev': [],
         'production': [],
     },
     include_package_data=True,
```

### Comparing `sloth-framework-0.1.8/sloth/Dockerfile` & `sloth-framework-0.1.9/sloth/Dockerfile`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/__init__.py` & `sloth-framework-0.1.9/sloth/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/actions/__init__.py` & `sloth-framework-0.1.9/sloth/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/actions/fields.py` & `sloth-framework-0.1.9/sloth/actions/fields.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 
 
 class QrCodeField(forms.CharField):
     def __init__(self, *args, **kwargs):
         kwargs.update(widget=inputs.QrCodeInput())
         super().__init__(*args, **kwargs)
 
+class PhotoField(forms.CharField):
+    def __init__(self, *args, max_width=200, max_height=200, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.widget.attrs.update(
+            {'data-max-width': self.max_width, 'data-max-height': self.max_height, 'accept': 'image/*', 'capture': ''}
+        )
+
 
 class ModelChoiceField(forms.ModelChoiceField):
     def __init__(self, *args, **kwargs):
         self.username_lookup = kwargs.pop('username_lookup', None)
         super().__init__(*args, **kwargs)
```

### Comparing `sloth-framework-0.1.8/sloth/actions/inputs.py` & `sloth-framework-0.1.9/sloth/actions/inputs.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/__init__.py` & `sloth-framework-0.1.9/sloth/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/actions.py` & `sloth-framework-0.1.9/sloth/api/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,17 +447,19 @@
         }
 
     def submit(self):
         self.instance.set_password(self.cleaned_data.get('pass1'))
         super().submit()
 
     def clean(self):
-        if User.objects.filter(username=self.cleaned_data.get('username')):
+        username = self.cleaned_data.get('username')
+        email = self.cleaned_data.get('email')
+        if username and User.objects.filter(username=username):
             raise actions.ValidationError('Usuário já cadastrado.')
-        if User.objects.filter(email=self.cleaned_data.get('email')):
+        if email and User.objects.filter(email=email):
             raise actions.ValidationError('E-mail já cadastrado.')
         if self.cleaned_data.get('pass1') != self.cleaned_data.get('pass2'):
             raise actions.ValidationError('Senhas não conferem.')
         return self.cleaned_data
 
     def has_permission(self, user):
         return not user.is_authenticated
```

### Comparing `sloth-framework-0.1.8/sloth/api/backends/__init__.py` & `sloth-framework-0.1.9/sloth/api/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/dashboard.py` & `sloth-framework-0.1.9/sloth/api/dashboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
         return ValueSet(self, names)
 
     def has_attr_permission(self, user, name):
         attr = getattr(self, 'has_{}_permission'.format(name), None)
         return attr is None or attr(user)
 
     def objects(self, model_name):
-        qs = apps.get_model(model_name).objects.all()
+        qs = apps.get_model(model_name).objects
         qs.request = self.request
         return qs.apply_role_lookups(self.request.user, self.request.session)
 
     @classmethod
     def get_attr_metadata(cls, lookup):
         attr = getattr(cls, lookup)
         template = getattr(attr, '__template__', None)
```

### Comparing `sloth-framework-0.1.8/sloth/api/management/commands/cloud.py` & `sloth-framework-0.1.9/sloth/api/management/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/management/commands/query.py` & `sloth-framework-0.1.9/sloth/api/management/commands/query.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/management/commands/send_web_push_notification.py` & `sloth-framework-0.1.9/sloth/api/management/commands/send_web_push_notification.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/management/commands/startserver.py` & `sloth-framework-0.1.9/sloth/api/management/commands/startserver.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/management/commands/sync.py` & `sloth-framework-0.1.9/sloth/api/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/migrations/0001_initial.py` & `sloth-framework-0.1.9/sloth/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/migrations/0002_role_user.py` & `sloth-framework-0.1.9/sloth/api/migrations/0002_role_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/migrations/0003_alter_application_user.py` & `sloth-framework-0.1.9/sloth/api/migrations/0003_alter_application_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/migrations/0004_task.py` & `sloth-framework-0.1.9/sloth/api/migrations/0004_task.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/migrations/0005_task_stopped_alter_task_message.py` & `sloth-framework-0.1.9/sloth/api/migrations/0005_task_stopped_alter_task_message.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py` & `sloth-framework-0.1.9/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py` & `sloth-framework-0.1.9/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py` & `sloth-framework-0.1.9/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/migrations/0009_pushnotification.py` & `sloth-framework-0.1.9/sloth/api/migrations/0009_pushnotification.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/migrations/0010_alter_pushnotification_user.py` & `sloth-framework-0.1.9/sloth/api/migrations/0010_alter_pushnotification_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/migrations/0011_alter_application_client_secret.py` & `sloth-framework-0.1.9/sloth/api/migrations/0011_alter_application_client_secret.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/migrations/0012_authcode.py` & `sloth-framework-0.1.9/sloth/api/migrations/0012_authcode.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/migrations/0013_task_partial_task_total.py` & `sloth-framework-0.1.9/sloth/api/migrations/0013_task_partial_task_total.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/migrations/0014_email.py` & `sloth-framework-0.1.9/sloth/api/migrations/0014_email.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/models.py` & `sloth-framework-0.1.9/sloth/api/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
 class PushNotification(models.Model):
     user = models.OneToOneField(DjangoUser, verbose_name='Usuário', on_delete=models.CASCADE, related_name='push_notification')
     subscription = models.JSONField(verbose_name='Dados da Inscrição')
 
 
 class EmailManager(models.Manager):
     def all(self):
-        return self.rows()
+        return self.rows().order_by('-id')
 
     def send(self, to, subject, content, from_email=None):
         to = [to] if isinstance(to, str) else list(to)
         return self.create(from_email=from_email or 'no-replay@mail.com', to=', '.join(to), subject=subject, content=content)
 
 
 class Email(models.Model):
```

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/all.min.css` & `sloth-framework-0.1.9/sloth/api/static/css/all.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/bootstrap-icons.css` & `sloth-framework-0.1.9/sloth/api/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/bootstrap.min.css` & `sloth-framework-0.1.9/sloth/api/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/bpmn.css` & `sloth-framework-0.1.9/sloth/api/static/css/bpmn.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/colorpick.min.css` & `sloth-framework-0.1.9/sloth/api/static/css/colorpick.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf` & `sloth-framework-0.1.9/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf` & `sloth-framework-0.1.9/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf` & `sloth-framework-0.1.9/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/fonts/bootstrap-icons.woff` & `sloth-framework-0.1.9/sloth/api/static/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/fonts/bootstrap-icons.woff2` & `sloth-framework-0.1.9/sloth/api/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.eot` & `sloth-framework-0.1.9/sloth/api/static/css/fonts/bpmn.eot`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.svg` & `sloth-framework-0.1.9/sloth/api/static/css/fonts/bpmn.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.ttf` & `sloth-framework-0.1.9/sloth/api/static/css/fonts/bpmn.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.woff` & `sloth-framework-0.1.9/sloth/api/static/css/fonts/bpmn.woff`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.woff2` & `sloth-framework-0.1.9/sloth/api/static/css/fonts/bpmn.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/icons.svg` & `sloth-framework-0.1.9/sloth/api/static/css/icons.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/images/ui-icons_444444_256x240.png` & `sloth-framework-0.1.9/sloth/api/static/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/images/ui-icons_555555_256x240.png` & `sloth-framework-0.1.9/sloth/api/static/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/jquery-ui.css` & `sloth-framework-0.1.9/sloth/api/static/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/leaflet.css` & `sloth-framework-0.1.9/sloth/api/static/css/leaflet.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/select2.min.css` & `sloth-framework-0.1.9/sloth/api/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/sloth.css` & `sloth-framework-0.1.9/sloth/api/static/css/sloth.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/css/trumbowyg.min.css` & `sloth-framework-0.1.9/sloth/api/static/css/trumbowyg.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/fontawesome.min.css` & `sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/fontawesome.min.js` & `sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/fontawesome.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf` & `sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2` & `sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf` & `sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2` & `sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf` & `sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2` & `sloth-framework-0.1.9/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2` & `sloth-framework-0.1.9/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2` & `sloth-framework-0.1.9/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2` & `sloth-framework-0.1.9/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/icons/materialicons/materialicons.css` & `sloth-framework-0.1.9/sloth/api/static/icons/materialicons/materialicons.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2` & `sloth-framework-0.1.9/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/images/click.png` & `sloth-framework-0.1.9/sloth/api/static/images/click.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/images/hand.png` & `sloth-framework-0.1.9/sloth/api/static/images/hand.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/images/icon.png` & `sloth-framework-0.1.9/sloth/api/static/images/icon.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/images/icon.svg` & `sloth-framework-0.1.9/sloth/api/static/images/icon.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/images/images/badge.png` & `sloth-framework-0.1.9/sloth/api/static/images/images/badge.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/images/images/icon.png` & `sloth-framework-0.1.9/sloth/api/static/images/images/icon.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/images/login.jpeg` & `sloth-framework-0.1.9/sloth/api/static/images/login.jpeg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/images/logo.png` & `sloth-framework-0.1.9/sloth/api/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/images/logo.svg` & `sloth-framework-0.1.9/sloth/api/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/images/no-image.png` & `sloth-framework-0.1.9/sloth/api/static/images/no-image.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/images/sloth.png` & `sloth-framework-0.1.9/sloth/api/static/images/sloth.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/images/user.png` & `sloth-framework-0.1.9/sloth/api/static/images/user.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/api.js` & `sloth-framework-0.1.9/sloth/api/static/js/api.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/bootstrap.bundle.min.js` & `sloth-framework-0.1.9/sloth/api/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/bpmn.js` & `sloth-framework-0.1.9/sloth/api/static/js/bpmn.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/colorpick.min.js` & `sloth-framework-0.1.9/sloth/api/static/js/colorpick.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/i18n/pt-BR.js` & `sloth-framework-0.1.9/sloth/api/static/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/jquery-3.6.0.min.js` & `sloth-framework-0.1.9/sloth/api/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/jquery-ui.js` & `sloth-framework-0.1.9/sloth/api/static/js/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/jquery.binarytransport.js` & `sloth-framework-0.1.9/sloth/api/static/js/jquery.binarytransport.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/jquery.mask.min.js` & `sloth-framework-0.1.9/sloth/api/static/js/jquery.mask.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/jquery.timepicker.js` & `sloth-framework-0.1.9/sloth/api/static/js/jquery.timepicker.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/leaflet.js` & `sloth-framework-0.1.9/sloth/api/static/js/leaflet.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/masonry.pkgd.min.js` & `sloth-framework-0.1.9/sloth/api/static/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/popper.min.js` & `sloth-framework-0.1.9/sloth/api/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/qr-scanner-worker.min.js` & `sloth-framework-0.1.9/sloth/api/static/js/qr-scanner-worker.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/qr-scanner.min.js` & `sloth-framework-0.1.9/sloth/api/static/js/qr-scanner.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/qrcode.min.js` & `sloth-framework-0.1.9/sloth/api/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/select2.min.js` & `sloth-framework-0.1.9/sloth/api/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/sloth.js` & `sloth-framework-0.1.9/sloth/api/static/js/sloth.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -56,44 +56,51 @@
         });
     },
     open: function(url, method, data) {
         $(this).request(url, method || 'GET', data || {}, function(html) {
             $('main').html(html).initialize();
         });
     },
-    ipopup: function(url) {
-        var html = '<iframe src="' + url + '" width="100%" height="500px"></iframe>';
-        $('#modal').find('.modal-body').html(html);
-        $('#modal').modal('show');
-        $('#modal').find('.modal-body').css('visibility', 'visible');
-    },
-    popup: function(url, method, data) {
-        $('.alert-dismissible').hide();
-        if (url.indexOf('?') > 0) url = url += '&modal=1'
-        else url += '?modal=1'
-
+    setUpPopupStack: function() {
         if (window['POPUP_STACK'] == null) {
             window['POPUP_STACK'] = [];
             window['POPUP_STACK_SELECT2'] = [];
             $('#modal').on('hidden.bs.modal', function(e) {
                 if (window['POPUP_STACK'].length > 0) {
                     $('#modal .modal-body').replaceWith(window['POPUP_STACK'].pop().initialize());
                     $('#modal').modal('show');
                     $('#modal').find('.modal-body').css('visibility', 'visible');
                     var vals = window['POPUP_STACK_SELECT2'].pop();
                     for (k in vals) {
                         $('#' + k).val(vals[k]).trigger('change')
                     }
                 } else $('#modal').find('.modal-body').html('');
+                testLoggerIdent = testLoggerIdent.substring(0, 8 - 4);
             });
             $('#modal').on('shown.bs.modal', function(e) {
                 $('#modal').responsive();
+                testLoggerIdent += '    ';
                 testlogger("self.look_at_popup_window()");
+                var h2 = $('#modal').find('h2');
+                if (h2.length) testlogger("self.look_at('" + $(h2[0]).text().trim() + "')");
             });
         }
+    },
+    ipopup: function(url) {
+        var html = '<iframe src="' + url + '" width="100%" height="500px"></iframe>';
+        $('#modal').setUpPopupStack();
+        $('#modal').find('.modal-body').html(html);
+        $('#modal').modal('show');
+        $('#modal').find('.modal-body').css('visibility', 'visible');
+    },
+    popup: function(url, method, data) {
+        $('.alert-dismissible').hide();
+        if (url.indexOf('?') > 0) url = url += '&modal=1'
+        else url += '?modal=1'
+        $('#modal').setUpPopupStack();
         if ($('#modal').find('.modal-body').html().trim()) {
             $('#modal').find('.modal-body').css('visibility', 'hidden');
             $('#modal .modal-body .select2-hidden-accessible').select2("destroy");
             window['POPUP_STACK'].push($('#modal').find('.modal-body').clone());
             var vals = {};
             var elements = $('.modal-body select');
             for (var i = 0; i < elements.length; i++) vals[elements[i].id] = $(elements[i]).val();
@@ -152,17 +159,18 @@
         return this;
     },
     getCookie: function(name) {
         var match = document.cookie.match(new RegExp('(^| )' + name + '=([^;]+)'));
         if (match) return match[2];
     },
     setCookie: function(name, value) {
-        document.cookie = name + "=" + value;
+        document.cookie = name + "=" + value + "; path=/";
     },
     initialize: function() {
+        initTestLogger(this);
         $(this).find('a.popup').on('click', function(e) {
             $(this).popup(this.href);
             e.preventDefault();
             return false;
         });
         $(this).find('.ajax').on('click', function(e) {
             $(this).open(this.href);
@@ -260,66 +268,52 @@
         $(this).find('.image-input').each(function(index) {
             var input = this;
             input.addEventListener('change', function(e) {
                 if (e.target.files) {
                     let imageFile = e.target.files[0];
                     var reader = new FileReader();
                     reader.onload = function(e) {
-                        const MAX_WIDTH = 800;
+                        const MAX_WIDTH = $(input).data('max-width') || 800;
                         var img = document.createElement("img");
+                        img.id = input.id + 'img';
                         img.onload = function(event) {
                             const ratio = MAX_WIDTH / img.width;
                             var canvas = document.createElement("canvas");
                             const ctx = canvas.getContext("2d");
                             canvas.height = canvas.width * (img.height / img.width);
                             const oc = document.createElement('canvas');
                             const octx = oc.getContext('2d');
                             oc.width = img.width * ratio;
                             oc.height = img.height * ratio;
                             octx.drawImage(img, 0, 0, oc.width, oc.height);
                             ctx.drawImage(oc, 0, 0, oc.width * ratio, oc.height * ratio, 0, 0, canvas.width, canvas.height);
-                            //document.getElementById("preview").src = dataurl;
                             oc.toBlob(function(blob) {
                                 $(input).addClass('resized-image');
                                 $(input).data('blob', blob);
                             });
+                            $('#cotainer' + img.id).remove();
+                            $(img).css('max-width', '200px').css('margin', '20px');
+                            var container = document.createElement("div");
+                            container.id = 'cotainer' + img.id;
+                            $(container).css('text-align', 'center').append(img);
+                            $(input).parent().append(container);
                         }
                         img.src = e.target.result;
                     }
                     reader.readAsDataURL(imageFile);
                 }
             });
         });
         $(document).on('select2:open', () => {
             $(this).closest('.select2-search__field').focus();
         });
         $('.fieldset-tab').map(function(i, item) {
             var fieldsets = $(this).find('.reloadable-fieldset, .reloadable-queryset');
             if (fieldsets.length == 1) fieldsets.find('.queryset-title, .fieldset-title').hide();
         });
-
-        if (window.testlogger && false) {
-            function formatValue(value) {
-                if (value && value.length == 10 && value.indexOf('-') == 4) {
-                    var tokens = value.split('-');
-                    if (tokens.length == 3) return tokens[2] + '/' + tokens[1] + '/' + tokens[0];
-                }
-                return value;
-            }
-            //            $(this).find('input, textarea').not('input[type=checkbox]').blur(function(){testlogger("self.enter('"+$(this).parent().find('label').html().trim().replace('*', '')+"', '"+formatValue($(this).val())+"')")});
-            //            $(this).find('select').change(function(){testlogger("self.choose('"+$(this).parent().find('label').html().trim().replace('*', '')+"', '"+$(this).find('option:selected').html()+"')")});
-            //            $(this).find('a:not(.btn):not(.nav-link):not(.menu-item):not(.menu-subitem):not(.search-menu-item)').click(function(){testlogger("self.click_link('"+$(this).text().replace("Loading...", "").trim()+"')")});
-            //            $(this).find('a.nav-link').click(function(){testlogger("self.click_tab('"+$(this).find('.nav-link-text').text().trim()+"')")});
-            //            $(this).find('a.menu-subitem').click(function(){testlogger("self.click_menu"+$(this).data("hierarchy")+"")});
-            //            $(this).find('a.search-menu-item').click(function(){testlogger("self.search_menu('"+$(this).text().trim()+"')")});
-            //            $(this).find('a.btn').click(function(){testlogger("self.click_button('"+$(this).text().trim()+"')")});
-            //            $(this).find('button').click(function(){testlogger("self.click_button('"+$(this).text().replace("Loading...", "").trim()+"')")});
-            //            $(this).find('input[type=checkbox]').click(function(){testlogger("self.check('"+($(this).parent().find('label').html()||"").trim().replace('*', '')+"')")});
-            //            $(this).find('btn i.bi').click(function(){testlogger("self.click_icon('"+$(this).attr('class').replace("bi ", "").replace("bi-", "")+"')")});
-        }
         return this;
     },
     refresh: function(areas) {
         function reloadAreas() {
             $('.reloadable-fieldset, .reloadable-queryset').map(
                 function(i, item) {
                     var querystring = '';
```

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/sw.js` & `sloth-framework-0.1.9/sloth/api/static/js/sw.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/tests.js` & `sloth-framework-0.1.9/sloth/api/static/js/tests.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,60 @@
 var cursor = document;
+var testLoggerIdent = '';
+
+function formatValue(value) {
+    if (value && value.length == 10 && value.indexOf('-') == 4) {
+        var tokens = value.split('-');
+        if (tokens.length == 3) return tokens[2] + '/' + tokens[1] + '/' + tokens[0];
+    }
+    return value;
+}
+
+function testlogger(command) {
+    if (LOG_TEST_ACTIONS) $.get('/app/dashboard/test_logger/?command=' + testLoggerIdent + command);
+}
+
+function initTestLogger(element) {
+    if (!LOG_TEST_ACTIONS) return;
+    $(element).find('.btn i.bi').click(function() {
+        testlogger("self.click_icon('" + $(this).attr('class').replace('bi ', '').replace('bi-', '') + "')")
+    });
+    $(element).find('input, textarea').not('input[type=checkbox]').blur(function() {
+        testlogger("self.enter('" + $(this).parent().find('label').html().trim().replace('*', '') + "', '" + formatValue($(this).val()) + "')")
+    });
+    $(element).find('select').change(function() {
+        testlogger("self.choose('" + $(this).parent().find('label').html().trim().replace('*', '') + "', '" + $(this).find('option:selected').html() + "')")
+    });
+    $(element).find('a:not(.btn):not(.nav-link):not(.menu-item):not(.menu-subitem):not(.search-menu-item)').click(function() {
+        testlogger("self.click_link('" + $(this).text().replace("Loading...", "").trim() + "')")
+    });
+    $(element).find('a.nav-link').click(function() {
+        testlogger("self.click_tab('" + $(this).find('.nav-link-text').text().trim() + "')")
+    });
+    $(element).find('a.menu-subitem').click(function() {
+        testlogger("self.click_menu" + $(this).data("hierarchy") + "")
+    });
+    $(element).find('a.search-menu-item').click(function() {
+        testlogger("self.search_menu('" + $(this).text().trim() + "')")
+    });
+    $(element).find('a.btn').click(function() {
+        var label = $(this).text().trim();
+        if (label) testlogger("self.click_button('" + label + "')")
+    });
+    $(element).find('button').click(function() {
+        var label = $(this).text().replace("Loading...", "").trim();
+        if (label) testlogger("self.click_button('" + label + "')")
+    });
+    $(element).find('input[type=checkbox]').click(function() {
+        testlogger("self.check('" + $(this).parent().find('label').html().trim().replace('*', '') + "')")
+    });
+    $(element).find('btn i.bi').click(function() {
+        testlogger("self.click_icon('" + $(this).attr('class').replace("bi ", "").replace("bi-", "") + "')")
+    });
+}
 
 function fakeMouse() {
     if ($("#fake-cursor").length == 0) {
         var img = $('<img id="fake-cursor">');
         img.attr('id', "fake-cursor");
         img.attr('src', "/static/images/hand.png");
         img.css('position', 'absolute');
@@ -23,30 +75,42 @@
     }
     if (index == string.length - 1) {
         var daterangepicker = el.data('daterangepicker');
         if (daterangepicker) daterangepicker.hide();
     }
 }
 
+function showFakeMouse(force) {
+    var top = $(document).getCookie('mouse-top') || 0;
+    var left = $(document).getCookie('mouse-left') || 0;
+    if ($('#fake-cursor').length == 0) $('body').append(
+        '<img id="fake-cursor" style="display:none;position:absolute;z-index:9999999;top:' + top + ';left:' + left + '"/>'
+    );
+    $("#fake-cursor").css('top', top);
+    $("#fake-cursor").css('left', left);
+    if (force || top || left) $("#fake-cursor").attr("src", "/static/images/hand.png").show();
+}
 
 function moveMouseTo(lookup, f) {
-    $("#fake-cursor").attr("src", "/static/images/hand.png").show();
     var el = $(lookup).first();
     var top = el.first().offset()['top'] + el.height() / 2;
     var left = el.first().offset()['left'] + el.width() / 2;
     var lastClickedElement = null;
-    window['mouse-top'] = top;
-    window['mouse-left'] = left;
+    $(document).setCookie('mouse-top', top);
+    $(document).setCookie('mouse-left', left);
     $('#fake-cursor').animate({
         top: top,
         left: left
     }, 1200, 'swing', function() {
         if (lastClickedElement != el) {
             $("#fake-cursor").attr("src", "/static/images/click.png");
             setTimeout(f, 500);
+            setTimeout(function() {
+                $("#fake-cursor").attr("src", "/static/images/hand.png")
+            }, 500);
         }
         lastClickedElement = el;
     });
 }
 
 function recursively(element) {
     if (element.length == 0 && (cursor || document) != document) {
@@ -69,15 +133,15 @@
 
 function scroolToElement(element, callback) {
     var lastScrooledElement = null;
     if (element.offset() && !isIntoView(element)) {
         var scrollData = {
             scrollTop: element.offset().top - $(window).height() / 2
         };
-        if (window['display_fake_mouse']) var scroolSpeed = 1200;
+        if (window['DISPLAY_FAKE_MOUSE']) var scroolSpeed = 1200;
         else var scroolSpeed = 0;
         // $([document.documentElement, document.body]).animate(scrollData, scroolSpeed, 'swing', function (){
         if ($('#modal:visible').length > 0) {
             var container = '#modal';
             var scrollData = {
                 scrollTop: element.offset().top - (window.innerHeight * 0.25) + $(container).scrollTop()
             };
@@ -137,15 +201,17 @@
         }).first();
         if (element.length == 0 && (link || button)) element = $(cursor || document).find("a[name='" + name + "']").first();
     }
 
     if (recursively(element)) {
         return click(name, type);
     } else if (element.length > 0) {
-        if (window['display_fake_mouse']) {
+        if (window['DISPLAY_FAKE_MOUSE']) {
+            showFakeMouse(true);
+
             function afterScrool() {
                 function afterMoveMouse() {
                     $(element[index]).trigger('mouseover');
                     element[index].click();
                 }
                 moveMouseTo(element[index], afterMoveMouse);
             }
@@ -250,15 +316,15 @@
         }
 
         if (recursively(element)) {
             return enter(name, value, submit);
         } else if (element.length > 0) {
             function afterScrool() {
                 element.focus();
-                if (window['display_fake_mouse']) {
+                if (window['DISPLAY_FAKE_MOUSE'] && name != 'search') {
                     fakeType(element, value, 0);
                 } else {
                     element.val(value);
                     var daterangepicker = element.data('daterangepicker');
                     if (daterangepicker) {
                         setTimeout(function() {
                             daterangepicker.hide()
@@ -352,8 +418,12 @@
 
 function wait(ms) {
     var start = new Date().getTime();
     var end = start;
     while (end < start + ms) {
         end = new Date().getTime();
     }
-}
+}
+
+$(document).ready(function() {
+    if (DISPLAY_FAKE_MOUSE) showFakeMouse();
+});
```

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/trumbowyg.min.js` & `sloth-framework-0.1.9/sloth/api/static/js/trumbowyg.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/static/js/wpn.js` & `sloth-framework-0.1.9/sloth/api/static/js/wpn.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/tasks/__init__.py` & `sloth-framework-0.1.9/sloth/api/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/actions/execute_query.html` & `sloth-framework-0.1.9/sloth/api/templates/actions/execute_query.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/actions/show_icons.html` & `sloth-framework-0.1.9/sloth/api/templates/actions/show_icons.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/actions/workflow.html` & `sloth-framework-0.1.9/sloth/api/templates/actions/workflow.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/api/index.html` & `sloth-framework-0.1.9/sloth/api/templates/api/index.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/charts/bar.html` & `sloth-framework-0.1.9/sloth/api/templates/charts/bar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/charts/column.html` & `sloth-framework-0.1.9/sloth/api/templates/charts/column.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/charts/pie.html` & `sloth-framework-0.1.9/sloth/api/templates/charts/pie.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/actions.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/actions.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/apps.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/apps.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/base.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/base.html`

 * *Files 13% similar despite different names*

```diff
@@ -48,15 +48,18 @@
     <script src="/static/js/jquery.binarytransport.js"></script>
     <script src="/static/js/jquery.mask.min.js"></script>
     <script src="/static/js/trumbowyg.min.js"></script>
     {% for url in dashboard.data.scripts %}
       <script src="{{ url }}?version={{ dashboard.data.footer.version }}"></script>
     {% endfor %}
     {% block extrahead %} {% endblock %}
-
+    <script>
+      var DISPLAY_FAKE_MOUSE = {{ DISPLAY_FAKE_MOUSE }};
+      var LOG_TEST_ACTIONS = {{ LOG_TEST_ACTIONS }};
+    </script>
   </head>
   <body id="{{ request.path|url_slug }}">
     {% include "dashboard/menu.html" with menu=dashboard.data.menu %}
     {% block header %}{% include "dashboard/header.html" %}{% endblock %}
     {% include "dashboard/links.html" with data=dashboard.data %}
 
       <main>
@@ -70,13 +73,9 @@
       </main>
     {% block footer %}
     {% include "dashboard/footer.html" %}
     {% endblock %}
     {% include "dashboard/modal.html" %}
     {% include "dashboard/bottom.html" %}
   </body>
-  <script>
-    var display_fake_mouse = false;
-    function testlogger(command){return;$.get('/app/dashboard/test_logger/?command='+command);};
-  </script>
 </html>
 {% endif %}
```

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/bottom.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/bottom.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/cards.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/footer.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/footer.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/form.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/form.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/grids.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/grids.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/header.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/header.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/links.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/links.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/menu.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/menu.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/messages.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/messages.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/modal.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/modal.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/plus.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/plus.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/report.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/report.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/search.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/search.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/selector.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/selector.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/settings.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/settings.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/shortcuts.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/shortcuts.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/tasks.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/tasks.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/dashboard/tools.html` & `sloth-framework-0.1.9/sloth/api/templates/dashboard/tools.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/inputs/picker.html` & `sloth-framework-0.1.9/sloth/api/templates/inputs/picker.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/inputs/qrcode.html` & `sloth-framework-0.1.9/sloth/api/templates/inputs/qrcode.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/inputs/select.html` & `sloth-framework-0.1.9/sloth/api/templates/inputs/select.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/queryset/accordion.html` & `sloth-framework-0.1.9/sloth/api/templates/queryset/accordion.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/queryset/calendar.html` & `sloth-framework-0.1.9/sloth/api/templates/queryset/calendar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/queryset/cards.html` & `sloth-framework-0.1.9/sloth/api/templates/queryset/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/queryset/datatable.html` & `sloth-framework-0.1.9/sloth/api/templates/queryset/datatable.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/queryset/filter.html` & `sloth-framework-0.1.9/sloth/api/templates/queryset/filter.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/queryset/filters.html` & `sloth-framework-0.1.9/sloth/api/templates/queryset/filters.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/queryset/queryset.html` & `sloth-framework-0.1.9/sloth/api/templates/queryset/queryset.html`

 * *Files 2% similar despite different names*

```diff
@@ -120,16 +120,18 @@
                         $(this).addClass('text-primary');
                         treeNode{{ data.uuid }}(this.id);
 
                     });
                 }
                 initializeNode{{ data.uuid }}($('#queryset-{{ data.uuid }}'));
                 $('#queryset-global-actions-{{ data.uuid }}').find('a').click(function(){
-                    var params = $('#form-{{ data.uuid }}').serialize();
-                    this.href = this.href.split('?')[0] + '?' + params + '&global_action=1';
+                    if(!this.href.indexOf('#')>0){
+                        var params = $('#form-{{ data.uuid }}').serialize();
+                        this.href = this.href.split('?')[0] + '?' + params + '&global_action=1';
+                    }
                 });
             </script>
         {% endif %}
 
         <div class="queryset-data" id="queryset-data-{{ data.uuid }}">
 
     {% if data.metadata.pagination.total or data.metadata.calendar %}
@@ -195,14 +197,17 @@
             </li>
           {% if forloop.counter == 4 %}
             <li class="page-item disabled">
               <a class="page-link" href="#" tabindex="-1" aria-disabled="true">...</a>
             </li>
           {% endif %}
         {% endfor %}
+        {% if data.metadata.pagination.pages|length > 4 %}
+        <li>&nbsp;&nbsp;&nbsp;Ir para página <input type="number" style="border:1px solid #dee2e6;height:38;width:48;padding-left:8;" value="{{ data.metadata.pagination.page }}" onkeypress="if(event.which==13){$('#pagination-{{ data.uuid }}').val(this.value);reload{{ data.uuid }}();document.getElementById('pagination-info-{{ data.uuid }}').scrollIntoView();return false;}"></li>
+        {% endif %}
       </ul>
     </nav>
     {% endif %}
         </div>
         </div>
     </div>
     {% if data.metadata.scrollable %}
```

### Comparing `sloth-framework-0.1.8/sloth/api/templates/queryset/rows.html` & `sloth-framework-0.1.9/sloth/api/templates/queryset/rows.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/queryset/scroll.html` & `sloth-framework-0.1.9/sloth/api/templates/queryset/scroll.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/queryset/statistics.html` & `sloth-framework-0.1.9/sloth/api/templates/queryset/statistics.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/queryset/timeline.html` & `sloth-framework-0.1.9/sloth/api/templates/queryset/timeline.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/queryset/tree.html` & `sloth-framework-0.1.9/sloth/api/templates/queryset/tree.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/renderers/calendar/calendar.html` & `sloth-framework-0.1.9/sloth/api/templates/renderers/calendar/calendar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/renderers/maps/map.html` & `sloth-framework-0.1.9/sloth/api/templates/renderers/maps/map.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/renderers/programing/strtable.html` & `sloth-framework-0.1.9/sloth/api/templates/renderers/programing/strtable.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/renderers/statistics/cards.html` & `sloth-framework-0.1.9/sloth/api/templates/renderers/statistics/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/renderers/steps/check.html` & `sloth-framework-0.1.9/sloth/api/templates/renderers/steps/check.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/renderers/utils/steps.html` & `sloth-framework-0.1.9/sloth/api/templates/renderers/utils/steps.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/renderers/utils/table.html` & `sloth-framework-0.1.9/sloth/api/templates/renderers/utils/table.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/themes/dark.html` & `sloth-framework-0.1.9/sloth/api/templates/themes/dark.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/valueset/fieldset-group.html` & `sloth-framework-0.1.9/sloth/api/templates/valueset/fieldset-group.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/valueset/fieldset-list.html` & `sloth-framework-0.1.9/sloth/api/templates/valueset/fieldset-list.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/valueset/fieldset.html` & `sloth-framework-0.1.9/sloth/api/templates/valueset/fieldset.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/valueset/value.html` & `sloth-framework-0.1.9/sloth/api/templates/valueset/value.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templates/valueset/valueset.html` & `sloth-framework-0.1.9/sloth/api/templates/valueset/valueset.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/templatetags/tags.py` & `sloth-framework-0.1.9/sloth/api/templatetags/tags.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/urls.py` & `sloth-framework-0.1.9/sloth/api/urls.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/api/views.py` & `sloth-framework-0.1.9/sloth/api/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from sloth import threadlocals
 from django.core.cache import cache
 from django.http import QueryDict
 from django.apps import apps
 from oauth2_provider.oauth2_backends import get_oauthlib_core
 from ..core.valueset import ValueSet
+from ..test import SeleniumTestCase
 from ..utils.http import ApiResponse
 from django.contrib.auth import authenticate
 from ..api import OpenApi
 from django.conf import settings
 from django.contrib import messages
 from django.core.exceptions import PermissionDenied
 from django.http import JsonResponse, HttpResponseForbidden, HttpResponse, HttpResponseRedirect
@@ -54,14 +55,16 @@
     if request.user.is_authenticated and settings.FORCE_PASSWORD_DEFINITION:
         default_password = settings.DEFAULT_PASSWORD(request.user)
         if request.user.check_password(default_password):
             messages.warning(request, 'Altere sua senha padrão')
             return HttpResponseRedirect('/app/dashboard/change_password/')
     try:
         ctx = dict(dashboard=Dashboards(request))
+        ctx['DISPLAY_FAKE_MOUSE'] = 1 if SeleniumTestCase.EXPLAIN else 0
+        ctx['LOG_TEST_ACTIONS'] = 1 if SeleniumTestCase.LOG_ACTION == 2 else 0
         if request.user.is_authenticated and request.path.startswith('/app/') and not is_ajax(request):
             if 'stack' not in request.session:
                 request.session['stack'] = []
             if request.path == '/app/dashboard/':
                 request.session['stack'].clear()
                 request.session['stack'].append(request.path)
             elif request.path in request.session['stack']:
```

### Comparing `sloth-framework-0.1.8/sloth/cloud/printer.py` & `sloth-framework-0.1.9/sloth/cloud/printer.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/cloud/server.py` & `sloth-framework-0.1.9/sloth/cloud/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     def _get_compose_file_path(self):
         return os.path.join(WORKDIR, self._get_project_name(), 'docker-compose.yml')
 
     def _get_nginx_project_conf(self):
         ssl = 'listen 80; listen 443 ssl; ssl_certificate %s; ssl_certificate_key %s; if ($scheme = http) {return 301 https://$server_name$request_uri;}' % CERTIFICATE if CERTIFICATE else ''
         static = 'location /static { alias %s; }' % os.path.join(self._get_project_dir(), 'static')
-        media = 'location /media { alias %s; }' % os.path.join(self._get_project_dir(), 'media')
+        media = 'location /media { alias %s; }' % os.path.join(self._get_project_dir(), '.docker', 'media')
         return 'server {server_name %s.%s; location / { proxy_pass http://127.0.0.1:%s; } %s %s %s }' % (
             self._get_project_name(), DOMAIN_NAME, self._get_container_port(), ssl, static, media
         )
 
     def get_project_deploy_url(self):
         return 'http://{}.{}/'.format(self._get_project_name(), DOMAIN_NAME)
```

### Comparing `sloth-framework-0.1.8/sloth/conf/settings.py` & `sloth-framework-0.1.9/sloth/conf/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -79,8 +79,11 @@
     DATABASES['default']['NAME'] = os.environ.get('DATABASE_NAME', 'database')
     DATABASES['default']['USER'] = os.environ.get('DATABASE_USER', 'postgres')
     DATABASES['default']['PASSWORD'] = os.environ.get('DATABASE_PASSWORD', 'password')
     DATABASES['default']['HOST'] = os.environ.get('DATABASE_HOST', 'postgres')
     DATABASES['default']['PORT'] = os.environ.get('DATABASE_PORT', '5432')
 
 
-from .local_settings import *
+try:
+    from .local_settings import *
+except ImportError as e:
+    print('[WARNING] Could not import local_settings.py: {}'.format(e))
```

### Comparing `sloth-framework-0.1.8/sloth/core/base.py` & `sloth-framework-0.1.9/sloth/core/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,18 +171,19 @@
                         scope_type.metaclass().app_label, scope_type.metaclass().model_name
                     ) if scope_type else None,
                     scope_key=scope_key, scope_value=scope_value
                 )
         deleted_role_tuples = role_tuples - role_tuples2
         # print('DELETED: ', deleted_role_tuples)
         for username, email, scope_name, scope_type, scope_key, scope_value in deleted_role_tuples:
-            scope_type = '{}.{}'.format(scope_type.metaclass().app_label, scope_type.metaclass().model_name)
-            role.objects.filter(
-                user__username=username, name=scope_name, scope_type=scope_type, scope_key=scope_key, scope_value=scope_value
-            ).delete()
+            if scope_type:
+                scope_type = '{}.{}'.format(scope_type.metaclass().app_label, scope_type.metaclass().model_name)
+                role.objects.filter(
+                    user__username=username, name=scope_name, scope_type=scope_type, scope_key=scope_key, scope_value=scope_value
+                ).delete()
 
     @classmethod
     def get_list_url(cls, prefix='', subset='all'):
         url = '{}/{}/{}/'.format(prefix, cls.metaclass().app_label, cls.metaclass().model_name)
         if subset != 'all':
             url = '{}{}/'.format(url, subset)
         return url
```

### Comparing `sloth-framework-0.1.8/sloth/core/queryset.py` & `sloth-framework-0.1.9/sloth/core/queryset.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/core/statistics.py` & `sloth-framework-0.1.9/sloth/core/statistics.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/core/validation.py` & `sloth-framework-0.1.9/sloth/core/validation.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/core/valueset.py` & `sloth-framework-0.1.9/sloth/core/valueset.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/db/models/__init__.py` & `sloth-framework-0.1.9/sloth/db/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,28 @@
     def formfield(self, **kwargs):
         from sloth.actions.inputs import ColorInput
         field = super().formfield(**kwargs)
         field.widget = ColorInput()
         return field
 
 
+class PhotoField(ImageField):
+    def __init__(self, *args, max_width=200, max_height=200, **kwargs):
+        self.max_width = max_width
+        self.max_height = max_height
+        super().__init__(*args, **kwargs)
+
+    def formfield(self, **kwargs):
+        field = super().formfield(**kwargs)
+        field.widget.attrs.update(
+            {'data-max-width': self.max_width, 'data-max-height': self.max_height, 'accept': 'image/*', 'capture': ''}
+        )
+        return field
+
+
 class CharField(CharField):
     def __init__(self, *args, max_length=255, **kwargs):
         self.mask = kwargs.pop('mask', None)
         self.rmask = kwargs.pop('rmask', None)
         super().__init__(*args, max_length=max_length, **kwargs)
 
     def formfield(self, **kwargs):
```

### Comparing `sloth-framework-0.1.8/sloth/test/__init__.py` & `sloth-framework-0.1.9/sloth/test/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/test/selenium/browser.py` & `sloth-framework-0.1.9/sloth/test/selenium/browser.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,20 +7,18 @@
 from selenium import webdriver
 from django.conf import settings
 from selenium.webdriver.common.by import By
 from selenium.webdriver.firefox.options import Options
 from selenium.common.exceptions import WebDriverException
 
 
-HEADLESS = os.environ.get('HEADLESS') in (None, '1')
-
 
 class Browser(webdriver.Firefox):
-    def __init__(self, server_url, options=None, verbose=True, slowly=False, maximize=True, headless=HEADLESS):
-
+    
+    def __init__(self, server_url, options=None, verbose=True, slowly=False, maximize=True, headless=True):
         if not options:
             options = Options()
         if maximize:
             options.add_argument("--start-maximized")
         else:
             options.add_argument("--window-size=720x800")
         if headless and '-v' not in sys.argv:
@@ -36,20 +34,14 @@
         if maximize:
             self.maximize_window()
         else:
             self.set_window_position(700, 0)
             self.set_window_size(720, 800)
         self.switch_to.window(self.current_window_handle)
 
-    def slow_down(self):
-        self.slowly = True
-
-    def speed_up(self):
-        self.slowly = False
-
     def wait(self, seconds=1):
         time.sleep(seconds)
 
     def watch(self, e):
         self.save_screenshot('/tmp/test.png')
         raise e
 
@@ -59,27 +51,29 @@
 
     def execute_script(self, script, *args):
         super().execute_script(script, *args)
         if self.slowly:
             self.wait(3)
 
     def open(self, url):
-        self.get("{}{}".format(self.server_url, url))
+        if url.startswith('http'):
+            self.get(url.replace('http://localhost:8000', self.server_url))
+        else:
+            self.get("{}{}".format(self.server_url, url))
 
     def pdb(self):
         breakpoint()
 
     def back(self, seconds=None):
         if seconds:
             self.wait(seconds)
         if not self.current_url or not self.current_url.endswith('/app/'):
             self.open('/app/')
 
     def enter(self, name, value, submit=False, count=4):
-
         if callable(value):
             value = value()
         if type(value) == datetime.date:
             value = value.strftime('%d/%m/%Y')
         if value:
             self.print('{} "{}" for "{}"'.format('Entering', value, name))
         try:
@@ -149,15 +143,15 @@
                     self.see(text, flag, count - 1)
                 else:
                     self.watch(e)
             if self.slowly:
                 self.wait(2)
 
     def see_message(self, text, count=4):
-        self.print('See message {}'.format(text))
+        self.print('See message "{}"'.format(text))
         try:
             self.execute_script("seeMessage('{}')".format(text))
         except WebDriverException as e:
             if count:
                 self.wait()
                 self.see_message(text, count - 1)
             else:
@@ -230,25 +224,24 @@
             if count:
                 self.wait()
                 self.check_radio(text=text, count=count - 1)
             else:
                 self.watch(e)
         self.wait()
 
-    def search_menu(self, *texts, count=4):
-        self.print('Searching "{}"'.format('->'.join(texts)))
-        for text in texts:
-            try:
-                self.execute_script("searchMenu('{}')".format(text.strip()))
-            except WebDriverException as e:
-                if count:
-                    self.wait()
-                    self.search_menu(*texts, count=count - 1)
-                else:
-                    self.watch(e)
+    def search_menu(self, text, count=4):
+        self.print('Searching "{}"'.format(text))
+        try:
+            self.execute_script("searchMenu('{}')".format(text.strip()))
+        except WebDriverException as e:
+            if count:
+                self.wait()
+                self.search_menu(text, count=count - 1)
+            else:
+                self.watch(e)
         self.wait()
 
     def click_menu(self, *texts, count=1):
         self.print('Clicking menu "{}"'.format('->'.join(texts)))
         for i, text in enumerate(texts):
             if i==0:
                 self.click_icon('list')
```

### Comparing `sloth-framework-0.1.8/sloth/utils/__init__.py` & `sloth-framework-0.1.9/sloth/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/utils/formatter/__init__.py` & `sloth-framework-0.1.9/sloth/utils/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/utils/http/__init__.py` & `sloth-framework-0.1.9/sloth/utils/http/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/utils/icons/bootstrap.py` & `sloth-framework-0.1.9/sloth/utils/icons/bootstrap.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/utils/icons/fontawesome.py` & `sloth-framework-0.1.9/sloth/utils/icons/fontawesome.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/utils/icons/materialicons.py` & `sloth-framework-0.1.9/sloth/utils/icons/materialicons.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth/utils/log/sql.py` & `sloth-framework-0.1.9/sloth/utils/log/sql.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.8/sloth_framework.egg-info/PKG-INFO` & `sloth-framework-0.1.9/sloth_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sloth-framework
-Version: 0.1.8
+Version: 0.1.9
 Summary: Metadata-based web framework for the development of management information systems
 Home-page: http://sloth.aplicativo.click/
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `sloth-framework-0.1.8/sloth_framework.egg-info/SOURCES.txt` & `sloth-framework-0.1.9/sloth_framework.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 sloth/api/management/commands/query.py
 sloth/api/management/commands/reset_passwords.py
 sloth/api/management/commands/selenium.py
 sloth/api/management/commands/send_web_push_notification.py
 sloth/api/management/commands/startserver.py
 sloth/api/management/commands/sync.py
 sloth/api/management/commands/sync_roles.py
+sloth/api/management/commands/test.py
 sloth/api/migrations/0001_initial.py
 sloth/api/migrations/0002_role_user.py
 sloth/api/migrations/0003_alter_application_user.py
 sloth/api/migrations/0004_task.py
 sloth/api/migrations/0005_task_stopped_alter_task_message.py
 sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
 sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
```

