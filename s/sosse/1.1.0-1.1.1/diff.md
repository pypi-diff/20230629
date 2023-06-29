# Comparing `tmp/sosse-1.1.0.tar.gz` & `tmp/sosse-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosse-1.1.0.tar", last modified: Wed Jun 28 15:15:25 2023, max compression
+gzip compressed data, was "sosse-1.1.1.tar", last modified: Thu Jun 29 14:30:06 2023, max compression
```

## Comparing `sosse-1.1.0.tar` & `sosse-1.1.1.tar`

### file list

```diff
@@ -1,229 +1,229 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.720515 sosse-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-06-28 15:14:52.000000 sosse-1.1.0/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      351 2023-06-28 15:14:52.000000 sosse-1.1.0/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.612520 sosse-1.1.0/.gitlab/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-28 15:14:52.000000 sosse-1.1.0/.gitlab/changelog_config.yml
--rw-rw-rw-   0 root         (0) root         (0)     6939 2023-06-28 15:14:52.000000 sosse-1.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-06-28 15:14:52.000000 sosse-1.1.0/.readthedocs.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1008 2023-06-28 15:14:52.000000 sosse-1.1.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1635 2023-06-28 15:14:52.000000 sosse-1.1.0/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)    34523 2023-06-28 15:14:52.000000 sosse-1.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-28 15:14:52.000000 sosse-1.1.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     7504 2023-06-28 15:14:52.000000 sosse-1.1.0/Makefile
--rw-r--r--   0 root         (0) root         (0)     3198 2023-06-28 15:15:25.720515 sosse-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2806 2023-06-28 15:14:52.000000 sosse-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.616520 sosse-1.1.0/debian/
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-06-28 15:14:52.000000 sosse-1.1.0/debian/changelog
--rw-rw-rw-   0 root         (0) root         (0)        3 2023-06-28 15:14:52.000000 sosse-1.1.0/debian/compat
--rw-rw-rw-   0 root         (0) root         (0)      697 2023-06-28 15:14:52.000000 sosse-1.1.0/debian/control
--rwxrwxrwx   0 root         (0) root         (0)      182 2023-06-28 15:14:52.000000 sosse-1.1.0/debian/rules
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-28 15:14:52.000000 sosse-1.1.0/debian/sosse-crawler.service
--rw-rw-rw-   0 root         (0) root         (0)      803 2023-06-28 15:14:52.000000 sosse-1.1.0/debian/sosse-uwsgi.service
--rw-rw-rw-   0 root         (0) root         (0)     2176 2023-06-28 15:14:52.000000 sosse-1.1.0/debian/sosse.conf
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-28 15:14:52.000000 sosse-1.1.0/debian/sosse.install
--rw-rw-rw-   0 root         (0) root         (0)     2733 2023-06-28 15:14:52.000000 sosse-1.1.0/debian/sosse.postinst
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-06-28 15:14:52.000000 sosse-1.1.0/debian/uwsgi.ini
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-06-28 15:14:52.000000 sosse-1.1.0/debian/uwsgi.params
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.620520 sosse-1.1.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/Makefile
--rwxrwxrwx   0 root         (0) root         (0)      314 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/build_changelog.sh
--rw-rw-rw-   0 root         (0) root         (0)     1897 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/get_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.632519 sosse-1.1.0/doc/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.632519 sosse-1.1.0/doc/source/_extensions/
--rw-rw-rw-   0 root         (0) root         (0)     1124 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/_extensions/code_blocks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.632519 sosse-1.1.0/doc/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/_static/style.css
--rw-rw-rw-   0 root         (0) root         (0)      723 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/admin_ui.rst
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/administration.rst
--rw-rw-rw-   0 root         (0) root         (0)      502 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/archive.rst
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/authentication.rst
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/cli.rst
--rw-rw-rw-   0 root         (0) root         (0)     1951 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/config_file.rst
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/cookies.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.636519 sosse-1.1.0/doc/source/crawl/
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/crawl/add_to_queue.rst
--rw-rw-rw-   0 root         (0) root         (0)     1452 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/crawl/crawl_depth.rst
--rw-rw-rw-   0 root         (0) root         (0)     5773 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/crawl/policies.rst
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/crawl/status.rst
--rw-rw-rw-   0 root         (0) root         (0)     1452 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/documents.rst
--rw-rw-rw-   0 root         (0) root         (0)     1408 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/domain_settings.rst
--rw-rw-rw-   0 root         (0) root         (0)      315 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/excluded_urls.rst
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.640519 sosse-1.1.0/doc/source/install/
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/install/database.rst.template
--rw-rw-rw-   0 root         (0) root         (0)     1463 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/install/debian.rst
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/install/debian_upgrades.rst
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/install/docker.rst
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/install/docker_upgrades.rst
--rw-rw-rw-   0 root         (0) root         (0)     3444 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/install/pip.rst
--rw-rw-rw-   0 root         (0) root         (0)      450 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/install/pip_upgrades.rst
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/install.rst
--rw-rw-rw-   0 root         (0) root         (0)      988 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/permissions.rst
--rw-rw-rw-   0 root         (0) root         (0)     1141 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/screenshots.rst
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/search_engines.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.644519 sosse-1.1.0/doc/source/user/
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/user/cached.rst
--rw-rw-rw-   0 root         (0) root         (0)      593 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/user/history.rst
--rw-rw-rw-   0 root         (0) root         (0)     1407 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/user/preferences.rst
--rw-rw-rw-   0 root         (0) root         (0)     4293 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/user/search.rst
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/user/shortcut_list.rst
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/user/shortcuts.rst
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/user/statistics.rst
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-06-28 15:14:52.000000 sosse-1.1.0/doc/source/user_doc.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.644519 sosse-1.1.0/docker/
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-06-28 15:14:52.000000 sosse-1.1.0/docker/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-06-28 15:14:52.000000 sosse-1.1.0/docker/Makefile.common
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.644519 sosse-1.1.0/docker/debian/
--rw-rw-rw-   0 root         (0) root         (0)     1965 2023-06-28 15:14:52.000000 sosse-1.1.0/docker/debian/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-06-28 15:14:52.000000 sosse-1.1.0/docker/debian/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.644519 sosse-1.1.0/docker/debian-pkg/
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-06-28 15:14:52.000000 sosse-1.1.0/docker/debian-pkg/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-28 15:14:52.000000 sosse-1.1.0/docker/debian-pkg/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.648519 sosse-1.1.0/docker/debian-test/
--rw-rw-rw-   0 root         (0) root         (0)     1166 2023-06-28 15:14:52.000000 sosse-1.1.0/docker/debian-test/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-06-28 15:14:52.000000 sosse-1.1.0/docker/debian-test/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.648519 sosse-1.1.0/docker/doc/
--rw-rw-rw-   0 root         (0) root         (0)      435 2023-06-28 15:14:52.000000 sosse-1.1.0/docker/doc/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-06-28 15:14:52.000000 sosse-1.1.0/docker/doc/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.648519 sosse-1.1.0/docker/pip-base/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-28 15:14:52.000000 sosse-1.1.0/docker/pip-base/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-28 15:14:52.000000 sosse-1.1.0/docker/pip-base/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.652518 sosse-1.1.0/docker/pip-release/
--rw-rw-rw-   0 root         (0) root         (0)     1405 2023-06-28 15:14:52.000000 sosse-1.1.0/docker/pip-release/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-06-28 15:14:52.000000 sosse-1.1.0/docker/pip-release/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.652518 sosse-1.1.0/docker/pip-test/
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-06-28 15:14:52.000000 sosse-1.1.0/docker/pip-test/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-28 15:14:52.000000 sosse-1.1.0/docker/pip-test/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-06-28 15:14:52.000000 sosse-1.1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-28 15:14:52.000000 sosse-1.1.0/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.668518 sosse-1.1.0/se/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 15:14:52.000000 sosse-1.1.0/se/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20834 2023-06-28 15:14:52.000000 sosse-1.1.0/se/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      996 2023-06-28 15:14:52.000000 sosse-1.1.0/se/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     4121 2023-06-28 15:14:52.000000 sosse-1.1.0/se/atom.py
--rw-rw-rw-   0 root         (0) root         (0)    24375 2023-06-28 15:14:52.000000 sosse-1.1.0/se/browser.py
--rw-rw-rw-   0 root         (0) root         (0)     3135 2023-06-28 15:14:52.000000 sosse-1.1.0/se/cached.py
--rw-rw-rw-   0 root         (0) root         (0)     4314 2023-06-28 15:14:52.000000 sosse-1.1.0/se/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-06-28 15:14:52.000000 sosse-1.1.0/se/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.668518 sosse-1.1.0/se/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 15:14:52.000000 sosse-1.1.0/se/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.672517 sosse-1.1.0/se/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 15:14:52.000000 sosse-1.1.0/se/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4311 2023-06-28 15:14:52.000000 sosse-1.1.0/se/management/commands/crawl.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-06-28 15:14:52.000000 sosse-1.1.0/se/management/commands/default_admin.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-06-28 15:14:52.000000 sosse-1.1.0/se/management/commands/default_conf.py
--rw-rw-rw-   0 root         (0) root         (0)     6143 2023-06-28 15:14:52.000000 sosse-1.1.0/se/management/commands/extract_doc.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2023-06-28 15:14:52.000000 sosse-1.1.0/se/management/commands/generate_secret.py
--rw-rw-rw-   0 root         (0) root         (0)     1746 2023-06-28 15:14:52.000000 sosse-1.1.0/se/management/commands/load_se.py
--rw-rw-rw-   0 root         (0) root         (0)     2150 2023-06-28 15:14:52.000000 sosse-1.1.0/se/management/commands/update_se.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.676517 sosse-1.1.0/se/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    13998 2023-06-28 14:55:25.000000 sosse-1.1.0/se/migrations/0001_initial.py
--rwxrwxrwx   0 root         (0) root         (0)     2976 2023-06-28 14:55:25.000000 sosse-1.1.0/se/migrations/0002_search_vector.py
--rw-rw-rw-   0 root         (0) root         (0)     1143 2023-06-28 14:55:25.000000 sosse-1.1.0/se/migrations/0003_sosse_1_1_0.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 14:55:25.000000 sosse-1.1.0/se/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    55878 2023-06-28 15:14:52.000000 sosse-1.1.0/se/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1974 2023-06-28 15:14:52.000000 sosse-1.1.0/se/screenshot.py
--rw-rw-rw-   0 root         (0) root         (0)     6607 2023-06-28 15:14:52.000000 sosse-1.1.0/se/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.600521 sosse-1.1.0/se/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.684517 sosse-1.1.0/se/static/se/
--rw-rw-rw-   0 root         (0) root         (0)    19511 2023-06-28 15:14:52.000000 sosse-1.1.0/se/static/se/admin-base.css
--rw-rw-rw-   0 root         (0) root         (0)     8810 2023-06-28 15:14:52.000000 sosse-1.1.0/se/static/se/admin-forms.css
--rw-rw-rw-   0 root         (0) root         (0)     2005 2023-06-28 15:14:52.000000 sosse-1.1.0/se/static/se/base.js
--rw-rw-rw-   0 root         (0) root         (0)     2435 2023-06-28 15:14:52.000000 sosse-1.1.0/se/static/se/icon-atom.svg
--rw-rw-rw-   0 root         (0) root         (0)     2196 2023-06-28 15:14:52.000000 sosse-1.1.0/se/static/se/icon-clear.svg
--rw-rw-rw-   0 root         (0) root         (0)     3722 2023-06-28 15:14:52.000000 sosse-1.1.0/se/static/se/icon-cog.svg
--rw-rw-rw-   0 root         (0) root         (0)     6887 2023-06-28 15:14:52.000000 sosse-1.1.0/se/static/se/icon-search.svg
--rw-rw-rw-   0 root         (0) root         (0)     2488 2023-06-28 15:14:52.000000 sosse-1.1.0/se/static/se/icon-stats.svg
--rw-rw-rw-   0 root         (0) root         (0)     3644 2023-06-28 15:14:52.000000 sosse-1.1.0/se/static/se/icon-trash.svg
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-06-28 15:14:52.000000 sosse-1.1.0/se/static/se/icon-user.svg
--rw-rw-rw-   0 root         (0) root         (0)     9798 2023-06-28 15:14:52.000000 sosse-1.1.0/se/static/se/index.js
--rw-rw-rw-   0 root         (0) root         (0)     4462 2023-06-28 15:14:52.000000 sosse-1.1.0/se/static/se/logo.png
--rw-rw-rw-   0 root         (0) root         (0)     9908 2023-06-28 15:14:52.000000 sosse-1.1.0/se/static/se/logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     5967 2023-06-28 15:14:52.000000 sosse-1.1.0/se/static/se/pygal-tooltips.min.js
--rw-rw-rw-   0 root         (0) root         (0)      982 2023-06-28 15:14:52.000000 sosse-1.1.0/se/static/se/screenshot.js
--rw-rw-rw-   0 root         (0) root         (0)     2522 2023-06-28 15:14:52.000000 sosse-1.1.0/se/static/se/style.css
--rw-rw-rw-   0 root         (0) root         (0)     8567 2023-06-28 15:14:52.000000 sosse-1.1.0/se/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.600521 sosse-1.1.0/se/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.688517 sosse-1.1.0/se/templates/admin/
--rw-rw-rw-   0 root         (0) root         (0)     3427 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/admin/add_to_queue.html
--rw-rw-rw-   0 root         (0) root         (0)     2518 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/admin/app_list.html
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/admin/base.html
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/admin/base_site.html
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/admin/change_form.html
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/admin/crawl_status.html
--rw-rw-rw-   0 root         (0) root         (0)     2706 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/admin/crawl_status_content.html
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/admin/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.700516 sosse-1.1.0/se/templates/se/
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/se/about.html
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/se/base.html
--rw-rw-rw-   0 root         (0) root         (0)     2285 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/se/cached.html
--rw-rw-rw-   0 root         (0) root         (0)     1870 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/se/history.html
--rw-rw-rw-   0 root         (0) root         (0)      671 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/se/home_browse.html
--rw-rw-rw-   0 root         (0) root         (0)     9293 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/se/index.html
--rw-rw-rw-   0 root         (0) root         (0)     1320 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/se/main_menu.html
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/se/opensearch.xml
--rw-rw-rw-   0 root         (0) root         (0)      761 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/se/pagination.html
--rw-rw-rw-   0 root         (0) root         (0)     2242 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/se/prefs.html
--rw-rw-rw-   0 root         (0) root         (0)     1706 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/se/screenshot.html
--rw-rw-rw-   0 root         (0) root         (0)     1523 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/se/search_redirect.html
--rw-rw-rw-   0 root         (0) root         (0)     1547 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/se/stats.html
--rw-rw-rw-   0 root         (0) root         (0)      741 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/se/unknown_url.html
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/se/words.html
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-28 15:14:52.000000 sosse-1.1.0/se/templates/se/www.html
--rw-rw-rw-   0 root         (0) root         (0)     5979 2023-06-28 15:14:52.000000 sosse-1.1.0/se/test_cookie.py
--rw-rw-rw-   0 root         (0) root         (0)    14987 2023-06-28 15:14:52.000000 sosse-1.1.0/se/test_crawl.py
--rw-rw-rw-   0 root         (0) root         (0)     9790 2023-06-28 15:14:52.000000 sosse-1.1.0/se/test_functionals.py
--rw-rw-rw-   0 root         (0) root         (0)     1459 2023-06-28 15:14:52.000000 sosse-1.1.0/se/test_misc.py
--rw-rw-rw-   0 root         (0) root         (0)     4659 2023-06-28 15:14:52.000000 sosse-1.1.0/se/test_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2133 2023-06-28 15:14:52.000000 sosse-1.1.0/se/test_redirect.py
--rw-rw-rw-   0 root         (0) root         (0)     1600 2023-06-28 15:14:52.000000 sosse-1.1.0/se/test_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     9547 2023-06-28 15:14:52.000000 sosse-1.1.0/se/test_search.py
--rw-rw-rw-   0 root         (0) root         (0)     2612 2023-06-28 15:14:52.000000 sosse-1.1.0/se/test_url.py
--rw-rw-rw-   0 root         (0) root         (0)     6326 2023-06-28 15:14:52.000000 sosse-1.1.0/se/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)     3101 2023-06-28 15:14:52.000000 sosse-1.1.0/se/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     8615 2023-06-28 15:14:52.000000 sosse-1.1.0/se/views.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-06-28 15:14:52.000000 sosse-1.1.0/se/words.py
--rw-rw-rw-   0 root         (0) root         (0)     2831 2023-06-28 15:14:52.000000 sosse-1.1.0/se/www.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 15:15:25.720515 sosse-1.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.704516 sosse-1.1.0/sosse/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 15:14:52.000000 sosse-1.1.0/sosse/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16942 2023-06-28 15:14:52.000000 sosse-1.1.0/sosse/conf.py
--rw-rw-rw-   0 root         (0) root         (0)    18193 2023-06-28 15:14:52.000000 sosse-1.1.0/sosse/search_engines.json
--rw-rw-rw-   0 root         (0) root         (0)     7433 2023-06-28 15:15:05.000000 sosse-1.1.0/sosse/settings.py
--rwxrwxrwx   0 root         (0) root         (0)     1328 2023-06-28 15:14:52.000000 sosse-1.1.0/sosse/sosse_admin.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-06-28 15:14:52.000000 sosse-1.1.0/sosse/test_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     2548 2023-06-28 15:14:52.000000 sosse-1.1.0/sosse/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-06-28 15:14:52.000000 sosse-1.1.0/sosse/wsgi.py
--rwxrwxrwx   0 root         (0) root         (0)       70 2023-06-28 15:14:52.000000 sosse-1.1.0/sosse-admin
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.708516 sosse-1.1.0/sosse.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3198 2023-06-28 15:15:25.000000 sosse-1.1.0/sosse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4845 2023-06-28 15:15:25.000000 sosse-1.1.0/sosse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 15:15:25.000000 sosse-1.1.0/sosse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-28 15:15:25.000000 sosse-1.1.0/sosse.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      129 2023-06-28 15:15:25.000000 sosse-1.1.0/sosse.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-28 15:15:25.000000 sosse-1.1.0/sosse.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.716515 sosse-1.1.0/tests/
--rwxrwxrwx   0 root         (0) root         (0)      281 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/build_doc.sh
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/cookies.json
--rwxrwxrwx   0 root         (0) root         (0)     1629 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/doc_test.sh
--rwxrwxrwx   0 root         (0) root         (0)      477 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/docker_run.sh
--rw-rw-rw-   0 root         (0) root         (0)     1015 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/document-ja.json
--rw-rw-rw-   0 root         (0) root         (0)      496 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/opensearch.xml
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/release.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.716515 sosse-1.1.0/tests/robotframework/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/robotframework/config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     7309 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/robotframework/home_docs.json
--rw-rw-rw-   0 root         (0) root         (0)    64349 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/robotframework/home_favicon.json
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/robotframework/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      605 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/robotframework/start.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:15:25.720515 sosse-1.1.0/tests/robotframework/tests/
--rw-rw-rw-   0 root         (0) root         (0)     5212 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/robotframework/tests/01_crawl.robot
--rw-rw-rw-   0 root         (0) root         (0)     3334 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/robotframework/tests/02_user.robot
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/robotframework/tests/__init__.robot
--rw-rw-rw-   0 root         (0) root         (0)     1535 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/robotframework/tests/common.robot
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/searchhistory.json
--rwxrwxrwx   0 root         (0) root         (0)      938 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/test_app.sh
--rwxrwxrwx   0 root         (0) root         (0)      101 2023-06-28 15:14:52.000000 sosse-1.1.0/tests/wait_for_pg.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.108817 sosse-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-06-29 14:29:39.000000 sosse-1.1.1/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      351 2023-06-29 14:29:39.000000 sosse-1.1.1/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.036820 sosse-1.1.1/.gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-29 14:29:39.000000 sosse-1.1.1/.gitlab/changelog_config.yml
+-rw-rw-rw-   0 root         (0) root         (0)     6963 2023-06-29 14:29:39.000000 sosse-1.1.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-06-29 14:29:39.000000 sosse-1.1.1/.readthedocs.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-06-29 14:29:39.000000 sosse-1.1.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2023-06-29 14:29:39.000000 sosse-1.1.1/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)    34523 2023-06-29 14:29:39.000000 sosse-1.1.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-29 14:29:39.000000 sosse-1.1.1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     7600 2023-06-29 14:29:39.000000 sosse-1.1.1/Makefile
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-06-29 14:30:06.108817 sosse-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2806 2023-06-29 14:29:39.000000 sosse-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.040820 sosse-1.1.1/debian/
+-rw-rw-rw-   0 root         (0) root         (0)      570 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/changelog
+-rw-rw-rw-   0 root         (0) root         (0)        3 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/compat
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/control
+-rwxrwxrwx   0 root         (0) root         (0)      182 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/rules
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/sosse-crawler.service
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/sosse-uwsgi.service
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/sosse.conf
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/sosse.install
+-rw-rw-rw-   0 root         (0) root         (0)     2733 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/sosse.postinst
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/uwsgi.ini
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/uwsgi.params
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.040820 sosse-1.1.1/doc/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/Makefile
+-rwxrwxrwx   0 root         (0) root         (0)      314 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/build_changelog.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1897 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/get_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.048819 sosse-1.1.1/doc/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.048819 sosse-1.1.1/doc/source/_extensions/
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/_extensions/code_blocks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.048819 sosse-1.1.1/doc/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/_static/style.css
+-rw-rw-rw-   0 root         (0) root         (0)      723 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/admin_ui.rst
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/administration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      502 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/archive.rst
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/authentication.rst
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/cli.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/config_file.rst
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/cookies.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.052819 sosse-1.1.1/doc/source/crawl/
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/crawl/add_to_queue.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/crawl/crawl_depth.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5773 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/crawl/policies.rst
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/crawl/status.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/documents.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1408 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/domain_settings.rst
+-rw-rw-rw-   0 root         (0) root         (0)      315 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/excluded_urls.rst
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.052819 sosse-1.1.1/doc/source/install/
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/install/database.rst.template
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/install/debian.rst
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/install/debian_upgrades.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/install/docker.rst
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/install/docker_upgrades.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3444 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/install/pip.rst
+-rw-rw-rw-   0 root         (0) root         (0)      450 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/install/pip_upgrades.rst
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)      988 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/permissions.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/screenshots.rst
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/search_engines.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.056819 sosse-1.1.1/doc/source/user/
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/user/cached.rst
+-rw-rw-rw-   0 root         (0) root         (0)      593 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/user/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/user/preferences.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/user/search.rst
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/user/shortcut_list.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/user/shortcuts.rst
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/user/statistics.rst
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/user_doc.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.056819 sosse-1.1.1/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/Makefile.common
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.056819 sosse-1.1.1/docker/debian/
+-rw-rw-rw-   0 root         (0) root         (0)     2006 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/debian/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/debian/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.056819 sosse-1.1.1/docker/debian-pkg/
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/debian-pkg/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/debian-pkg/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.060819 sosse-1.1.1/docker/debian-test/
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/debian-test/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/debian-test/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.060819 sosse-1.1.1/docker/doc/
+-rw-rw-rw-   0 root         (0) root         (0)      435 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/doc/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/doc/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.060819 sosse-1.1.1/docker/pip-base/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/pip-base/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/pip-base/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.060819 sosse-1.1.1/docker/pip-release/
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/pip-release/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/pip-release/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.060819 sosse-1.1.1/docker/pip-test/
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/pip-test/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/pip-test/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-06-29 14:29:39.000000 sosse-1.1.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-29 14:29:39.000000 sosse-1.1.1/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.072818 sosse-1.1.1/se/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:29:39.000000 sosse-1.1.1/se/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20834 2023-06-29 14:29:39.000000 sosse-1.1.1/se/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-06-29 14:29:39.000000 sosse-1.1.1/se/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     4121 2023-06-29 14:29:39.000000 sosse-1.1.1/se/atom.py
+-rw-rw-rw-   0 root         (0) root         (0)    24429 2023-06-29 14:29:39.000000 sosse-1.1.1/se/browser.py
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2023-06-29 14:29:39.000000 sosse-1.1.1/se/cached.py
+-rw-rw-rw-   0 root         (0) root         (0)     4314 2023-06-29 14:29:39.000000 sosse-1.1.1/se/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-06-29 14:29:39.000000 sosse-1.1.1/se/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.072818 sosse-1.1.1/se/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.076818 sosse-1.1.1/se/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4311 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/commands/crawl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/commands/default_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/commands/default_conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6143 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/commands/extract_doc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/commands/generate_secret.py
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/commands/load_se.py
+-rw-rw-rw-   0 root         (0) root         (0)     2150 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/commands/update_se.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.076818 sosse-1.1.1/se/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    13998 2023-06-29 14:18:44.000000 sosse-1.1.1/se/migrations/0001_initial.py
+-rwxrwxrwx   0 root         (0) root         (0)     2976 2023-06-29 14:18:44.000000 sosse-1.1.1/se/migrations/0002_search_vector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2023-06-29 14:18:44.000000 sosse-1.1.1/se/migrations/0003_sosse_1_1_0.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:18:44.000000 sosse-1.1.1/se/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    56021 2023-06-29 14:29:39.000000 sosse-1.1.1/se/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2023-06-29 14:29:39.000000 sosse-1.1.1/se/screenshot.py
+-rw-rw-rw-   0 root         (0) root         (0)     6607 2023-06-29 14:29:39.000000 sosse-1.1.1/se/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.028820 sosse-1.1.1/se/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.084818 sosse-1.1.1/se/static/se/
+-rw-rw-rw-   0 root         (0) root         (0)    19511 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/admin-base.css
+-rw-rw-rw-   0 root         (0) root         (0)     8810 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/admin-forms.css
+-rw-rw-rw-   0 root         (0) root         (0)     2005 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/base.js
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/icon-atom.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/icon-clear.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3722 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/icon-cog.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/icon-search.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/icon-stats.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3644 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/icon-trash.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/icon-user.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9798 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/index.js
+-rw-rw-rw-   0 root         (0) root         (0)     4462 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/logo.png
+-rw-rw-rw-   0 root         (0) root         (0)     9908 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     5967 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/pygal-tooltips.min.js
+-rw-rw-rw-   0 root         (0) root         (0)      982 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/screenshot.js
+-rw-rw-rw-   0 root         (0) root         (0)     2522 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/style.css
+-rw-rw-rw-   0 root         (0) root         (0)     8567 2023-06-29 14:29:39.000000 sosse-1.1.1/se/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.028820 sosse-1.1.1/se/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.084818 sosse-1.1.1/se/templates/admin/
+-rw-rw-rw-   0 root         (0) root         (0)     3427 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/admin/add_to_queue.html
+-rw-rw-rw-   0 root         (0) root         (0)     2518 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/admin/app_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/admin/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/admin/base_site.html
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/admin/change_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/admin/crawl_status.html
+-rw-rw-rw-   0 root         (0) root         (0)     2706 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/admin/crawl_status_content.html
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/admin/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.092817 sosse-1.1.1/se/templates/se/
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/about.html
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/base.html
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/cached.html
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/history.html
+-rw-rw-rw-   0 root         (0) root         (0)      671 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/home_browse.html
+-rw-rw-rw-   0 root         (0) root         (0)     9293 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     1320 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/main_menu.html
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/opensearch.xml
+-rw-rw-rw-   0 root         (0) root         (0)      761 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/pagination.html
+-rw-rw-rw-   0 root         (0) root         (0)     2242 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/prefs.html
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/screenshot.html
+-rw-rw-rw-   0 root         (0) root         (0)     1523 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/search_redirect.html
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/stats.html
+-rw-rw-rw-   0 root         (0) root         (0)      741 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/unknown_url.html
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/words.html
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/www.html
+-rw-rw-rw-   0 root         (0) root         (0)     5979 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_cookie.py
+-rw-rw-rw-   0 root         (0) root         (0)    14987 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_crawl.py
+-rw-rw-rw-   0 root         (0) root         (0)     9790 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_functionals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1459 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4659 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2133 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_redirect.py
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     9547 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_search.py
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_url.py
+-rw-rw-rw-   0 root         (0) root         (0)     6326 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     3101 2023-06-29 14:29:39.000000 sosse-1.1.1/se/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     8615 2023-06-29 14:29:39.000000 sosse-1.1.1/se/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-06-29 14:29:39.000000 sosse-1.1.1/se/words.py
+-rw-rw-rw-   0 root         (0) root         (0)     2831 2023-06-29 14:29:39.000000 sosse-1.1.1/se/www.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 14:30:06.108817 sosse-1.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.096817 sosse-1.1.1/sosse/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:29:39.000000 sosse-1.1.1/sosse/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16990 2023-06-29 14:29:39.000000 sosse-1.1.1/sosse/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)    18193 2023-06-29 14:29:39.000000 sosse-1.1.1/sosse/search_engines.json
+-rw-rw-rw-   0 root         (0) root         (0)     7433 2023-06-29 14:29:49.000000 sosse-1.1.1/sosse/settings.py
+-rwxrwxrwx   0 root         (0) root         (0)     1328 2023-06-29 14:29:39.000000 sosse-1.1.1/sosse/sosse_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-06-29 14:29:39.000000 sosse-1.1.1/sosse/test_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2548 2023-06-29 14:29:39.000000 sosse-1.1.1/sosse/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-06-29 14:29:39.000000 sosse-1.1.1/sosse/wsgi.py
+-rwxrwxrwx   0 root         (0) root         (0)       70 2023-06-29 14:29:39.000000 sosse-1.1.1/sosse-admin
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.100817 sosse-1.1.1/sosse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-06-29 14:30:05.000000 sosse-1.1.1/sosse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4845 2023-06-29 14:30:06.000000 sosse-1.1.1/sosse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 14:30:05.000000 sosse-1.1.1/sosse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-29 14:30:05.000000 sosse-1.1.1/sosse.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      129 2023-06-29 14:30:05.000000 sosse-1.1.1/sosse.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-29 14:30:05.000000 sosse-1.1.1/sosse.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.104817 sosse-1.1.1/tests/
+-rwxrwxrwx   0 root         (0) root         (0)      281 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/build_doc.sh
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/cookies.json
+-rwxrwxrwx   0 root         (0) root         (0)     1629 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/doc_test.sh
+-rwxrwxrwx   0 root         (0) root         (0)      477 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/docker_run.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1015 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/document-ja.json
+-rw-rw-rw-   0 root         (0) root         (0)      496 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/opensearch.xml
+-rw-rw-rw-   0 root         (0) root         (0)      898 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/release.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.108817 sosse-1.1.1/tests/robotframework/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     7309 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/home_docs.json
+-rw-rw-rw-   0 root         (0) root         (0)    64349 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/home_favicon.json
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      605 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/start.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.108817 sosse-1.1.1/tests/robotframework/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5212 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/tests/01_crawl.robot
+-rw-rw-rw-   0 root         (0) root         (0)     3334 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/tests/02_user.robot
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/tests/__init__.robot
+-rw-rw-rw-   0 root         (0) root         (0)     1583 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/tests/common.robot
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/searchhistory.json
+-rwxrwxrwx   0 root         (0) root         (0)      938 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/test_app.sh
+-rwxrwxrwx   0 root         (0) root         (0)      101 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/wait_for_pg.sh
```

### Comparing `sosse-1.1.0/.gitlab-ci.yml` & `sosse-1.1.1/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         coverage_format: cobertura
         path: coverage.xml
   script:
     - /etc/init.d/postgresql start
     - mkdir -p /var/lib/sosse/screenshots/ /var/lib/sosse/downloads/0 && chown -R www-data:www-data /var/lib/sosse/
     - /usr/bin/python3 /root/httpbin/httpbin/manage.py runserver 0.0.0.0:8000 &
     - export PYTHONPATH="$CI_PROJECT_DIR"
