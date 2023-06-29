# Comparing `tmp/Flask-BigApp-2023.1.9.5.tar.gz` & `tmp/Flask-BigApp-2023.1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-BigApp-2023.1.9.5.tar", last modified: Thu Jun 29 07:31:25 2023, max compression
+gzip compressed data, was "Flask-BigApp-2023.1.9.6.tar", last modified: Thu Jun 29 08:02:27 2023, max compression
```

## Comparing `Flask-BigApp-2023.1.9.5.tar` & `Flask-BigApp-2023.1.9.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.751425 Flask-BigApp-2023.1.9.5/
--rw-rw-r--   0 david     (1000) david     (1000)    25342 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)       60 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-06-29 07:31:25.751425 Flask-BigApp-2023.1.9.5/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      699 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/README.md
--rw-rw-r--   0 david     (1000) david     (1000)      271 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)      174 2023-06-29 07:31:25.751425 Flask-BigApp-2023.1.9.5/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     1582 2023-06-29 07:23:55.000000 Flask-BigApp-2023.1.9.5/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.743425 Flask-BigApp-2023.1.9.5/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.747425 Flask-BigApp-2023.1.9.5/src/Flask_BigApp.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-06-29 07:31:25.000000 Flask-BigApp-2023.1.9.5/src/Flask_BigApp.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1855 2023-06-29 07:31:25.000000 Flask-BigApp-2023.1.9.5/src/Flask_BigApp.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-29 07:31:25.000000 Flask-BigApp-2023.1.9.5/src/Flask_BigApp.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       54 2023-06-29 07:31:25.000000 Flask-BigApp-2023.1.9.5/src/Flask_BigApp.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-15 10:09:07.000000 Flask-BigApp-2023.1.9.5/src/Flask_BigApp.egg-info/not-zip-safe
--rw-rw-r--   0 david     (1000) david     (1000)      101 2023-06-29 07:31:25.000000 Flask-BigApp-2023.1.9.5/src/Flask_BigApp.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       30 2023-06-29 07:31:25.000000 Flask-BigApp-2023.1.9.5/src/Flask_BigApp.egg-info/top_level.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.747425 Flask-BigApp-2023.1.9.5/src/flask_bigapp/
--rw-rw-r--   0 david     (1000) david     (1000)      305 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    10522 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp/auth.py
--rw-rw-r--   0 david     (1000) david     (1000)    11409 2023-06-29 07:26:28.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp/bigapp.py
--rw-rw-r--   0 david     (1000) david     (1000)     6229 2023-06-29 07:12:39.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp/blueprint.py
--rw-rw-r--   0 david     (1000) david     (1000)     4881 2023-06-29 07:27:24.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp/helpers.py
--rw-rw-r--   0 david     (1000) david     (1000)     5845 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp/orm.py
--rw-rw-r--   0 david     (1000) david     (1000)      788 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp/registeries.py
--rw-rw-r--   0 david     (1000) david     (1000)     1659 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp/resources.py
--rw-rw-r--   0 david     (1000) david     (1000)     7663 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp/security.py
--rw-rw-r--   0 david     (1000) david     (1000)     3352 2023-06-29 07:28:26.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp/utilities.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.747425 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/
--rw-rw-r--   0 david     (1000) david     (1000)       46 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.743425 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.747425 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/builtins/
--rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/builtins/context_processors.py
--rw-rw-r--   0 david     (1000) david     (1000)      915 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.743425 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/static/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.747425 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/static/css/
--rw-rw-r--   0 david     (1000) david     (1000)       45 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/static/css/example__css.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.747425 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/static/img/
--rw-rw-r--   0 david     (1000) david     (1000)    28469 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.747425 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/static/js/
--rw-rw-r--   0 david     (1000) david     (1000)      119 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/static/js/example__js.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.743425 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.743425 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.747425 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/
--rw-rw-r--   0 david     (1000) david     (1000)      268 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/400.html
--rw-rw-r--   0 david     (1000) david     (1000)      315 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/401.html
--rw-rw-r--   0 david     (1000) david     (1000)      261 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/403.html
--rw-rw-r--   0 david     (1000) david     (1000)      281 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/404.html
--rw-rw-r--   0 david     (1000) david     (1000)      302 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/405.html
--rw-rw-r--   0 david     (1000) david     (1000)      278 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/500.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.747425 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/
--rw-rw-r--   0 david     (1000) david     (1000)      766 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.751425 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/
--rw-rw-r--   0 david     (1000) david     (1000)       13 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/footer.html
--rw-rw-r--   0 david     (1000) david     (1000)       11 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/menu.html
--rw-rw-r--   0 david     (1000) david     (1000)     9883 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/cli.py
--rw-rw-r--   0 david     (1000) david     (1000)      992 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/resources.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:31:25.751425 Flask-BigApp-2023.1.9.5/tests/
--rw-rw-r--   0 david     (1000) david     (1000)     2537 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.5/tests/test_group.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.954105 Flask-BigApp-2023.1.9.6/
+-rw-rw-r--   0 david     (1000) david     (1000)    25342 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)       60 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-06-29 08:02:27.954105 Flask-BigApp-2023.1.9.6/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      699 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)      271 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)      174 2023-06-29 08:02:27.954105 Flask-BigApp-2023.1.9.6/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     1582 2023-06-29 08:02:23.000000 Flask-BigApp-2023.1.9.6/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.942104 Flask-BigApp-2023.1.9.6/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.946104 Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-06-29 08:02:27.000000 Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     1855 2023-06-29 08:02:27.000000 Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-29 08:02:27.000000 Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       54 2023-06-29 08:02:27.000000 Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-15 10:09:07.000000 Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/not-zip-safe
+-rw-rw-r--   0 david     (1000) david     (1000)      101 2023-06-29 08:02:27.000000 Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       30 2023-06-29 08:02:27.000000 Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.950105 Flask-BigApp-2023.1.9.6/src/flask_bigapp/
+-rw-rw-r--   0 david     (1000) david     (1000)      305 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10522 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/auth.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11409 2023-06-29 07:26:28.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/bigapp.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6229 2023-06-29 07:12:39.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/blueprint.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5172 2023-06-29 07:59:44.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/helpers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5845 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/orm.py
+-rw-rw-r--   0 david     (1000) david     (1000)      788 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/registeries.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1659 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/resources.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7663 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/security.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3630 2023-06-29 07:52:15.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp/utilities.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.950105 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/
+-rw-rw-r--   0 david     (1000) david     (1000)       46 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.942104 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.950105 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/builtins/
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/builtins/context_processors.py
+-rw-rw-r--   0 david     (1000) david     (1000)      915 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.942104 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/static/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.950105 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/static/css/
+-rw-rw-r--   0 david     (1000) david     (1000)       45 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/static/css/example__css.css
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.950105 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/static/img/
+-rw-rw-r--   0 david     (1000) david     (1000)    28469 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.950105 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/static/js/
+-rw-rw-r--   0 david     (1000) david     (1000)      119 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/static/js/example__js.js
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.946104 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.946104 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.954105 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/
+-rw-rw-r--   0 david     (1000) david     (1000)      268 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/400.html
+-rw-rw-r--   0 david     (1000) david     (1000)      315 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/401.html
+-rw-rw-r--   0 david     (1000) david     (1000)      261 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/403.html
+-rw-rw-r--   0 david     (1000) david     (1000)      281 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/404.html
+-rw-rw-r--   0 david     (1000) david     (1000)      302 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/405.html
+-rw-rw-r--   0 david     (1000) david     (1000)      278 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/500.html
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.954105 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/
+-rw-rw-r--   0 david     (1000) david     (1000)      766 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.954105 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/
+-rw-rw-r--   0 david     (1000) david     (1000)       13 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/footer.html
+-rw-rw-r--   0 david     (1000) david     (1000)       11 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/menu.html
+-rw-rw-r--   0 david     (1000) david     (1000)     9883 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/cli.py
+-rw-rw-r--   0 david     (1000) david     (1000)      992 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/resources.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 08:02:27.954105 Flask-BigApp-2023.1.9.6/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)     2537 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.6/tests/test_group.py
```

### Comparing `Flask-BigApp-2023.1.9.5/LICENSE` & `Flask-BigApp-2023.1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.5/PKG-INFO` & `Flask-BigApp-2023.1.9.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-BigApp
-Version: 2023.1.9.5
+Version: 2023.1.9.6
 Summary: A Flask auto importer that allows your Flask apps to grow big.
 Home-page: https://github.com/Flask-Planet/Flask-BigApp
 Author: David Carmichael
 Author-email: carmichaelits@gmail.com
 License: GNU Lesser General Public License v2.1
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Flask-BigApp-2023.1.9.5/README.md` & `Flask-BigApp-2023.1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.5/setup.py` & `Flask-BigApp-2023.1.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from setuptools import setup, find_packages
 
 readme = pathlib.Path(pathlib.Path.cwd() / "README.md").read_text()
 
 setup(
     name='Flask-BigApp',
-    version=f'2023.1.9.5',
+    version=f'2023.1.9.6',
     url='https://github.com/Flask-Planet/Flask-BigApp',
     license='GNU Lesser General Public License v2.1',
     author='David Carmichael',
     author_email='carmichaelits@gmail.com',
     description='A Flask auto importer that allows your Flask apps to grow big.',
     long_description=f'{readme}',
     long_description_content_type='text/markdown',
```

### Comparing `Flask-BigApp-2023.1.9.5/src/Flask_BigApp.egg-info/PKG-INFO` & `Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-BigApp
-Version: 2023.1.9.5
+Version: 2023.1.9.6
 Summary: A Flask auto importer that allows your Flask apps to grow big.
 Home-page: https://github.com/Flask-Planet/Flask-BigApp
 Author: David Carmichael
 Author-email: carmichaelits@gmail.com
 License: GNU Lesser General Public License v2.1
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Flask-BigApp-2023.1.9.5/src/Flask_BigApp.egg-info/SOURCES.txt` & `Flask-BigApp-2023.1.9.6/src/Flask_BigApp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.5/src/flask_bigapp/auth.py` & `Flask-BigApp-2023.1.9.6/src/flask_bigapp/auth.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.5/src/flask_bigapp/bigapp.py` & `Flask-BigApp-2023.1.9.6/src/flask_bigapp/bigapp.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.5/src/flask_bigapp/blueprint.py` & `Flask-BigApp-2023.1.9.6/src/flask_bigapp/blueprint.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.5/src/flask_bigapp/helpers.py` & `Flask-BigApp-2023.1.9.6/src/flask_bigapp/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,23 +60,32 @@
         )
 
     config_suffix = ('.toml', '.tml')
 
     if config_file_path.suffix not in config_suffix:
         raise TypeError("Config from_file must be one of the following types: .toml / .tml")
 
