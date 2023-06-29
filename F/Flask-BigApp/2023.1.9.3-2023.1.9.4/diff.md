# Comparing `tmp/Flask-BigApp-2023.1.9.3.tar.gz` & `tmp/Flask-BigApp-2023.1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-BigApp-2023.1.9.3.tar", last modified: Sat Jun 10 15:06:04 2023, max compression
+gzip compressed data, was "Flask-BigApp-2023.1.9.4.tar", last modified: Thu Jun 29 07:18:10 2023, max compression
```

## Comparing `Flask-BigApp-2023.1.9.3.tar` & `Flask-BigApp-2023.1.9.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/
--rw-rw-r--   0 david     (1000) david     (1000)    25342 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)       60 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      699 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/README.md
--rw-rw-r--   0 david     (1000) david     (1000)      271 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)      174 2023-06-10 15:06:04.925279 Flask-BigApp-2023.1.9.3/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     1582 2023-06-10 14:58:31.000000 Flask-BigApp-2023.1.9.3/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-06-10 15:06:04.000000 Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1855 2023-06-10 15:06:04.000000 Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-10 15:06:04.000000 Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       54 2023-06-10 15:06:04.000000 Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-10 14:53:19.000000 Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/not-zip-safe
--rw-rw-r--   0 david     (1000) david     (1000)      101 2023-06-10 15:06:04.000000 Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       30 2023-06-10 15:06:04.000000 Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/top_level.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp/
--rw-rw-r--   0 david     (1000) david     (1000)      305 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    10522 2023-06-10 14:56:44.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/auth.py
--rw-rw-r--   0 david     (1000) david     (1000)    11183 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/bigapp.py
--rw-rw-r--   0 david     (1000) david     (1000)     6229 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/blueprint.py
--rw-rw-r--   0 david     (1000) david     (1000)     4958 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/helpers.py
--rw-rw-r--   0 david     (1000) david     (1000)     5845 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/orm.py
--rw-rw-r--   0 david     (1000) david     (1000)      788 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/registeries.py
--rw-rw-r--   0 david     (1000) david     (1000)     1659 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/resources.py
--rw-rw-r--   0 david     (1000) david     (1000)     7663 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/security.py
--rw-rw-r--   0 david     (1000) david     (1000)     3093 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp/utilities.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/
--rw-rw-r--   0 david     (1000) david     (1000)       46 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/builtins/
--rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/builtins/context_processors.py
--rw-rw-r--   0 david     (1000) david     (1000)      915 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/static/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/static/css/
--rw-rw-r--   0 david     (1000) david     (1000)       45 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/static/css/example__css.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/static/img/
--rw-rw-r--   0 david     (1000) david     (1000)    28469 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/static/js/
--rw-rw-r--   0 david     (1000) david     (1000)      119 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/static/js/example__js.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/
--rw-rw-r--   0 david     (1000) david     (1000)      268 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/400.html
--rw-rw-r--   0 david     (1000) david     (1000)      315 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/401.html
--rw-rw-r--   0 david     (1000) david     (1000)      261 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/403.html
--rw-rw-r--   0 david     (1000) david     (1000)      281 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/404.html
--rw-rw-r--   0 david     (1000) david     (1000)      302 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/405.html
--rw-rw-r--   0 david     (1000) david     (1000)      278 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/500.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/
--rw-rw-r--   0 david     (1000) david     (1000)      766 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/
--rw-rw-r--   0 david     (1000) david     (1000)       13 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/footer.html
--rw-rw-r--   0 david     (1000) david     (1000)       11 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/menu.html
--rw-rw-r--   0 david     (1000) david     (1000)     9883 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/cli.py
--rw-rw-r--   0 david     (1000) david     (1000)      992 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/resources.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-10 15:06:04.921279 Flask-BigApp-2023.1.9.3/tests/
--rw-rw-r--   0 david     (1000) david     (1000)     2537 2023-06-10 14:53:13.000000 Flask-BigApp-2023.1.9.3/tests/test_group.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.322229 Flask-BigApp-2023.1.9.4/
+-rw-rw-r--   0 david     (1000) david     (1000)    25342 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)       60 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-06-29 07:18:10.322229 Flask-BigApp-2023.1.9.4/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      699 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)      271 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)      174 2023-06-29 07:18:10.322229 Flask-BigApp-2023.1.9.4/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     1582 2023-06-29 07:18:04.000000 Flask-BigApp-2023.1.9.4/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.314229 Flask-BigApp-2023.1.9.4/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.318229 Flask-BigApp-2023.1.9.4/src/Flask_BigApp.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-06-29 07:18:10.000000 Flask-BigApp-2023.1.9.4/src/Flask_BigApp.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     1855 2023-06-29 07:18:10.000000 Flask-BigApp-2023.1.9.4/src/Flask_BigApp.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-29 07:18:10.000000 Flask-BigApp-2023.1.9.4/src/Flask_BigApp.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       54 2023-06-29 07:18:10.000000 Flask-BigApp-2023.1.9.4/src/Flask_BigApp.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-15 10:09:07.000000 Flask-BigApp-2023.1.9.4/src/Flask_BigApp.egg-info/not-zip-safe
+-rw-rw-r--   0 david     (1000) david     (1000)      101 2023-06-29 07:18:10.000000 Flask-BigApp-2023.1.9.4/src/Flask_BigApp.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       30 2023-06-29 07:18:10.000000 Flask-BigApp-2023.1.9.4/src/Flask_BigApp.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.318229 Flask-BigApp-2023.1.9.4/src/flask_bigapp/
+-rw-rw-r--   0 david     (1000) david     (1000)      305 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10522 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp/auth.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11175 2023-06-15 10:12:02.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp/bigapp.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6229 2023-06-29 07:12:39.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp/blueprint.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4756 2023-06-29 07:03:10.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp/helpers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5845 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp/orm.py
+-rw-rw-r--   0 david     (1000) david     (1000)      788 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp/registeries.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1659 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp/resources.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7663 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp/security.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3098 2023-06-29 07:12:56.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp/utilities.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.318229 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/
+-rw-rw-r--   0 david     (1000) david     (1000)       46 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.314229 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.318229 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/builtins/
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/builtins/context_processors.py
+-rw-rw-r--   0 david     (1000) david     (1000)      915 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.314229 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/static/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.318229 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/static/css/
+-rw-rw-r--   0 david     (1000) david     (1000)       45 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/static/css/example__css.css
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.318229 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/static/img/
+-rw-rw-r--   0 david     (1000) david     (1000)    28469 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.318229 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/static/js/
+-rw-rw-r--   0 david     (1000) david     (1000)      119 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/static/js/example__js.js
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.314229 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.314229 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.318229 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/
+-rw-rw-r--   0 david     (1000) david     (1000)      268 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/400.html
+-rw-rw-r--   0 david     (1000) david     (1000)      315 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/401.html
+-rw-rw-r--   0 david     (1000) david     (1000)      261 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/403.html
+-rw-rw-r--   0 david     (1000) david     (1000)      281 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/404.html
+-rw-rw-r--   0 david     (1000) david     (1000)      302 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/405.html
+-rw-rw-r--   0 david     (1000) david     (1000)      278 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/500.html
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.322229 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/
+-rw-rw-r--   0 david     (1000) david     (1000)      766 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.322229 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/
+-rw-rw-r--   0 david     (1000) david     (1000)       13 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/footer.html
+-rw-rw-r--   0 david     (1000) david     (1000)       11 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/menu.html
+-rw-rw-r--   0 david     (1000) david     (1000)     9883 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/cli.py
+-rw-rw-r--   0 david     (1000) david     (1000)      992 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/resources.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 07:18:10.322229 Flask-BigApp-2023.1.9.4/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)     2537 2023-06-15 10:08:54.000000 Flask-BigApp-2023.1.9.4/tests/test_group.py
```

### Comparing `Flask-BigApp-2023.1.9.3/LICENSE` & `Flask-BigApp-2023.1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.3/PKG-INFO` & `Flask-BigApp-2023.1.9.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-BigApp
-Version: 2023.1.9.3
+Version: 2023.1.9.4
 Summary: A Flask auto importer that allows your Flask apps to grow big.
 Home-page: https://github.com/Flask-Planet/Flask-BigApp
 Author: David Carmichael
 Author-email: carmichaelits@gmail.com
 License: GNU Lesser General Public License v2.1
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Flask-BigApp-2023.1.9.3/README.md` & `Flask-BigApp-2023.1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.3/setup.py` & `Flask-BigApp-2023.1.9.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from setuptools import setup, find_packages
 
 readme = pathlib.Path(pathlib.Path.cwd() / "README.md").read_text()
 
 setup(
     name='Flask-BigApp',
-    version=f'2023.1.9.3',
+    version=f'2023.1.9.4',
     url='https://github.com/Flask-Planet/Flask-BigApp',
     license='GNU Lesser General Public License v2.1',
     author='David Carmichael',
     author_email='carmichaelits@gmail.com',
     description='A Flask auto importer that allows your Flask apps to grow big.',
     long_description=f'{readme}',
     long_description_content_type='text/markdown',
```

### Comparing `Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/PKG-INFO` & `Flask-BigApp-2023.1.9.4/src/Flask_BigApp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-BigApp
-Version: 2023.1.9.3
+Version: 2023.1.9.4
 Summary: A Flask auto importer that allows your Flask apps to grow big.
 Home-page: https://github.com/Flask-Planet/Flask-BigApp
 Author: David Carmichael
 Author-email: carmichaelits@gmail.com
 License: GNU Lesser General Public License v2.1
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Flask-BigApp-2023.1.9.3/src/Flask_BigApp.egg-info/SOURCES.txt` & `Flask-BigApp-2023.1.9.4/src/Flask_BigApp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.3/src/flask_bigapp/auth.py` & `Flask-BigApp-2023.1.9.4/src/flask_bigapp/auth.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.3/src/flask_bigapp/bigapp.py` & `Flask-BigApp-2023.1.9.4/src/flask_bigapp/bigapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .blueprint import BigAppBlueprint
 from .helpers import init_app_config
 from .registeries import ModelRegistry
 from .resources import Resources
 from .utilities import cast_to_bool, cast_to_import_str, deprecated
 
 
-class BigApp(object):
+class BigApp:
     _app: Flask
     _app_name: str
     _app_path: Path
     _app_folder: Path
 
     __model_registry__: ModelRegistry
```

### Comparing `Flask-BigApp-2023.1.9.3/src/flask_bigapp/blueprint.py` & `Flask-BigApp-2023.1.9.4/src/flask_bigapp/blueprint.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.3/src/flask_bigapp/helpers.py` & `Flask-BigApp-2023.1.9.4/src/flask_bigapp/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 import logging
 import os
 from pathlib import Path
 
 from toml import load as toml_load
 
 from .resources import Resources
-from .utilities import if_env_replace, capitalize_dict_keys, cast_to_bool, lower_dict_keys
+from .utilities import cast_to_bool, process_dict
 
 
 def build_database_uri(database_config_value: dict, app) -> str:
     """
     Puts together the correct database URI depending on the type specified.
 
     Fails if type is not supported.
     """
     app_root = Path(app.root_path)
 
-    db_type = if_env_replace(database_config_value.get("TYPE", "None"))
-    db_name = if_env_replace(database_config_value.get('DATABASE_NAME', 'database'))
-
-    db_location = if_env_replace(database_config_value.get("LOCATION", "db"))
-    db_port = if_env_replace(str(database_config_value.get('PORT', 'None')))
-
-    db_username = if_env_replace(database_config_value.get('USERNAME', 'None'))
-    db_password = if_env_replace(database_config_value.get('PASSWORD', 'None'))
+    db_type = database_config_value.get("TYPE", "None")
+    db_name = database_config_value.get('DATABASE_NAME', 'database')
+    db_location = database_config_value.get("LOCATION", "db")
+    db_port = str(database_config_value.get('PORT', 'None'))
+    db_username = database_config_value.get('USERNAME', 'None')
+    db_password = database_config_value.get('PASSWORD', 'None')
 
     db_allowed = ('postgresql', 'mysql', 'oracle')
 
     if db_type == "sqlite":
         if db_location is not None:
 
             if Path(db_location).exists():
-                database = Path(db_location / f"{db_name}.db")
+                database = Path(Path(db_location) / f"{db_name}.db")
                 return f"sqlite:///{database}"
 
             db_location_path = Path(app_root / db_location)
             db_location_path.mkdir(parents=True, exist_ok=True)
             db_location_file_path = db_location_path / f"{db_name}.db"
             return f"sqlite:///{db_location_file_path}"
 
         db_at_root = Path(app_root / f"{db_name}.db")
-        return f"{db_type}:///{db_at_root}"
+        return f"sqlite:///{db_at_root}"
 
     if db_type in db_allowed:
         return f"{db_type}://{db_username}:{db_password}@{db_location}:{db_port}/{db_name}"
 
     raise ValueError(
         "Unknown database type, must be: postgresql / mysql / oracle / sqlite")
 
@@ -62,34 +60,35 @@
         )
 
     config_suffix = ('.toml', '.tml')
 
     if config_file_path.suffix not in config_suffix:
         raise TypeError("Config from_file must be one of the following types: .toml / .tml")
 