-    - /tmp/sudo_sosse default_conf | sed -e "s/^#debug=.*/debug=true/" -e "s/^#browser_options=\(.*\)/browser_options=\1 --no-sandbox/" -e "s/#dl_check_time=.*/dl_check_time=1/" > /etc/sosse/sosse.conf
+    - /tmp/sudo_sosse default_conf | sed -e "s/^#debug=.*/debug=true/" -e "s/^#browser_options=\(.*\)/browser_options=\1 --no-sandbox --disable-dev-shm-usage/" -e "s/#dl_check_time=.*/dl_check_time=1/" > /etc/sosse/sosse.conf
     - /tmp/sudo_sosse test -v3 --failfast
     - /tmp/sudo_sosse load_se tests/opensearch.xml
     - /tmp/sudo_sosse update_se
     - /tmp/sudo_sosse shell -c 'from django.contrib.auth.models import User; User.objects.all().delete()'
     - /tmp/sudo_sosse default_admin
     - /tmp/sudo_sosse generate_secret
     - /tmp/sudo_sosse extract_doc cli > /dev/null
```

### Comparing `sosse-1.1.0/CHANGELOG.md` & `sosse-1.1.1/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.1.1 (2023-06-29)
+### Bug fixes (1 change)
+- [misc Bookworm, Docker and Selenium fixes](biolds1/sosse@54fcc7043bfc34a6125fa301d58c08ea02e0b292) ([merge request](biolds1/sosse!12))
+
 ## 1.1.0 (2023-06-18)
 ### Features (3 changes)
 - [Debian Bookworm support](biolds1/sosse@b2112e5a0a526e777600499d726002ad62612aac) ([merge request](biolds1/sosse!10))
 - [browsable archive on homepage view](biolds1/sosse@f3f2c065f63ada182e0f6154b5586dcae1ea5158) ([merge request](biolds1/sosse!8))
 - [automatically follow redirection in cached pages](biolds1/sosse@5d2a40ef0d253a5e47746d25d725794d58216cb2) ([merge request](biolds1/sosse!7))
 ### Bug fixes (2 changes)
 - [fix resolving links when the header has a <base> tag](biolds1/sosse@ff6d4f2d33d6395be87c026c5c9f87c457d5f1a7) ([merge request](biolds1/sosse!6))
