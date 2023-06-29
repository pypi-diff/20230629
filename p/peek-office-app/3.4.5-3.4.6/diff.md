# Comparing `tmp/peek-office-app-3.4.5.tar.gz` & `tmp/peek-office-app-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-office-app-3.4.5.tar", last modified: Wed Jun 28 07:27:09 2023, max compression
+gzip compressed data, was "peek-office-app-3.4.6.tar", last modified: Thu Jun 29 10:20:56 2023, max compression
```

## Comparing `peek-office-app-3.4.5.tar` & `peek-office-app-3.4.6.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.256088 peek-office-app-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-28 07:27:09.256088 peek-office-app-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.252088 peek-office-app-3.4.5/peek_office_app/
--rw-r--r--   0 root         (0) root         (0)      487 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/.browserslistrc
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/.gitignore
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)     1082 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/README.md
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-28 07:27:09.000000 peek-office-app-3.4.5/peek_office_app/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6615 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/angular.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.252088 peek-office-app-3.4.5/peek_office_app/e2e/
--rw-r--r--   0 root         (0) root         (0)      326 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/e2e/app.e2e-spec.ts
--rw-r--r--   0 root         (0) root         (0)      227 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/e2e/app.po.ts
--rw-r--r--   0 root         (0) root         (0)      367 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/e2e/tsconfig.e2e.json
--rw-r--r--   0 root         (0) root         (0)     1341 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/karma.conf.js
--rw-r--r--   0 root         (0) root         (0)   680107 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/package-lock.json
--rw-r--r--   0 root         (0) root         (0)     3021 2023-06-28 07:27:09.000000 peek-office-app-3.4.5/peek_office_app/package.json
--rw-r--r--   0 root         (0) root         (0)      868 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/protractor.conf.js
--rw-r--r--   0 root         (0) root         (0)      279 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/proxy.conf.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.253088 peek-office-app-3.4.5/peek_office_app/src/
--rw-r--r--   0 root         (0) root         (0)     1151 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/_components.scss
--rw-r--r--   0 root         (0) root         (0)      994 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/_variables.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.253088 peek-office-app-3.4.5/peek_office_app/src/app/
--rw-r--r--   0 root         (0) root         (0)     2400 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/app.module.ts
--rw-r--r--   0 root         (0) root         (0)     1110 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/app.routes.ts
--rw-r--r--   0 root         (0) root         (0)      897 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/app.services.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.253088 peek-office-app-3.4.5/peek_office_app/src/app/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.253088 peek-office-app-3.4.5/peek_office_app/src/app/core/components/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.253088 peek-office-app-3.4.5/peek_office_app/src/app/core/components/app/
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/core/components/app/app.component.html
--rw-r--r--   0 root         (0) root         (0)      899 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/core/components/app/app.component.scss
--rw-r--r--   0 root         (0) root         (0)     1391 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/core/components/app/app.component.ts
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/core/components/app/index.ts
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/core/components/components.module.ts
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/core/components/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.254088 peek-office-app-3.4.5/peek_office_app/src/app/core/components/sidebar/
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/core/components/sidebar/index.ts
--rw-r--r--   0 root         (0) root         (0)     3805 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/core/components/sidebar/sidebar.component.html
--rw-r--r--   0 root         (0) root         (0)     1457 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/core/components/sidebar/sidebar.component.scss
--rw-r--r--   0 root         (0) root         (0)     2935 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/core/components/sidebar/sidebar.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.254088 peek-office-app-3.4.5/peek_office_app/src/app/core/components/status/
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/core/components/status/index.ts
--rw-r--r--   0 root         (0) root         (0)      861 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/core/components/status/status.component.html
--rw-r--r--   0 root         (0) root         (0)      505 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/core/components/status/status.component.scss
--rw-r--r--   0 root         (0) root         (0)     1585 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/core/components/status/status.component.ts
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/core/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.254088 peek-office-app-3.4.5/peek_office_app/src/app/pages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.254088 peek-office-app-3.4.5/peek_office_app/src/app/pages/config/
--rw-r--r--   0 root         (0) root         (0)      948 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/pages/config/config.page.html
--rw-r--r--   0 root         (0) root         (0)     1373 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/pages/config/config.page.scss
--rw-r--r--   0 root         (0) root         (0)      723 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/pages/config/config.page.ts
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/pages/config/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.254088 peek-office-app-3.4.5/peek_office_app/src/app/pages/home/
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/pages/home/home.page.html
--rw-r--r--   0 root         (0) root         (0)      333 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/pages/home/home.page.scss
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/pages/home/home.page.ts
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/pages/home/index.ts
--rw-r--r--   0 root         (0) root         (0)      126 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/pages/index.ts
--rw-r--r--   0 root         (0) root         (0)      800 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/pages/pages.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.255088 peek-office-app-3.4.5/peek_office_app/src/app/pages/unknown-route/
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/pages/unknown-route/index.ts
--rw-r--r--   0 root         (0) root         (0)    19057 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/pages/unknown-route/unknown-route.page.html
--rw-r--r--   0 root         (0) root         (0)     1101 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/pages/unknown-route/unknown-route.page.scss
--rw-r--r--   0 root         (0) root         (0)      513 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/pages/unknown-route/unknown-route.page.ts
--rw-r--r--   0 root         (0) root         (0)      222 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/app/plugin-root.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.255088 peek-office-app-3.4.5/peek_office_app/src/assets/
--rw-r--r--   0 root         (0) root         (0)   156480 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/assets/Poppins-Medium.ttf
--rw-r--r--   0 root         (0) root         (0)   158192 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/assets/Poppins-Regular.ttf
--rw-r--r--   0 root         (0) root         (0)   155192 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/assets/Poppins-SemiBold.ttf
--rw-r--r--   0 root         (0) root         (0)   715281 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/assets/home-background.png
--rw-r--r--   0 root         (0) root         (0)    66513 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/assets/home-center.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.256088 peek-office-app-3.4.5/peek_office_app/src/assets/peek_core_docdb/
--rw-r--r--   0 root         (0) root         (0)    12054 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/assets/peek_core_docdb/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.256088 peek-office-app-3.4.5/peek_office_app/src/assets/peek_core_search/
--rw-r--r--   0 root         (0) root         (0)    12730 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/assets/peek_core_search/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.256088 peek-office-app-3.4.5/peek_office_app/src/assets/peek_core_user/
--rw-r--r--   0 root         (0) root         (0)     5572 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/assets/peek_core_user/plugin_icon.png
--rw-r--r--   0 root         (0) root         (0)   161189 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/assets/sidebar_background.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.256088 peek-office-app-3.4.5/peek_office_app/src/environments/
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/environments/environment.prod.ts
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/environments/environment.ts
--rw-r--r--   0 root         (0) root         (0)       61 2023-06-28 07:27:09.000000 peek-office-app-3.4.5/peek_office_app/src/environments/peek-app-environment.ts
--rw-r--r--   0 root         (0) root         (0)    39980 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     4988 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/index.html
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/main.ts
--rw-r--r--   0 root         (0) root         (0)     2395 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/polyfills.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.256088 peek-office-app-3.4.5/peek_office_app/src/styles/
--rw-r--r--   0 root         (0) root         (0)     5595 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/styles/shared.scss
--rw-r--r--   0 root         (0) root         (0)    33066 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/styles/theme.less
--rw-r--r--   0 root         (0) root         (0)     3384 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/styles.scss
--rw-r--r--   0 root         (0) root         (0)     1090 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/test.ts
--rw-r--r--   0 root         (0) root         (0)      521 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/tsconfig.app.json
--rw-r--r--   0 root         (0) root         (0)      242 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/tsconfig.spec.json
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/src/typings.d.ts
--rw-r--r--   0 root         (0) root         (0)      414 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/tsconfig.json
--rw-r--r--   0 root         (0) root         (0)      320 2023-06-28 07:25:24.000000 peek-office-app-3.4.5/peek_office_app/tsconfig.worker.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:09.252088 peek-office-app-3.4.5/peek_office_app.egg-info/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-28 07:27:09.000000 peek-office-app-3.4.5/peek_office_app.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3632 2023-06-28 07:27:09.000000 peek-office-app-3.4.5/peek_office_app.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:27:09.000000 peek-office-app-3.4.5/peek_office_app.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:27:09.000000 peek-office-app-3.4.5/peek_office_app.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-28 07:27:09.000000 peek-office-app-3.4.5/peek_office_app.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-28 07:27:09.000000 peek-office-app-3.4.5/peek_office_app.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:27:09.256088 peek-office-app-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3089 2023-06-28 07:27:09.000000 peek-office-app-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.718471 peek-office-app-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-29 10:20:56.718471 peek-office-app-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.713471 peek-office-app-3.4.6/peek_office_app/
+-rw-r--r--   0 root         (0) root         (0)      487 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/.browserslistrc
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/README.md
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-29 10:20:56.000000 peek-office-app-3.4.6/peek_office_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6615 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/angular.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.714471 peek-office-app-3.4.6/peek_office_app/e2e/
+-rw-r--r--   0 root         (0) root         (0)      326 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/e2e/app.e2e-spec.ts
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/e2e/app.po.ts
+-rw-r--r--   0 root         (0) root         (0)      367 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/e2e/tsconfig.e2e.json
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/karma.conf.js
+-rw-r--r--   0 root         (0) root         (0)   680109 2023-06-29 10:19:20.000000 peek-office-app-3.4.6/peek_office_app/package-lock.json
+-rw-r--r--   0 root         (0) root         (0)     3022 2023-06-29 10:20:56.000000 peek-office-app-3.4.6/peek_office_app/package.json
+-rw-r--r--   0 root         (0) root         (0)      868 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/protractor.conf.js
+-rw-r--r--   0 root         (0) root         (0)      279 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/proxy.conf.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.715471 peek-office-app-3.4.6/peek_office_app/src/
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/_components.scss
+-rw-r--r--   0 root         (0) root         (0)      994 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/_variables.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.715471 peek-office-app-3.4.6/peek_office_app/src/app/
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/app.module.ts
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/app.routes.ts
+-rw-r--r--   0 root         (0) root         (0)      897 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/app.services.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.715471 peek-office-app-3.4.6/peek_office_app/src/app/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.715471 peek-office-app-3.4.6/peek_office_app/src/app/core/components/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.715471 peek-office-app-3.4.6/peek_office_app/src/app/core/components/app/
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/core/components/app/app.component.html
+-rw-r--r--   0 root         (0) root         (0)      899 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/core/components/app/app.component.scss
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/core/components/app/app.component.ts
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/core/components/app/index.ts
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/core/components/components.module.ts
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/core/components/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.715471 peek-office-app-3.4.6/peek_office_app/src/app/core/components/sidebar/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/core/components/sidebar/index.ts
+-rw-r--r--   0 root         (0) root         (0)     3805 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/core/components/sidebar/sidebar.component.html
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/core/components/sidebar/sidebar.component.scss
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/core/components/sidebar/sidebar.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.716471 peek-office-app-3.4.6/peek_office_app/src/app/core/components/status/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/core/components/status/index.ts
+-rw-r--r--   0 root         (0) root         (0)      861 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/core/components/status/status.component.html
+-rw-r--r--   0 root         (0) root         (0)      505 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/core/components/status/status.component.scss
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/core/components/status/status.component.ts
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/core/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.716471 peek-office-app-3.4.6/peek_office_app/src/app/pages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.716471 peek-office-app-3.4.6/peek_office_app/src/app/pages/config/
+-rw-r--r--   0 root         (0) root         (0)      948 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/pages/config/config.page.html
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/pages/config/config.page.scss
+-rw-r--r--   0 root         (0) root         (0)      723 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/pages/config/config.page.ts
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/pages/config/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.716471 peek-office-app-3.4.6/peek_office_app/src/app/pages/home/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/pages/home/home.page.html
+-rw-r--r--   0 root         (0) root         (0)      333 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/pages/home/home.page.scss
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/pages/home/home.page.ts
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/pages/home/index.ts
+-rw-r--r--   0 root         (0) root         (0)      126 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/pages/index.ts
+-rw-r--r--   0 root         (0) root         (0)      800 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/pages/pages.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.716471 peek-office-app-3.4.6/peek_office_app/src/app/pages/unknown-route/
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/pages/unknown-route/index.ts
+-rw-r--r--   0 root         (0) root         (0)    19057 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/pages/unknown-route/unknown-route.page.html
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/pages/unknown-route/unknown-route.page.scss
+-rw-r--r--   0 root         (0) root         (0)      513 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/pages/unknown-route/unknown-route.page.ts
+-rw-r--r--   0 root         (0) root         (0)      222 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/app/plugin-root.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.717471 peek-office-app-3.4.6/peek_office_app/src/assets/
+-rw-r--r--   0 root         (0) root         (0)   156480 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/assets/Poppins-Medium.ttf
+-rw-r--r--   0 root         (0) root         (0)   158192 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/assets/Poppins-Regular.ttf
+-rw-r--r--   0 root         (0) root         (0)   155192 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/assets/Poppins-SemiBold.ttf
+-rw-r--r--   0 root         (0) root         (0)   715281 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/assets/home-background.png
+-rw-r--r--   0 root         (0) root         (0)    66513 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/assets/home-center.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.717471 peek-office-app-3.4.6/peek_office_app/src/assets/peek_core_docdb/
+-rw-r--r--   0 root         (0) root         (0)    12054 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/assets/peek_core_docdb/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.717471 peek-office-app-3.4.6/peek_office_app/src/assets/peek_core_search/
+-rw-r--r--   0 root         (0) root         (0)    12730 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/assets/peek_core_search/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.717471 peek-office-app-3.4.6/peek_office_app/src/assets/peek_core_user/
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/assets/peek_core_user/plugin_icon.png
+-rw-r--r--   0 root         (0) root         (0)   161189 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/assets/sidebar_background.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.718471 peek-office-app-3.4.6/peek_office_app/src/environments/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/environments/environment.prod.ts
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/environments/environment.ts
+-rw-r--r--   0 root         (0) root         (0)       61 2023-06-29 10:20:56.000000 peek-office-app-3.4.6/peek_office_app/src/environments/peek-app-environment.ts
+-rw-r--r--   0 root         (0) root         (0)    39980 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)     4988 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/index.html
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/main.ts
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/polyfills.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.718471 peek-office-app-3.4.6/peek_office_app/src/styles/
+-rw-r--r--   0 root         (0) root         (0)     5595 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/styles/shared.scss
+-rw-r--r--   0 root         (0) root         (0)    33066 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/styles/theme.less
+-rw-r--r--   0 root         (0) root         (0)     3384 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/styles.scss
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/test.ts
+-rw-r--r--   0 root         (0) root         (0)      521 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/tsconfig.app.json
+-rw-r--r--   0 root         (0) root         (0)      242 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/tsconfig.spec.json
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/src/typings.d.ts
+-rw-r--r--   0 root         (0) root         (0)      414 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/tsconfig.json
+-rw-r--r--   0 root         (0) root         (0)      320 2023-06-29 10:19:15.000000 peek-office-app-3.4.6/peek_office_app/tsconfig.worker.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:56.714471 peek-office-app-3.4.6/peek_office_app.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-29 10:20:56.000000 peek-office-app-3.4.6/peek_office_app.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-06-29 10:20:56.000000 peek-office-app-3.4.6/peek_office_app.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:20:56.000000 peek-office-app-3.4.6/peek_office_app.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:20:56.000000 peek-office-app-3.4.6/peek_office_app.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-29 10:20:56.000000 peek-office-app-3.4.6/peek_office_app.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-29 10:20:56.000000 peek-office-app-3.4.6/peek_office_app.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:20:56.718471 peek-office-app-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3089 2023-06-29 10:20:56.000000 peek-office-app-3.4.6/setup.py
```

### Comparing `peek-office-app-3.4.5/README.rst` & `peek-office-app-3.4.6/README.rst`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/README.md` & `peek-office-app-3.4.6/peek_office_app/README.md`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/angular.json` & `peek-office-app-3.4.6/peek_office_app/angular.json`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/karma.conf.js` & `peek-office-app-3.4.6/peek_office_app/karma.conf.js`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/package-lock.json` & `peek-office-app-3.4.6/peek_office_app/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999852138307552%*

 * *Differences: {"'dependencies'": "{'@synerty/vortexjs': {'version': '3.3.11', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@synerty/vortexjs/-/vortexjs-3.3.11.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-IkbVN+gLBE0NJBQEjlqAAbkfvQTCp6A8vU/gLZJXsHvUzsEf7poHSt4Vf2NauWF3N1nJh2Yt20f1T/vjxdDlyw==', "*

 * *                   "'dependencies': {'tslib': {'version': '2.6.0', 'resolved': "*

 * *                   "'https://registry.npmjs.org/tslib/-/tslib-2.6.0.tgz', 'integrity': "*

 * *                 […]*

```diff
@@ -2279,25 +2279,25 @@
             },
             "resolved": "https://registry.npmjs.org/@synerty/peek-plugin-base-js/-/peek-plugin-base-js-10.7.10.tgz",
             "version": "10.7.10"
         },
         "@synerty/vortexjs": {
             "dependencies": {
                 "tslib": {
-                    "integrity": "sha512-mSxlJJwl3BMEQCUNnxXBU9jP4JBktcEGhURcPR6VQVlnP0FdDEsIaz0C35dXNGLyRfrATNofF0F5p2KPxQgB+w==",
-                    "resolved": "https://registry.npmjs.org/tslib/-/tslib-2.5.3.tgz",
-                    "version": "2.5.3"
+                    "integrity": "sha512-7At1WUettjcSRHXCyYtTselblcHl9PJFFVKiCAy/bY97+BPZXSQ2wbq0P9s8tK2G7dFQfNnlJnPAiArVBVBsfA==",
+                    "resolved": "https://registry.npmjs.org/tslib/-/tslib-2.6.0.tgz",
+                    "version": "2.6.0"
                 }
             },
-            "integrity": "sha512-WuMRpei1gHkT7pUGBtuIjRAl7U5KY5rkKdmgJXIBjl378wjo+pcTlkobrzAZf1mfx7OlrAMP5C9pPWOjzEhgBw==",
+            "integrity": "sha512-IkbVN+gLBE0NJBQEjlqAAbkfvQTCp6A8vU/gLZJXsHvUzsEf7poHSt4Vf2NauWF3N1nJh2Yt20f1T/vjxdDlyw==",
             "requires": {
                 "tslib": "^2.0.0"
             },
-            "resolved": "https://registry.npmjs.org/@synerty/vortexjs/-/vortexjs-3.3.9.tgz",
-            "version": "3.3.9"
+            "resolved": "https://registry.npmjs.org/@synerty/vortexjs/-/vortexjs-3.3.11.tgz",
+            "version": "3.3.11"
         },
         "@types/cordova": {
             "integrity": "sha512-rkiiTuf/z2wTd4RxFOb+clE7PF4AEJU0hsczbUdkHHBtkUmpWQpEddynNfJYKYtZFJKbq4F+brfekt1kx85IZA==",
             "resolved": "https://registry.npmjs.org/@types/cordova/-/cordova-0.0.34.tgz",
             "version": "0.0.34"
         },
         "@types/emscripten": {
```

### Comparing `peek-office-app-3.4.5/peek_office_app/package.json` & `peek-office-app-3.4.6/peek_office_app/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9226388229710489%*

 * *Differences: {"'dependencies'": "{'@synerty/vortexjs': '^3.3.11'}",*

 * * "'scripts'": "{'start': 'ng serve --disableHostCheck --host 3.4.6.0 --port 4002 --proxy-config "*

 * *              "proxy.conf.json'}",*

 * * "'version'": "'3.4.6'"}*

```diff
@@ -25,15 +25,15 @@
         "@capacitor/filesystem": "^1.1.0",
         "@capacitor/geolocation": "^1.3.1",
         "@capacitor/ios": "^3.5.1",
         "@capacitor/local-notifications": "^1.1.0",
         "@capacitor/network": "^1.0.7",
         "@ionic/pwa-elements": "^3.1.1",
         "@synerty/peek-plugin-base-js": "^10.7.10",
-        "@synerty/vortexjs": "^3.3.9",
+        "@synerty/vortexjs": "^3.3.11",
         "assert": "^1.5.0",
         "base-64": "^0.1.0",
         "bootstrap": "^3.4.1",
         "cordova-plugin-nativeaudio": "^3.0.9",
         "core-js": "^3.6.5",
         "jquery": "^3.4.1",
         "json-stable-stringify": "^1.0.1",
@@ -71,12 +71,12 @@
     "private": true,
     "scripts": {
         "build": "ng build",
         "e2e": "ng e2e",
         "lint": "ng lint",
         "ng": "ng",
         "postinstall": "ngcc --properties es2015 es5 browser module main --first-only --create-ivy-entry-points",
-        "start": "ng serve --disableHostCheck --host 3.4.5.0 --port 4002 --proxy-config proxy.conf.json",
+        "start": "ng serve --disableHostCheck --host 3.4.6.0 --port 4002 --proxy-config proxy.conf.json",
         "test": "ng test"
     },
-    "version": "3.4.5"
+    "version": "3.4.6"
 }
```

### Comparing `peek-office-app-3.4.5/peek_office_app/protractor.conf.js` & `peek-office-app-3.4.6/peek_office_app/protractor.conf.js`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/_components.scss` & `peek-office-app-3.4.6/peek_office_app/src/_components.scss`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/_variables.scss` & `peek-office-app-3.4.6/peek_office_app/src/_variables.scss`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/app.module.ts` & `peek-office-app-3.4.6/peek_office_app/src/app/app.module.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/app.routes.ts` & `peek-office-app-3.4.6/peek_office_app/src/app/app.routes.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/app.services.ts` & `peek-office-app-3.4.6/peek_office_app/src/app/app.services.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/core/components/app/app.component.html` & `peek-office-app-3.4.6/peek_office_app/src/app/core/components/app/app.component.html`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/core/components/app/app.component.scss` & `peek-office-app-3.4.6/peek_office_app/src/app/core/components/app/app.component.scss`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/core/components/app/app.component.ts` & `peek-office-app-3.4.6/peek_office_app/src/app/core/components/app/app.component.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/core/components/components.module.ts` & `peek-office-app-3.4.6/peek_office_app/src/app/core/components/components.module.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/core/components/sidebar/sidebar.component.html` & `peek-office-app-3.4.6/peek_office_app/src/app/core/components/sidebar/sidebar.component.html`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/core/components/sidebar/sidebar.component.scss` & `peek-office-app-3.4.6/peek_office_app/src/app/core/components/sidebar/sidebar.component.scss`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/core/components/sidebar/sidebar.component.ts` & `peek-office-app-3.4.6/peek_office_app/src/app/core/components/sidebar/sidebar.component.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/core/components/status/status.component.html` & `peek-office-app-3.4.6/peek_office_app/src/app/core/components/status/status.component.html`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/core/components/status/status.component.ts` & `peek-office-app-3.4.6/peek_office_app/src/app/core/components/status/status.component.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/pages/config/config.page.html` & `peek-office-app-3.4.6/peek_office_app/src/app/pages/config/config.page.html`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/pages/config/config.page.scss` & `peek-office-app-3.4.6/peek_office_app/src/app/pages/config/config.page.scss`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/pages/config/config.page.ts` & `peek-office-app-3.4.6/peek_office_app/src/app/pages/config/config.page.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/pages/home/home.page.ts` & `peek-office-app-3.4.6/peek_office_app/src/app/pages/home/home.page.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/pages/pages.module.ts` & `peek-office-app-3.4.6/peek_office_app/src/app/pages/pages.module.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/pages/unknown-route/unknown-route.page.html` & `peek-office-app-3.4.6/peek_office_app/src/app/pages/unknown-route/unknown-route.page.html`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/pages/unknown-route/unknown-route.page.scss` & `peek-office-app-3.4.6/peek_office_app/src/app/pages/unknown-route/unknown-route.page.scss`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/app/pages/unknown-route/unknown-route.page.ts` & `peek-office-app-3.4.6/peek_office_app/src/app/pages/unknown-route/unknown-route.page.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/assets/Poppins-Medium.ttf` & `peek-office-app-3.4.6/peek_office_app/src/assets/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/assets/Poppins-Regular.ttf` & `peek-office-app-3.4.6/peek_office_app/src/assets/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/assets/Poppins-SemiBold.ttf` & `peek-office-app-3.4.6/peek_office_app/src/assets/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/assets/home-background.png` & `peek-office-app-3.4.6/peek_office_app/src/assets/home-background.png`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/assets/home-center.png` & `peek-office-app-3.4.6/peek_office_app/src/assets/home-center.png`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/assets/peek_core_docdb/icon.png` & `peek-office-app-3.4.6/peek_office_app/src/assets/peek_core_docdb/icon.png`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/assets/peek_core_search/icon.png` & `peek-office-app-3.4.6/peek_office_app/src/assets/peek_core_search/icon.png`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/assets/peek_core_user/plugin_icon.png` & `peek-office-app-3.4.6/peek_office_app/src/assets/peek_core_user/plugin_icon.png`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/assets/sidebar_background.png` & `peek-office-app-3.4.6/peek_office_app/src/assets/sidebar_background.png`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/favicon.ico` & `peek-office-app-3.4.6/peek_office_app/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/index.html` & `peek-office-app-3.4.6/peek_office_app/src/index.html`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/main.ts` & `peek-office-app-3.4.6/peek_office_app/src/main.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/polyfills.ts` & `peek-office-app-3.4.6/peek_office_app/src/polyfills.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/styles/shared.scss` & `peek-office-app-3.4.6/peek_office_app/src/styles/shared.scss`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/styles/theme.less` & `peek-office-app-3.4.6/peek_office_app/src/styles/theme.less`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/styles.scss` & `peek-office-app-3.4.6/peek_office_app/src/styles.scss`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/test.ts` & `peek-office-app-3.4.6/peek_office_app/src/test.ts`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app/src/tsconfig.app.json` & `peek-office-app-3.4.6/peek_office_app/src/tsconfig.app.json`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/peek_office_app.egg-info/SOURCES.txt` & `peek-office-app-3.4.6/peek_office_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-office-app-3.4.5/setup.py` & `peek-office-app-3.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_office_app"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Office UI App."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