-    config = process_dict(
-        toml_load(config_file_path),
+    config = process_dict(toml_load(config_file_path))
+
+    flask_config = process_dict(
+        config.get("FLASK"),
         key_case_switch="upper",
         ignore_missing_env_variables=ignore_missing_env_variables
     )
-
-    flask_config = config.get("FLASK")
-    session_config = config.get("SESSION")
-    database_config = config.get("DATABASE")
+    session_config = process_dict(
+        config.get("SESSION"),
+        key_case_switch="ignore",
+        ignore_missing_env_variables=ignore_missing_env_variables
+    )
+    database_config = process_dict(
+        config.get("DATABASE"),
+        key_case_switch="upper",
+        ignore_missing_env_variables=ignore_missing_env_variables,
+        crawl=True
+    )
 
     if flask_config is not None and isinstance(flask_config, dict):
         for flask_config_key, flask_config_value in flask_config.items():
             app.config.update({flask_config_key: flask_config_value})
 
     if database_config is not None and isinstance(database_config, dict):
         app.config['SQLALCHEMY_BINDS'] = dict()
```

### Comparing `Flask-BigApp-2023.1.9.5/src/flask_bigapp/orm.py` & `Flask-BigApp-2023.1.9.6/src/flask_bigapp/orm.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.5/src/flask_bigapp/registeries.py` & `Flask-BigApp-2023.1.9.6/src/flask_bigapp/registeries.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.5/src/flask_bigapp/resources.py` & `Flask-BigApp-2023.1.9.6/src/flask_bigapp/resources.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.5/src/flask_bigapp/security.py` & `Flask-BigApp-2023.1.9.6/src/flask_bigapp/security.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.5/src/flask_bigapp/utilities.py` & `Flask-BigApp-2023.1.9.6/src/flask_bigapp/utilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,25 +48,36 @@
             return os.environ.get(env_var, f"{env_value} not found in environment variables")
     return env_value
 
 
 def process_dict(
         this_dict: t.Optional[dict],
         key_case_switch: str = "upper",
-        ignore_missing_env_variables: bool = False
+        ignore_missing_env_variables: bool = False,
+        crawl: bool = False
 ) -> dict:
     if this_dict is None:
         return {}
 
     return_dict = {}
     for key, value in this_dict.items():
-        cs_key = key.upper() if key_case_switch == "upper" else key.lower()
-        if isinstance(value, dict):
-            return_dict[cs_key] = process_dict(value, key_case_switch)
-            continue
+        if key_case_switch == "ignore":
+            cs_key = key
+        else:
+            cs_key = key.upper() if key_case_switch == "upper" else key.lower()
+
+        if crawl:
+            if isinstance(value, dict):
+                return_dict[cs_key] = process_dict(
+                    value,
+                    key_case_switch,
+                    ignore_missing_env_variables,
+                    crawl
+                )
+                continue
 
         return_dict[cs_key] = if_env_replace(value)
 
     return return_dict
 
 
 def cast_to_import_str(app_name: str, folder_path: Path) -> str:
```

### Comparing `Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py` & `Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png` & `Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html` & `Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/cli.py` & `Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/cli.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.5/src/flask_bigapp_cli/resources.py` & `Flask-BigApp-2023.1.9.6/src/flask_bigapp_cli/resources.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.5/tests/test_group.py` & `Flask-BigApp-2023.1.9.6/tests/test_group.py`

 * *Files identical despite different names*