```

### Comparing `sosse-1.1.0/Dockerfile` & `sosse-1.1.1/Dockerfile`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ADD MANIFEST.in .
 ADD se/ se/
 ADD sosse/ sosse/
 RUN virtualenv /venv
 RUN /venv/bin/pip install ./ && /venv/bin/pip install uwsgi && /venv/bin/pip cache purge
 ADD debian/sosse.conf /etc/nginx/sites-enabled/default
 RUN mkdir -p /etc/sosse/ /etc/sosse_src/ /var/log/sosse /var/log/uwsgi
-RUN /venv/bin/sosse-admin default_conf | sed -e 's/^#db_pass.*/db_pass=sosse/' -e 's/^#\(browser_options=.*\)$/\1 --no-sandbox/' > /etc/sosse_src/sosse.conf
+RUN /venv/bin/sosse-admin default_conf | sed -e 's/^#db_pass.*/db_pass=sosse/' -e 's/^#\(browser_options=.*\)$/\1 --no-sandbox --disable-dev-shm-usage/' > /etc/sosse_src/sosse.conf
 ADD debian/uwsgi.* /etc/sosse_src/
 RUN chown -R root:www-data /etc/sosse /etc/sosse_src && chmod 750 /etc/sosse_src/ && chmod 640 /etc/sosse_src/*
 
 WORKDIR /
 USER postgres
 RUN /etc/init.d/postgresql start && \
     psql --command "CREATE USER sosse WITH PASSWORD 'sosse';" && \
```