-    config = capitalize_dict_keys(toml_load(config_file_path))
-    flask_config = capitalize_dict_keys(config.get("FLASK"))
+    config = process_dict(toml_load(config_file_path), key_case_switch="upper")
+
+    flask_config = config.get("FLASK")
     session_config = config.get("SESSION")
-    database_config = capitalize_dict_keys(config.get("DATABASE"))
+    database_config = config.get("DATABASE")
 
     if flask_config is not None and isinstance(flask_config, dict):
         for flask_config_key, flask_config_value in flask_config.items():
-            app.config.update({str(flask_config_key): if_env_replace(flask_config_value)})
+            app.config.update({flask_config_key: flask_config_value})
 
     if database_config is not None and isinstance(database_config, dict):
         app.config['SQLALCHEMY_BINDS'] = dict()
         for database_config_key, database_config_values in database_config.items():
-            values = capitalize_dict_keys(database_config_values)
-            if values.get("ENABLED", False):
+            if database_config_values.get("ENABLED", False):
+                database_uri = build_database_uri(database_config_values, app)
                 if database_config_key == "MAIN":
-                    app.config['SQLALCHEMY_DATABASE_URI'] = f"{build_database_uri(values, app)}"
+                    app.config['SQLALCHEMY_DATABASE_URI'] = database_uri
                     continue
 
                 app.config['SQLALCHEMY_BINDS'].update({
-                    str(database_config_key).lower(): f"{build_database_uri(values, app)}"
+                    str(database_config_key).lower(): database_uri
                 })
 
     return {"FLASK": flask_config, "SESSION": session_config, "DATABASE": database_config}
 
 
 def init_bp_config(blueprint_name: str, config_file_path: Path) -> tuple:
     """
@@ -100,23 +99,23 @@
         raise FileNotFoundError(f"{blueprint_name} Blueprint config from_file {config_file_path.name} was not found")
 
     config_suffix = ('.toml', '.tml')
 
     if config_file_path.suffix not in config_suffix:
         raise TypeError("Config from_file must be one of the following types: .toml / .tml")
 
-    config = capitalize_dict_keys(toml_load(config_file_path))
+    config = process_dict(toml_load(config_file_path), key_case_switch="lower")
 
-    enabled = cast_to_bool(config.get('ENABLED', False))
+    enabled = cast_to_bool(config.get('enabled', False))
 
     if not enabled:
         return enabled, {}, {}
 
-    session = config.get('SESSION', {})
-    settings = lower_dict_keys(config.get('SETTINGS', {}))
+    session = config.get('session', {})
+    settings = config.get('settings', {})
 
     kwargs = dict()
 
     valid_settings = (
         'url_prefix', 'subdomain', 'url_defaults', 'static_folder', 'template_folder', 'static_url_path', 'root_path'
     )
```

### Comparing `Flask-BigApp-2023.1.9.3/src/flask_bigapp/orm.py` & `Flask-BigApp-2023.1.9.4/src/flask_bigapp/orm.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.3/src/flask_bigapp/registeries.py` & `Flask-BigApp-2023.1.9.4/src/flask_bigapp/registeries.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.3/src/flask_bigapp/resources.py` & `Flask-BigApp-2023.1.9.4/src/flask_bigapp/resources.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.3/src/flask_bigapp/security.py` & `Flask-BigApp-2023.1.9.4/src/flask_bigapp/security.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.3/src/flask_bigapp/utilities.py` & `Flask-BigApp-2023.1.9.4/src/flask_bigapp/utilities.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,32 +40,28 @@
     if isinstance(env_value, str):
         if re.match(pattern, env_value):
             env_var = re.findall(pattern, env_value)[0]
             return os.environ.get(env_var, "ENV_KEY_NOT_FOUND")
     return env_value
 
 
-def capitalize_dict_keys(dictionary: t.Optional[dict]) -> dict:
-    """
-    Capitalizes the keys in a dictionary.
-    """
-    if dictionary is None:
+def process_dict(this_dict: t.Optional[dict], key_case_switch: str = "upper") -> dict:
+    if this_dict is None:
         return {}
 
-    return {key.upper(): value for key, value in dictionary.items()}
+    return_dict = {}
+    for key, value in this_dict.items():
+        cs_key = key.upper() if key_case_switch == "upper" else key.lower()
+        if isinstance(value, dict):
+            return_dict[cs_key] = process_dict(value, key_case_switch)
+            continue
 
+        return_dict[cs_key] = if_env_replace(value)
 
-def lower_dict_keys(dictionary: t.Optional[dict]) -> dict:
-    """
-    Lowercases the keys in a dictionary.
-    """
-    if dictionary is None:
-        return {}
-
-    return {key.lower(): value for key, value in dictionary.items()}
+    return return_dict
 
 
 def cast_to_import_str(app_name: str, folder_path: Path) -> str:
     folder_parts = folder_path.parts
     parts = folder_parts[folder_parts.index(app_name):]
     if sys.version_info.major == 3:
         if sys.version_info.minor < 9:
```

### Comparing `Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py` & `Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png` & `Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html` & `Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/cli.py` & `Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/cli.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.3/src/flask_bigapp_cli/resources.py` & `Flask-BigApp-2023.1.9.4/src/flask_bigapp_cli/resources.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9.3/tests/test_group.py` & `Flask-BigApp-2023.1.9.4/tests/test_group.py`

 * *Files identical despite different names*