### Comparing `sosse-1.1.0/LICENSE` & `sosse-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/Makefile` & `sosse-1.1.1/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -118,26 +118,26 @@
 	grep -q 'pip install sosse' /tmp/code_blocks.json
 	sed -e 's#pip install sosse#pip install dist/*.whl#' -i /tmp/code_blocks.json
 	bash ./tests/doc_test.sh /tmp/code_blocks.json install/pip
 
 _common_pip_functional_tests:
 	cp doc/code_blocks.json /tmp/code_blocks.json
 	grep -q 'sosse-admin default_conf' /tmp/code_blocks.json
-	sed -e 's#sosse-admin default_conf#sosse-admin default_conf | sed -e \\"s/^.browser_options=.*/browser_options=--enable-precise-memory-info --disable-default-apps --incognito --headless --no-sandbox/\\" -e \\"s/^.browser_crash_retry=.*/browser_crash_retry=3/\\" -e \\"s/^.crawler_count=.*/crawler_count=1/\\" -e \\"s/^.debug=.*/debug=true/\\"#' -i /tmp/code_blocks.json # add --no-sandbox to chromium's command line
+	sed -e 's#sosse-admin default_conf#sosse-admin default_conf | sed -e \\"s/^.browser_options=.*/browser_options=--enable-precise-memory-info --disable-default-apps --incognito --headless --no-sandbox --disable-dev-shm-usage/\\" -e \\"s/^.browser_crash_retry=.*/browser_crash_retry=3/\\" -e \\"s/^.crawler_count=.*/crawler_count=1/\\" -e \\"s/^.debug=.*/debug=true/\\"#' -i /tmp/code_blocks.json # add --no-sandbox --disable-dev-shm-usage to chromium's command line
 	echo 'SOSSE_ADMIN: /opt/sosse-venv/bin/sosse-admin' > tests/robotframework/config.yaml
 
 _deb_pkg_functional_tests:
 	grep ^Depends: debian/control | sed -e "s/.*},//" -e "s/,//g" | xargs apt install -y
 	grep '^ExecStartPre=' debian/sosse-uwsgi.service | sed -e 's/^ExecStartPre=-\?+\?//' -e 's/^/---- /'
 	bash -c "`grep '^ExecStartPre=' debian/sosse-uwsgi.service | sed -e 's/^ExecStartPre=-\?+\?//'`"
 	cp doc/code_blocks.json /tmp/code_blocks.json
 	grep -q 'apt install -y sosse' /tmp/code_blocks.json
 	sed -e 's#apt install -y sosse#apt install -y sudo; dpkg -i deb/*.deb ; /etc/init.d/postgresql start \& bash ./tests/wait_for_pg.sh#' -i /tmp/code_blocks.json
 	bash ./tests/doc_test.sh /tmp/code_blocks.json install/debian
-	sed -e 's/^.browser_options=.*/browser_options=--enable-precise-memory-info --disable-default-apps --incognito --headless --no-sandbox/' -i /etc/sosse/sosse.conf # add --no-sandbox to chromium's command line
+	sed -e 's/^.browser_options=.*/browser_options=--enable-precise-memory-info --disable-default-apps --incognito --headless --no-sandbox --disable-dev-shm-usage/' -i /etc/sosse/sosse.conf # add --no-sandbox --disable-dev-shm-usage to chromium's command line
 	sed -e 's/^.browser_crash_retry=.*/browser_crash_retry=3/' -i /etc/sosse/sosse.conf
 	sed -e 's/^.debug=.*/debug=true/' -i /etc/sosse/sosse.conf
 	sed -e 's/^.crawler_count=.*/crawler_count=1/' -i /etc/sosse/sosse.conf
 	/etc/init.d/nginx start
 	bash -c 'uwsgi --uid www-data --gid www-data --plugin python3 --ini /etc/sosse/uwsgi.ini --logto /var/log/sosse/uwsgi.log & sudo -u www-data sosse-admin crawl &'
 	bash ./tests/docker_run.sh docker/pip-test/Dockerfile
```

### Comparing `sosse-1.1.0/PKG-INFO` & `sosse-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosse
-Version: 1.1.0
+Version: 1.1.1
 Summary: Selenium Open Source Search Engine
 Author-email: Laurent Defert <laurent_defert@yahoo.fr>
 License: GNU Affero General Public License v3
 Keywords: search engine,crawler
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sosse Version: 1.1.0 Summary: Selenium Open Source
+Metadata-Version: 2.1 Name: sosse Version: 1.1.1 Summary: Selenium Open Source
 Search Engine Author-email: Laurent Defert
 yahoo.fr> License: GNU Affero General Public License v3 Keywords: search
 engine,crawler Classifier: Framework :: Django Classifier: Programming Language
 :: Python :: 3 Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE
 [https://raw.githubusercontent.com/biolds/sosse/main/se/static/se/logo.svg]
 [https://img.shields.io/gitlab/pipeline-coverage/biolds1/
```

### Comparing `sosse-1.1.0/README.md` & `sosse-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/debian/control` & `sosse-1.1.1/debian/control`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/debian/sosse-crawler.service` & `sosse-1.1.1/debian/sosse-crawler.service`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/debian/sosse-uwsgi.service` & `sosse-1.1.1/debian/sosse-uwsgi.service`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/debian/sosse.conf` & `sosse-1.1.1/debian/sosse.conf`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/debian/sosse.postinst` & `sosse-1.1.1/debian/sosse.postinst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/debian/uwsgi.params` & `sosse-1.1.1/debian/uwsgi.params`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/Makefile` & `sosse-1.1.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/get_artifacts.py` & `sosse-1.1.1/doc/get_artifacts.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/make.bat` & `sosse-1.1.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/_extensions/code_blocks.py` & `sosse-1.1.1/doc/source/_extensions/code_blocks.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/admin_ui.rst` & `sosse-1.1.1/doc/source/admin_ui.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/authentication.rst` & `sosse-1.1.1/doc/source/authentication.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/conf.py` & `sosse-1.1.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/crawl/add_to_queue.rst` & `sosse-1.1.1/doc/source/crawl/add_to_queue.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/crawl/crawl_depth.rst` & `sosse-1.1.1/doc/source/crawl/crawl_depth.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/crawl/policies.rst` & `sosse-1.1.1/doc/source/crawl/policies.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/documents.rst` & `sosse-1.1.1/doc/source/documents.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/domain_settings.rst` & `sosse-1.1.1/doc/source/domain_settings.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/index.rst` & `sosse-1.1.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/install/database.rst.template` & `sosse-1.1.1/doc/source/install/database.rst.template`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/install/debian.rst` & `sosse-1.1.1/doc/source/install/debian.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/install/docker.rst` & `sosse-1.1.1/doc/source/install/docker.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/install/pip.rst` & `sosse-1.1.1/doc/source/install/pip.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/permissions.rst` & `sosse-1.1.1/doc/source/permissions.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/screenshots.rst` & `sosse-1.1.1/doc/source/screenshots.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/search_engines.rst` & `sosse-1.1.1/doc/source/search_engines.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/user/cached.rst` & `sosse-1.1.1/doc/source/user/cached.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/user/history.rst` & `sosse-1.1.1/doc/source/user/history.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/user/preferences.rst` & `sosse-1.1.1/doc/source/user/preferences.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/user/search.rst` & `sosse-1.1.1/doc/source/user/search.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/doc/source/user/shortcuts.rst` & `sosse-1.1.1/doc/source/user/shortcuts.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/docker/Makefile` & `sosse-1.1.1/docker/Makefile`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/docker/debian/Dockerfile` & `sosse-1.1.1/docker/debian/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 RUN apt install -y sosse && \
         apt-get clean autoclean && \
         apt-get autoremove --yes && \
         rm -rf /var/lib/cache /var/lib/log /usr/share/doc /usr/share/man
 
 RUN sosse-admin default_conf > /etc/sosse/sosse.conf
 RUN chown -R root:www-data /etc/sosse && chmod 750 /etc/sosse/ && chmod 640 /etc/sosse/*
-RUN sed -e 's/^#\(browser_options=.*\)$/\1 --no-sandbox/' -i /etc/sosse/sosse.conf
+RUN sed -e 's/^#\(browser_options=.*\)$/\1 --no-sandbox --disable-dev-shm-usage/' -i /etc/sosse/sosse.conf
 RUN rm /etc/nginx/sites-enabled/default
 RUN ln -s /etc/nginx/sites-available/sosse.conf /etc/nginx/sites-enabled/
 
 WORKDIR /
 USER postgres
 RUN echo "listen_addresses='127.0.0.1'" >> /etc/postgresql/15/main/postgresql.conf
 RUN /etc/init.d/postgresql start && \
@@ -37,13 +37,13 @@
 RUN echo '#!/bin/bash -x \n \
 /etc/init.d/postgresql start \n \
 mkdir -p /run/sosse \n \
 chown -R www-data:www-data /run/sosse \n \
 sosse-admin migrate \n \
 sosse-admin update_se \n \
 sosse-admin collectstatic --noinput \n \
-/usr/bin/uwsgi --uid www-data --gid www-data --ini /etc/sosse/uwsgi.ini & \n \
+/usr/bin/uwsgi --uid www-data --gid www-data --plugin python3 --ini /etc/sosse/uwsgi.ini & \n \
 /etc/init.d/nginx start \n \
 sosse-admin crawl & \n \
 tail -F /var/log/sosse/crawler.log' > /run.sh ; chmod +x /run.sh
 RUN test -z "$APT_PROXY" || rm /etc/apt/apt.conf.d/proxy.conf
 CMD /run.sh
```

### Comparing `sosse-1.1.0/docker/debian-pkg/Dockerfile` & `sosse-1.1.1/docker/debian-pkg/Dockerfile`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/docker/debian-test/Dockerfile` & `sosse-1.1.1/docker/debian-test/Dockerfile`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/docker/pip-release/Dockerfile` & `sosse-1.1.1/docker/pip-release/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 FROM biolds/sosse:pip-base
 ARG PIP_INDEX_URL=
 ARG PIP_TRUSTED_HOST=
 RUN virtualenv /venv
 RUN /venv/bin/pip install sosse uwsgi && /venv/bin/pip cache purge
 RUN mkdir -p /etc/sosse/ /etc/sosse_src/ /var/log/sosse /var/log/uwsgi
-RUN sosse-admin default_conf | sed -e 's/^#db_pass.*/db_pass=sosse/' -e 's/^#\(browser_options=.*\)$/\1 --no-sandbox/' > /etc/sosse_src/sosse.conf
+RUN /venv/bin/sosse-admin default_conf | sed -e 's/^#db_pass.*/db_pass=sosse/' -e 's/^#\(browser_options=.*\)$/\1 --no-sandbox --disable-dev-shm-usage/' > /etc/sosse_src/sosse.conf
 ADD uwsgi.* /etc/sosse_src/
 ADD sosse.conf /etc/nginx/sites-enabled/default
 RUN chown -R root:www-data /etc/sosse /etc/sosse_src && chmod 750 /etc/sosse_src/ && chmod 640 /etc/sosse_src/*
 
 WORKDIR /
 USER postgres
 RUN /etc/init.d/postgresql start && \
@@ -18,16 +18,16 @@
 USER root
 RUN echo '#!/bin/bash -x \n \
 /etc/init.d/postgresql start \n \
 test -e /etc/sosse/sosse.conf || (cp -p /etc/sosse_src/* /etc/sosse/) \n \
 mkdir -p /run/sosse \n \
 touch /var/log/sosse/{debug.log,main.log,crawler.log,uwsgi.log,webserver.log} \n \
 chown -R www-data:www-data /run/sosse /var/log/sosse/ \n \
-sosse-admin migrate \n \
-sosse-admin collectstatic --noinput \n \
-sosse-admin update_se \n \
-sosse-admin default_admin \n \
+/venv/bin/sosse-admin migrate \n \
+/venv/bin/sosse-admin collectstatic --noinput \n \
+/venv/bin/sosse-admin update_se \n \
+/venv/bin/sosse-admin default_admin \n \
 /venv/bin/uwsgi --uid www-data --gid www-data --ini /etc/sosse/uwsgi.ini --logto /var/log/sosse/uwsgi.log & \n \
 /etc/init.d/nginx start \n \
-sosse-admin crawl & \n \
+/venv/bin/sosse-admin crawl & \n \
 tail -F /var/log/sosse/crawler.log' > /run.sh ; chmod +x /run.sh
 CMD /run.sh
```

### Comparing `sosse-1.1.0/docker/pip-test/Dockerfile` & `sosse-1.1.1/docker/pip-test/Dockerfile`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/pyproject.toml` & `sosse-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/admin.py` & `sosse-1.1.1/se/admin.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/apps.py` & `sosse-1.1.1/se/apps.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/atom.py` & `sosse-1.1.1/se/atom.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/browser.py` & `sosse-1.1.1/se/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 from bs4 import BeautifulSoup
 from django.conf import settings
 import requests
 from selenium import webdriver
 from selenium.common.exceptions import WebDriverException
 from selenium.webdriver.chrome.options import Options
+from urllib3.exceptions import HTTPError
 
 
 crawl_logger = logging.getLogger('crawler')
 
 
 class AuthElemFailed(Exception):
     def __init__(self, page, *args, **kwargs):
@@ -313,15 +314,15 @@
     def _retry(*args, **kwargs):
         count = 0
         while count <= settings.SOSSE_BROWSER_CRASH_RETRY:
             try:
                 r = f(*args, **kwargs)
                 crawl_logger.debug('%s succeeded' % f)
                 return r
-            except WebDriverException:
+            except (WebDriverException, HTTPError):
                 exc = traceback.format_exc()
                 crawl_logger.error('%s failed' % f)
                 crawl_logger.error('Selenium returned an exception:\n%s' % exc)
 
                 cls = args[0]
                 cls.destroy()
                 sleep(settings.SOSSE_BROWSER_CRASH_SLEEP)
```

### Comparing `sosse-1.1.0/se/cached.py` & `sosse-1.1.1/se/cached.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/forms.py` & `sosse-1.1.1/se/forms.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/login.py` & `sosse-1.1.1/se/login.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/management/commands/crawl.py` & `sosse-1.1.1/se/management/commands/crawl.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/management/commands/default_admin.py` & `sosse-1.1.1/se/management/commands/default_admin.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/management/commands/default_conf.py` & `sosse-1.1.1/se/management/commands/default_conf.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/management/commands/extract_doc.py` & `sosse-1.1.1/se/management/commands/extract_doc.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/management/commands/generate_secret.py` & `sosse-1.1.1/se/management/commands/generate_secret.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/management/commands/load_se.py` & `sosse-1.1.1/se/management/commands/load_se.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/management/commands/update_se.py` & `sosse-1.1.1/se/management/commands/update_se.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/migrations/0001_initial.py` & `sosse-1.1.1/se/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/migrations/0002_search_vector.py` & `sosse-1.1.1/se/migrations/0002_search_vector.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/migrations/0003_sosse_1_1_0.py` & `sosse-1.1.1/se/migrations/0003_sosse_1_1_0.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/models.py` & `sosse-1.1.1/se/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,17 @@
 
         beautified_url = url_beautify(page.url)
         normalized_url = beautified_url.split('://', 1)[1].replace('/', ' ').strip()
         self.normalized_url = remove_accent(normalized_url)
 
         # dirty hack to avoid some errors (as triggered since bookworm during tests)
         magic_head = page.content[:10].strip().lower()
-        if magic_head.startswith('<html'):
+        is_html = isinstance(magic_head, str) and magic_head.startswith('<html')
+        is_html |= isinstance(magic_head, bytes) and magic_head.startswith(b'<html')
+        if is_html:
             self.mimetype = 'text/html'
         else:
             from magic import from_buffer as magic_from_buffer
             self.mimetype = magic_from_buffer(page.content, mime=True)
 
         if not re.match(crawl_policy.mimetype_regex, self.mimetype):
             crawl_logger.debug('skipping %s due to mimetype %s' % (self.url, self.mimetype))
```

### Comparing `sosse-1.1.0/se/screenshot.py` & `sosse-1.1.1/se/screenshot.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/search.py` & `sosse-1.1.1/se/search.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/static/se/admin-base.css` & `sosse-1.1.1/se/static/se/admin-base.css`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/static/se/admin-forms.css` & `sosse-1.1.1/se/static/se/admin-forms.css`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/static/se/base.js` & `sosse-1.1.1/se/static/se/base.js`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/static/se/icon-atom.svg` & `sosse-1.1.1/se/static/se/icon-atom.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/static/se/icon-clear.svg` & `sosse-1.1.1/se/static/se/icon-clear.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/static/se/icon-cog.svg` & `sosse-1.1.1/se/static/se/icon-cog.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/static/se/icon-search.svg` & `sosse-1.1.1/se/static/se/icon-search.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/static/se/icon-stats.svg` & `sosse-1.1.1/se/static/se/icon-stats.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/static/se/icon-trash.svg` & `sosse-1.1.1/se/static/se/icon-trash.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/static/se/icon-user.svg` & `sosse-1.1.1/se/static/se/icon-user.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/static/se/index.js` & `sosse-1.1.1/se/static/se/index.js`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/static/se/logo.png` & `sosse-1.1.1/se/static/se/logo.png`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/static/se/logo.svg` & `sosse-1.1.1/se/static/se/logo.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/static/se/pygal-tooltips.min.js` & `sosse-1.1.1/se/static/se/pygal-tooltips.min.js`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/static/se/screenshot.js` & `sosse-1.1.1/se/static/se/screenshot.js`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/static/se/style.css` & `sosse-1.1.1/se/static/se/style.css`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/stats.py` & `sosse-1.1.1/se/stats.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/admin/add_to_queue.html` & `sosse-1.1.1/se/templates/admin/add_to_queue.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/admin/app_list.html` & `sosse-1.1.1/se/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/admin/base.html` & `sosse-1.1.1/se/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/admin/change_form.html` & `sosse-1.1.1/se/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/admin/crawl_status.html` & `sosse-1.1.1/se/templates/admin/crawl_status.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/admin/crawl_status_content.html` & `sosse-1.1.1/se/templates/admin/crawl_status_content.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/se/about.html` & `sosse-1.1.1/se/templates/se/about.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/se/base.html` & `sosse-1.1.1/se/templates/se/base.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/se/cached.html` & `sosse-1.1.1/se/templates/se/cached.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/se/history.html` & `sosse-1.1.1/se/templates/se/history.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/se/home_browse.html` & `sosse-1.1.1/se/templates/se/home_browse.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/se/index.html` & `sosse-1.1.1/se/templates/se/index.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/se/main_menu.html` & `sosse-1.1.1/se/templates/se/main_menu.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/se/opensearch.xml` & `sosse-1.1.1/se/templates/se/opensearch.xml`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/se/pagination.html` & `sosse-1.1.1/se/templates/se/pagination.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/se/prefs.html` & `sosse-1.1.1/se/templates/se/prefs.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/se/screenshot.html` & `sosse-1.1.1/se/templates/se/screenshot.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/se/search_redirect.html` & `sosse-1.1.1/se/templates/se/search_redirect.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/se/stats.html` & `sosse-1.1.1/se/templates/se/stats.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/templates/se/unknown_url.html` & `sosse-1.1.1/se/templates/se/unknown_url.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/test_cookie.py` & `sosse-1.1.1/se/test_cookie.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/test_crawl.py` & `sosse-1.1.1/se/test_crawl.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/test_functionals.py` & `sosse-1.1.1/se/test_functionals.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/test_misc.py` & `sosse-1.1.1/se/test_misc.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/test_parser.py` & `sosse-1.1.1/se/test_parser.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/test_redirect.py` & `sosse-1.1.1/se/test_redirect.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/test_requests.py` & `sosse-1.1.1/se/test_requests.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/test_search.py` & `sosse-1.1.1/se/test_search.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/test_url.py` & `sosse-1.1.1/se/test_url.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/test_views.py` & `sosse-1.1.1/se/test_views.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/utils.py` & `sosse-1.1.1/se/utils.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/views.py` & `sosse-1.1.1/se/views.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/words.py` & `sosse-1.1.1/se/words.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/se/www.py` & `sosse-1.1.1/se/www.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/sosse/conf.py` & `sosse-1.1.1/sosse/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
             'default': 'md5'
         }],
         ['screenshots_size', {
             'comment': 'Resolution of the browser used to take screenshots.',
             'default': '1920x1080'
         }],
         ['browser_options', {
-            'comment': "Options passed to Chromium's command line.\nYou may need to add ``--no-sandbox`` to run the crawler in a virtualized container.",
+            'comment': "Options passed to Chromium's command line.\nYou may need to add ``--no-sandbox`` to run the crawler as root,\nor ``--disable-dev-shm-usage`` to run in a virtualized container.",
             'default': '--enable-precise-memory-info --disable-default-apps --incognito --headless'
         }],
         ['js_stable_time', {
             'comment': 'When loading a page in a browser, wait ``js_stable_time`` seconds before checking the DOM stays unchanged.',
             'default': 0.1,
             'type': float
         }],
```

### Comparing `sosse-1.1.0/sosse/search_engines.json` & `sosse-1.1.1/sosse/search_engines.json`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/sosse/settings.py` & `sosse-1.1.1/sosse/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,9 +325,9 @@
         'name': 'chinese',
         'flag': '🇹🇼'
     }
 }
 
 globals().update(Conf.get())
 
-SOSSE_VERSION_TAG = '1.1.0'
-SOSSE_VERSION_COMMIT = '46ea944e'
+SOSSE_VERSION_TAG = '1.1.1'
+SOSSE_VERSION_COMMIT = '828424d6'
```

### Comparing `sosse-1.1.0/sosse/sosse_admin.py` & `sosse-1.1.1/sosse/sosse_admin.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/sosse/urls.py` & `sosse-1.1.1/sosse/urls.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/sosse/wsgi.py` & `sosse-1.1.1/sosse/wsgi.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/sosse.egg-info/PKG-INFO` & `sosse-1.1.1/sosse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosse
-Version: 1.1.0
+Version: 1.1.1
 Summary: Selenium Open Source Search Engine
 Author-email: Laurent Defert <laurent_defert@yahoo.fr>
 License: GNU Affero General Public License v3
 Keywords: search engine,crawler
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sosse Version: 1.1.0 Summary: Selenium Open Source
+Metadata-Version: 2.1 Name: sosse Version: 1.1.1 Summary: Selenium Open Source
 Search Engine Author-email: Laurent Defert
 yahoo.fr> License: GNU Affero General Public License v3 Keywords: search
 engine,crawler Classifier: Framework :: Django Classifier: Programming Language
 :: Python :: 3 Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE
 [https://raw.githubusercontent.com/biolds/sosse/main/se/static/se/logo.svg]
 [https://img.shields.io/gitlab/pipeline-coverage/biolds1/
```

### Comparing `sosse-1.1.0/sosse.egg-info/SOURCES.txt` & `sosse-1.1.1/sosse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/tests/cookies.json` & `sosse-1.1.1/tests/cookies.json`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/tests/doc_test.sh` & `sosse-1.1.1/tests/doc_test.sh`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/tests/document-ja.json` & `sosse-1.1.1/tests/document-ja.json`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/tests/release.md` & `sosse-1.1.1/tests/release.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 - debian update: version + changelog
 - doc version update
 - build and update the CHANGELOG.md
 - MR
 - create tag "vX.X.X"
+- update the `stable` branch for the release (to update the `stable` version of readthedoc)
 - pip release (this needs to be done before the docker step below)
   - clear `dist/`
   - download the artifacts of the `pip_pkg` step and unzip it in the root (it creates `dist/` with packages)
   - run `make pip_pkg_push`
 - debian packages
   - wget `<pkg url>`
   - cd /var/www/html/repo/apt/debian/
-  - reprepro -V --keepunreferencedfiles includedeb bullseye `<path to the .deb>`
+  - reprepro -V --keepunreferencedfiles includedeb bookworm `<path to the .deb>`
 - docker build:
   - clear pip caches
   - make docker_release_build APT_PROXY=http://192.168.1.24:3142/ PIP_INDEX_URL=http://192.168.3.3:5000/index/ PIP_TRUSTED_HOST=192.168.3.3
   - test
   - make docker_release_push
   - docker tag biolds/sosse:latest biolds/sosse:X.X.X
   - docker push biolds/sosse:X.X.X
```

### Comparing `sosse-1.1.0/tests/robotframework/home_docs.json` & `sosse-1.1.1/tests/robotframework/home_docs.json`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/tests/robotframework/home_favicon.json` & `sosse-1.1.1/tests/robotframework/home_favicon.json`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/tests/robotframework/start.sh` & `sosse-1.1.1/tests/robotframework/start.sh`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/tests/robotframework/tests/01_crawl.robot` & `sosse-1.1.1/tests/robotframework/tests/01_crawl.robot`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/tests/robotframework/tests/02_user.robot` & `sosse-1.1.1/tests/robotframework/tests/02_user.robot`

 * *Files identical despite different names*

### Comparing `sosse-1.1.0/tests/robotframework/tests/common.robot` & `sosse-1.1.1/tests/robotframework/tests/common.robot`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 | *Settings* |
 | Library | Process
 
 | *Keywords* |
 | Login
 |  | Open Browser | http://127.0.0.1/ | browser=Firefox |  options=add_argument("--headless")
-#|  | Open Browser | http://127.0.0.1/ | browser=Chrome | options=add_argument("--no-sandbox");add_argument("--headless");add_argument('--enable-precise-memory-info');add_argument('--disable-default-apps')
+#|  | Open Browser | http://127.0.0.1/ | browser=Chrome | options=add_argument("--no-sandbox");options=add_argument("--disable-dev-shm-usage");add_argument("--headless");add_argument('--enable-precise-memory-info');add_argument('--disable-default-apps')
 |  | Set Window Size | 1024 | 768
 |  | Set Screenshot Directory | screenshots/
 |  | Input Text | id=id_username | admin
 |  | Input Text | id=id_password | admin
 |  | Click Element | xpath=//form[@id='login-form']//input[@type='submit']
```

### Comparing `sosse-1.1.0/tests/test_app.sh` & `sosse-1.1.1/tests/test_app.sh`

 * *Files identical despite different names*

