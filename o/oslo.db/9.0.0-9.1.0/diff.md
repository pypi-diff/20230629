# Comparing `tmp/oslo.db-9.0.0.tar.gz` & `tmp/oslo.db-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oslo.db-9.0.0.tar", last modified: Wed May 12 16:46:40 2021, max compression
+gzip compressed data, was "dist/oslo.db-9.1.0.tar", last modified: Tue Jun 15 09:59:28 2021, max compression
```

## Comparing `oslo.db-9.0.0.tar` & `oslo.db-9.1.0.tar`

### file list

```diff
@@ -1,161 +1,162 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.173291 oslo.db-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2021-05-12 16:46:05.000000 oslo.db-9.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2021-05-12 16:46:05.000000 oslo.db-9.0.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1364 2021-05-12 16:46:05.000000 oslo.db-9.0.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2021-05-12 16:46:05.000000 oslo.db-9.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2021-05-12 16:46:05.000000 oslo.db-9.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7273 2021-05-12 16:46:40.000000 oslo.db-9.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3487 2021-05-12 16:46:05.000000 oslo.db-9.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38401 2021-05-12 16:46:40.000000 oslo.db-9.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2021-05-12 16:46:05.000000 oslo.db-9.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2021-05-12 16:46:05.000000 oslo.db-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2255 2021-05-12 16:46:40.173291 oslo.db-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1032 2021-05-12 16:46:05.000000 oslo.db-9.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2021-05-12 16:46:05.000000 oslo.db-9.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.161293 oslo.db-9.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2021-05-12 16:46:05.000000 oslo.db-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.161293 oslo.db-9.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2117 2021-05-12 16:46:05.000000 oslo.db-9.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.161293 oslo.db-9.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-05-12 16:46:05.000000 oslo.db-9.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2021-05-12 16:46:05.000000 oslo.db-9.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.161293 oslo.db-9.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2021-05-12 16:46:05.000000 oslo.db-9.0.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.161293 oslo.db-9.0.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2021-05-12 16:46:05.000000 oslo.db-9.0.0/doc/source/reference/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2021-05-12 16:46:05.000000 oslo.db-9.0.0/doc/source/reference/opts.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.161293 oslo.db-9.0.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2021-05-12 16:46:05.000000 oslo.db-9.0.0/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2021-05-12 16:46:05.000000 oslo.db-9.0.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5144 2021-05-12 16:46:05.000000 oslo.db-9.0.0/doc/source/user/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.165292 oslo.db-9.0.0/oslo.db.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2255 2021-05-12 16:46:40.000000 oslo.db-9.0.0/oslo.db.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4564 2021-05-12 16:46:40.000000 oslo.db-9.0.0/oslo.db.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-05-12 16:46:40.000000 oslo.db-9.0.0/oslo.db.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2021-05-12 16:46:40.000000 oslo.db-9.0.0/oslo.db.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-05-12 16:46:40.000000 oslo.db-9.0.0/oslo.db.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-05-12 16:46:40.000000 oslo.db-9.0.0/oslo.db.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2021-05-12 16:46:40.000000 oslo.db-9.0.0/oslo.db.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2021-05-12 16:46:40.000000 oslo.db-9.0.0/oslo.db.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.165292 oslo.db-9.0.0/oslo_db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11715 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2642 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/concurrency.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9196 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/exception.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.157293 oslo.db-9.0.0/oslo_db/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.157293 oslo.db-9.0.0/oslo_db/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.165292 oslo.db-9.0.0/oslo_db/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2805 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/locale/en_GB/LC_MESSAGES/oslo_db.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.157293 oslo.db-9.0.0/oslo_db/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.165292 oslo.db-9.0.0/oslo_db/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2941 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/locale/es/LC_MESSAGES/oslo_db.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.157293 oslo.db-9.0.0/oslo_db/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.165292 oslo.db-9.0.0/oslo_db/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2905 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/locale/fr/LC_MESSAGES/oslo_db.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10304 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/options.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.165292 oslo.db-9.0.0/oslo_db/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49467 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/enginefacade.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17238 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/engines.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20130 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/exc_filters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7224 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/migration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.165292 oslo.db-9.0.0/oslo_db/sqlalchemy/migration_cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/migration_cli/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/migration_cli/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4507 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/migration_cli/ext_alembic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2331 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/migration_cli/ext_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2781 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/migration_cli/ext_migrate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4315 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/migration_cli/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4774 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3773 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/ndb.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2642 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/orm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22019 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/provision.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6780 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/session.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8950 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22447 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/test_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22440 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/test_migrations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4842 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17856 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/update_match.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47302 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/sqlalchemy/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.169291 oslo.db-9.0.0/oslo_db/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.169291 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      725 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2630 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4776 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_async_eventlet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    75006 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_enginefacade.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51482 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_exc_filters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9349 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14642 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_migrate_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13150 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_migration_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21623 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_migrations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7452 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7927 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_ndb.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5131 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_options.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8429 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_provision.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29443 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_sqlalchemy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3707 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13842 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_update_match.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    63359 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12335 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4220 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/test_concurrency.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1068 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/tests/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1157 2021-05-12 16:46:05.000000 oslo.db-9.0.0/oslo_db/warning.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.157293 oslo.db-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.173291 oslo.db-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/MySQL-python-no-longer-tested-2a6c32cce6b03215.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/add-reno-e5c2f63e73c25959.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/add_connection_parameters-231aa7d8b7d2d416.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/add_facade_started-14f9bc34fac89371.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/connection_debug_min_max-bf6d53d49be7ca52.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/deprecate-insert-from-select-ea831381ebd7e7cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/deprecate-sqlalchemy-migrate-6f899935615d6984.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/deprecate_config_sqlite_db-bd41d49343049319.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/deprecate_idle_timeout-029d9f2cb7184b28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/drop-python27-support-2308d7fbcd66cc22.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/enginefacade_decorators-4660862fe22d2669.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/fix_synchronous_reader-ca442ca9f07470ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1005 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/increase-default-max-overflow-0af787268807f926.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/new-db-fixtures-58223e3926122413.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/remove-config-option-sqlite_db-7b7c6459135fd8c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/removed-deprecated-min-pool-size-1f351d79fe232129.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/removed-deprecated-sql-max-pool-size-c9b7bfc14c3b6b14.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/warn-incomplete-url-c44cd03baf630c7c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/notes/wrap_db_retry-34c7ff2d82afa3f5.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.173291 oslo.db-9.0.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.173291 oslo.db-9.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.173291 oslo.db-9.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8566 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/liberty.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.157293 oslo.db-9.0.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.157293 oslo.db-9.0.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.173291 oslo.db-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13936 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.157293 oslo.db-9.0.0/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.173291 oslo.db-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1622 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2021-05-12 16:46:05.000000 oslo.db-9.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      677 2021-05-12 16:46:05.000000 oslo.db-9.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1202 2021-05-12 16:46:40.177290 oslo.db-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2021-05-12 16:46:05.000000 oslo.db-9.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      646 2021-05-12 16:46:05.000000 oslo.db-9.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-05-12 16:46:40.173291 oslo.db-9.0.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      261 2021-05-12 16:46:05.000000 oslo.db-9.0.0/tools/run-pifpaf-tests.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2014 2021-05-12 16:46:05.000000 oslo.db-9.0.0/tools/test-setup.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2531 2021-05-12 16:46:05.000000 oslo.db-9.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.740091 oslo.db-9.1.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2021-06-15 09:58:56.000000 oslo.db-9.1.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2021-06-15 09:58:56.000000 oslo.db-9.1.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2021-06-15 09:58:56.000000 oslo.db-9.1.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2021-06-15 09:58:56.000000 oslo.db-9.1.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2021-06-15 09:58:56.000000 oslo.db-9.1.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7352 2021-06-15 09:59:28.000000 oslo.db-9.1.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3487 2021-06-15 09:58:56.000000 oslo.db-9.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38632 2021-06-15 09:59:28.000000 oslo.db-9.1.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2021-06-15 09:58:56.000000 oslo.db-9.1.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2021-06-15 09:58:56.000000 oslo.db-9.1.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2255 2021-06-15 09:59:28.740091 oslo.db-9.1.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1032 2021-06-15 09:58:56.000000 oslo.db-9.1.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2021-06-15 09:58:56.000000 oslo.db-9.1.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.724091 oslo.db-9.1.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2021-06-15 09:58:56.000000 oslo.db-9.1.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.724091 oslo.db-9.1.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2117 2021-06-15 09:58:56.000000 oslo.db-9.1.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.724091 oslo.db-9.1.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-06-15 09:58:56.000000 oslo.db-9.1.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2021-06-15 09:58:56.000000 oslo.db-9.1.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.724091 oslo.db-9.1.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2021-06-15 09:58:56.000000 oslo.db-9.1.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.724091 oslo.db-9.1.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2021-06-15 09:58:56.000000 oslo.db-9.1.0/doc/source/reference/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2021-06-15 09:58:56.000000 oslo.db-9.1.0/doc/source/reference/opts.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.724091 oslo.db-9.1.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2021-06-15 09:58:56.000000 oslo.db-9.1.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2021-06-15 09:58:56.000000 oslo.db-9.1.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5144 2021-06-15 09:58:56.000000 oslo.db-9.1.0/doc/source/user/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.728091 oslo.db-9.1.0/oslo.db.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2255 2021-06-15 09:59:28.000000 oslo.db-9.1.0/oslo.db.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4654 2021-06-15 09:59:28.000000 oslo.db-9.1.0/oslo.db.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-06-15 09:59:28.000000 oslo.db-9.1.0/oslo.db.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2021-06-15 09:59:28.000000 oslo.db-9.1.0/oslo.db.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-06-15 09:59:28.000000 oslo.db-9.1.0/oslo.db.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-06-15 09:59:28.000000 oslo.db-9.1.0/oslo.db.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2021-06-15 09:59:28.000000 oslo.db-9.1.0/oslo.db.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2021-06-15 09:59:28.000000 oslo.db-9.1.0/oslo.db.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.728091 oslo.db-9.1.0/oslo_db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11715 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2642 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/concurrency.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9196 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/exception.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.720091 oslo.db-9.1.0/oslo_db/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.720091 oslo.db-9.1.0/oslo_db/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.728091 oslo.db-9.1.0/oslo_db/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2805 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/locale/en_GB/LC_MESSAGES/oslo_db.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.720091 oslo.db-9.1.0/oslo_db/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.728091 oslo.db-9.1.0/oslo_db/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2941 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/locale/es/LC_MESSAGES/oslo_db.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.720091 oslo.db-9.1.0/oslo_db/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.728091 oslo.db-9.1.0/oslo_db/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2905 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/locale/fr/LC_MESSAGES/oslo_db.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10304 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/options.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.732091 oslo.db-9.1.0/oslo_db/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49467 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/enginefacade.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17238 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/engines.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20552 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/exc_filters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7224 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/migration.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.732091 oslo.db-9.1.0/oslo_db/sqlalchemy/migration_cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/migration_cli/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/migration_cli/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4507 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/migration_cli/ext_alembic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2331 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/migration_cli/ext_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2781 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/migration_cli/ext_migrate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4315 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/migration_cli/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4774 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3773 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/ndb.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2642 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/orm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22019 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/provision.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6780 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/session.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8950 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22447 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/test_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22440 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/test_migrations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4842 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17856 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/update_match.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47302 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/sqlalchemy/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.732091 oslo.db-9.1.0/oslo_db/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.736091 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      725 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2630 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4776 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_async_eventlet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    75006 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_enginefacade.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52463 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_exc_filters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9349 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14642 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_migrate_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13150 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_migration_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21623 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_migrations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7452 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7927 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_ndb.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5131 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_options.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8429 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_provision.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29443 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_sqlalchemy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3707 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13842 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_update_match.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    63359 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12335 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4220 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/test_concurrency.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1068 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/tests/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1157 2021-06-15 09:58:56.000000 oslo.db-9.1.0/oslo_db/warning.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.720091 oslo.db-9.1.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.736091 oslo.db-9.1.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/MySQL-python-no-longer-tested-2a6c32cce6b03215.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/add-reno-e5c2f63e73c25959.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/add_connection_parameters-231aa7d8b7d2d416.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/add_facade_started-14f9bc34fac89371.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/connection_debug_min_max-bf6d53d49be7ca52.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/deprecate-insert-from-select-ea831381ebd7e7cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/deprecate-sqlalchemy-migrate-6f899935615d6984.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/deprecate_config_sqlite_db-bd41d49343049319.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/deprecate_idle_timeout-029d9f2cb7184b28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/drop-python27-support-2308d7fbcd66cc22.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/enginefacade_decorators-4660862fe22d2669.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/fix-mysql-duplicate-key-error-information-update-548888bc44b8dbd7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/fix_synchronous_reader-ca442ca9f07470ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1005 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/increase-default-max-overflow-0af787268807f926.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/new-db-fixtures-58223e3926122413.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/remove-config-option-sqlite_db-7b7c6459135fd8c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/removed-deprecated-min-pool-size-1f351d79fe232129.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/removed-deprecated-sql-max-pool-size-c9b7bfc14c3b6b14.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/warn-incomplete-url-c44cd03baf630c7c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/notes/wrap_db_retry-34c7ff2d82afa3f5.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.740091 oslo.db-9.1.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.740091 oslo.db-9.1.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.740091 oslo.db-9.1.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8566 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/liberty.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.720091 oslo.db-9.1.0/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.720091 oslo.db-9.1.0/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.740091 oslo.db-9.1.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13936 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.720091 oslo.db-9.1.0/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.740091 oslo.db-9.1.0/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1622 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2021-06-15 09:58:56.000000 oslo.db-9.1.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      677 2021-06-15 09:58:56.000000 oslo.db-9.1.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1202 2021-06-15 09:59:28.744091 oslo.db-9.1.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2021-06-15 09:58:56.000000 oslo.db-9.1.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      646 2021-06-15 09:58:56.000000 oslo.db-9.1.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-15 09:59:28.740091 oslo.db-9.1.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      261 2021-06-15 09:58:56.000000 oslo.db-9.1.0/tools/run-pifpaf-tests.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2014 2021-06-15 09:58:56.000000 oslo.db-9.1.0/tools/test-setup.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2531 2021-06-15 09:58:56.000000 oslo.db-9.1.0/tox.ini
```

### Comparing `oslo.db-9.0.0/.pre-commit-config.yaml` & `oslo.db-9.1.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # the newer versions with their commit hash.
 
 default_language_version:
   python: python3
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: ebc15addedad713c86ef18ae9632c88e187dd0af  # v3.1.0
+    rev: 9136088a246768144165fcc3ecc3d31bb686920a # v3.3.0
     hooks:
       - id: trailing-whitespace
       # Replaces or checks mixed line ending
       - id: mixed-line-ending
         args: ['--fix', 'lf']
         exclude: '.*\.(svg)$'
       # Forbid files which have a UTF-8 byte-order marker
```

### Comparing `oslo.db-9.0.0/AUTHORS` & `oslo.db-9.1.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 Joshua Harlow <harlowja@gmail.com>
 Joshua Harlow <harlowja@yahoo-inc.com>
 Joshua Harlow <jxharlow@godaddy.com>
 Julia Varlamova <jvarlamova@mirantis.com>
 Julian Sy <js802v@att.com>
 Julien Danjou <julien@danjou.info>
 Kai Zhang <kazhang2@cisco.com>
+Kamlesh Chauvhan <kamlesh.chauvhan@gmail.com>
 Kenneth Giusti <kgiusti@gmail.com>
 Kevin Benton <blak111@gmail.com>
 Kevin Benton <kevin@benton.pub>
 Lucas Alvares Gomes <lucasagomes@gmail.com>
 Luis A. Garcia <luis@linux.vnet.ibm.com>
 Marco Fargetta <marco.fargetta@ct.infn.it>
 Mark McLoughlin <markmc@redhat.com>
@@ -150,14 +151,15 @@
 Vlad Okhrimenko <vokhrimenko@mirantis.com>
 Vladyslav Drok <vdrok@mirantis.com>
 Vu Cong Tuan <tuanvc@vn.fujitsu.com>
 Wu Wenxiang <wu.wenxiang@99cloud.net>
 Yaguo Zhou <ygzhou@sysnew.com>
 Yaguo Zhou <zhouyaguo@gmail.com>
 Yikun Jiang <yikunkero@gmail.com>
+YuehuiLei <leiyuehui@inspur.com>
 Zane Bitter <zbitter@redhat.com>
 Zhang Chun <zhang.chun.os@99cloud.net>
 Zhang Xin <ada.os@99cloud.net>
 Zhi Yan Liu <zhiyanl@cn.ibm.com>
 ZhijunWei <wzj334965317@outlook.com>
 ZhongShengping <chdzsp@163.com>
 Zhongyue Luo <zhongyue.nah@intel.com>
```

### Comparing `oslo.db-9.0.0/CONTRIBUTING.rst` & `oslo.db-9.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/ChangeLog` & `oslo.db-9.1.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 CHANGES
 =======
 
+9.1.0
+-----
+
+* Followup of "Added handler for mysql 8.0.19 duplicate key error update"
+* Added handler for mysql 8.0.19 duplicate key error update
+* update the pre-commit-hooks version
+
 9.0.0
 -----
 
+* setup.cfg: Replace dashes with underscores
 
 8.6.0
 -----
 
 * Don't use private API to get query criteria
 * Remove the sql\_max\_pool\_size option
 * Fix formatting of release list
```

### Comparing `oslo.db-9.0.0/LICENSE` & `oslo.db-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/PKG-INFO` & `oslo.db-9.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslo.db
-Version: 9.0.0
+Version: 9.1.0
 Summary: Oslo Database library
 Home-page: https://docs.openstack.org/oslo.db/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `oslo.db-9.0.0/README.rst` & `oslo.db-9.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/doc/source/conf.py` & `oslo.db-9.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/doc/source/index.rst` & `oslo.db-9.1.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/doc/source/install/index.rst` & `oslo.db-9.1.0/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/doc/source/user/usage.rst` & `oslo.db-9.1.0/doc/source/user/usage.rst`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo.db.egg-info/PKG-INFO` & `oslo.db-9.1.0/oslo.db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslo.db
-Version: 9.0.0
+Version: 9.1.0
 Summary: Oslo Database library
 Home-page: https://docs.openstack.org/oslo.db/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `oslo.db-9.0.0/oslo.db.egg-info/SOURCES.txt` & `oslo.db-9.1.0/oslo.db.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 releasenotes/notes/connection_debug_min_max-bf6d53d49be7ca52.yaml
 releasenotes/notes/deprecate-insert-from-select-ea831381ebd7e7cf.yaml
 releasenotes/notes/deprecate-sqlalchemy-migrate-6f899935615d6984.yaml
 releasenotes/notes/deprecate_config_sqlite_db-bd41d49343049319.yaml
 releasenotes/notes/deprecate_idle_timeout-029d9f2cb7184b28.yaml
 releasenotes/notes/drop-python27-support-2308d7fbcd66cc22.yaml
 releasenotes/notes/enginefacade_decorators-4660862fe22d2669.yaml
+releasenotes/notes/fix-mysql-duplicate-key-error-information-update-548888bc44b8dbd7.yaml
 releasenotes/notes/fix_synchronous_reader-ca442ca9f07470ec.yaml
 releasenotes/notes/increase-default-max-overflow-0af787268807f926.yaml
 releasenotes/notes/new-db-fixtures-58223e3926122413.yaml
 releasenotes/notes/remove-config-option-sqlite_db-7b7c6459135fd8c9.yaml
 releasenotes/notes/removed-deprecated-min-pool-size-1f351d79fe232129.yaml
 releasenotes/notes/removed-deprecated-sql-max-pool-size-c9b7bfc14c3b6b14.yaml
 releasenotes/notes/warn-incomplete-url-c44cd03baf630c7c.yaml
```

### Comparing `oslo.db-9.0.0/oslo.db.egg-info/requires.txt` & `oslo.db-9.1.0/oslo.db.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/_i18n.py` & `oslo.db-9.1.0/oslo_db/_i18n.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/api.py` & `oslo.db-9.1.0/oslo_db/api.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/concurrency.py` & `oslo.db-9.1.0/oslo_db/concurrency.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/exception.py` & `oslo.db-9.1.0/oslo_db/exception.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/locale/en_GB/LC_MESSAGES/oslo_db.po` & `oslo.db-9.1.0/oslo_db/locale/en_GB/LC_MESSAGES/oslo_db.po`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/locale/es/LC_MESSAGES/oslo_db.po` & `oslo.db-9.1.0/oslo_db/locale/es/LC_MESSAGES/oslo_db.po`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/locale/fr/LC_MESSAGES/oslo_db.po` & `oslo.db-9.1.0/oslo_db/locale/fr/LC_MESSAGES/oslo_db.po`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/options.py` & `oslo.db-9.1.0/oslo_db/options.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/enginefacade.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/enginefacade.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/engines.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/engines.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/exc_filters.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/exc_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,20 @@
 
     postgres:
     1 column - (IntegrityError) duplicate key value violates unique
                constraint "users_c1_key"
     N columns - (IntegrityError) duplicate key value violates unique
                constraint "name_of_our_constraint"
 
+    mysql since 8.0.19:
+    1 column - (IntegrityError) (1062, "Duplicate entry 'value_of_c1' for key
+               'table_name.c1'")
+    N columns - (IntegrityError) (1062, "Duplicate entry 'values joined
+               with -' for key 'table_name.name_of_our_constraint'")
+
     mysql+mysqldb:
     1 column - (IntegrityError) (1062, "Duplicate entry 'value_of_c1' for key
                'c1'")
     N columns - (IntegrityError) (1062, "Duplicate entry 'values joined
                with -' for key 'name_of_our_constraint'")
 
     mysql+mysqlconnector:
@@ -141,14 +147,17 @@
     # note(vsergeyev): UniqueConstraint name convention: "uniq_t0c10c2"
     #                  where `t` it is table name and columns `c1`, `c2`
     #                  are in UniqueConstraint.
     uniqbase = "uniq_"
     if not columns.startswith(uniqbase):
         if engine_name == "postgresql":
             columns = [columns[columns.index("_") + 1:columns.rindex("_")]]
+        elif (engine_name == "mysql") and \
+             (uniqbase in str(columns.split("0")[:1])):
+            columns = columns.split("0")[1:]
         else:
             columns = [columns]
     else:
         columns = columns[len(uniqbase):].split("0")[1:]
 
     value = match.groupdict().get('value')
```

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/migration.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/migration.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/migration_cli/ext_alembic.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/migration_cli/ext_alembic.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/migration_cli/ext_base.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/migration_cli/ext_base.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/migration_cli/ext_migrate.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/migration_cli/ext_migrate.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/migration_cli/manager.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/migration_cli/manager.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/models.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/ndb.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/ndb.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/orm.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/orm.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/provision.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/provision.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/session.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/session.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/test_base.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/test_base.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/test_fixtures.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/test_migrations.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/test_migrations.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/types.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/update_match.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/update_match.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/sqlalchemy/utils.py` & `oslo.db-9.1.0/oslo_db/sqlalchemy/utils.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/__init__.py` & `oslo.db-9.1.0/oslo_db/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/base.py` & `oslo.db-9.1.0/oslo_db/tests/base.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/__init__.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/base.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_async_eventlet.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_async_eventlet.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_enginefacade.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_enginefacade.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_exc_filters.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_exc_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -817,14 +817,22 @@
         self._run_dupe_constraint_test(
             "mysql",
             "1062 (23000): Duplicate entry '2' for key 'b'",
             expected_columns=['b'],
             expected_value='2'
         )
 
+    def test_mysql_duplicate_entry_key_start_with_tablename(self):
+        self._run_dupe_constraint_test(
+            "mysql",
+            "1062 (23000): Duplicate entry '2' for key 'tbl.uniq_tbl0b'",
+            expected_columns=['b'],
+            expected_value='2'
+        )
+
     def test_mysql_binary(self):
         self._run_dupe_constraint_test(
             "mysql",
             "(1062, \'Duplicate entry "
             "\\\'\\\\x8A$\\\\x8D\\\\xA6\"s\\\\x8E\\\' "
             "for key \\\'PRIMARY\\\'\')",
             expected_columns=['PRIMARY'],
@@ -835,14 +843,32 @@
             "(1062, \'Duplicate entry "
             "''\\\\x8A$\\\\x8D\\\\xA6\"s\\\\x8E!,' "
             "for key 'PRIMARY'\')",
             expected_columns=['PRIMARY'],
             expected_value="'\\\\x8A$\\\\x8D\\\\xA6\"s\\\\x8E!,"
         )
 
+    def test_mysql_duplicate_entry_key_start_with_tablename_binary(self):
+        self._run_dupe_constraint_test(
+            "mysql",
+            "(1062, \'Duplicate entry "
+            "\\\'\\\\x8A$\\\\x8D\\\\xA6\"s\\\\x8E\\\' "
+            "for key \\\'tbl.uniq_tbl0c1\\\'\')",
+            expected_columns=['c1'],
+            expected_value="\\\\x8A$\\\\x8D\\\\xA6\"s\\\\x8E"
+        )
+        self._run_dupe_constraint_test(
+            "mysql",
+            "(1062, \'Duplicate entry "
+            "''\\\\x8A$\\\\x8D\\\\xA6\"s\\\\x8E!,' "
+            "for key 'tbl.uniq_tbl0c1'\')",
+            expected_columns=['c1'],
+            expected_value="'\\\\x8A$\\\\x8D\\\\xA6\"s\\\\x8E!,"
+        )
+
     def test_postgresql_single(self):
         self._run_dupe_constraint_test(
             'postgresql',
             'duplicate key value violates unique constraint "uniq_tbl0b"\n'
             'DETAIL:  Key (b)=(2) already exists.\n',
             expected_columns=['b'],
             expected_value='2'
```

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_fixtures.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_migrate_cli.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_migrate_cli.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_migration_common.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_migration_common.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_migrations.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_migrations.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_models.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_models.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_ndb.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_ndb.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_options.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_options.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_provision.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_provision.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_sqlalchemy.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_types.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_types.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_update_match.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_update_match.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/sqlalchemy/test_utils.py` & `oslo.db-9.1.0/oslo_db/tests/sqlalchemy/test_utils.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/test_api.py` & `oslo.db-9.1.0/oslo_db/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/test_concurrency.py` & `oslo.db-9.1.0/oslo_db/tests/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/tests/utils.py` & `oslo.db-9.1.0/oslo_db/tests/utils.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/oslo_db/warning.py` & `oslo.db-9.1.0/oslo_db/warning.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/releasenotes/notes/deprecate-sqlalchemy-migrate-6f899935615d6984.yaml` & `oslo.db-9.1.0/releasenotes/notes/deprecate-sqlalchemy-migrate-6f899935615d6984.yaml`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/releasenotes/notes/deprecate_idle_timeout-029d9f2cb7184b28.yaml` & `oslo.db-9.1.0/releasenotes/notes/deprecate_idle_timeout-029d9f2cb7184b28.yaml`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/releasenotes/notes/increase-default-max-overflow-0af787268807f926.yaml` & `oslo.db-9.1.0/releasenotes/notes/increase-default-max-overflow-0af787268807f926.yaml`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/releasenotes/notes/warn-incomplete-url-c44cd03baf630c7c.yaml` & `oslo.db-9.1.0/releasenotes/notes/warn-incomplete-url-c44cd03baf630c7c.yaml`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/releasenotes/source/conf.py` & `oslo.db-9.1.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `oslo.db-9.1.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `oslo.db-9.1.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/requirements.txt` & `oslo.db-9.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/setup.cfg` & `oslo.db-9.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = oslo.db
 summary = Oslo Database library
-description-file = 
+description_file = 
 	README.rst
 author = OpenStack
-author-email = openstack-discuss@lists.openstack.org
-home-page = https://docs.openstack.org/oslo.db/latest
-python-requires = >=3.6
+author_email = openstack-discuss@lists.openstack.org
+home_page = https://docs.openstack.org/oslo.db/latest
+python_requires = >=3.6
 classifier = 
 	Environment :: OpenStack
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
```

### Comparing `oslo.db-9.0.0/setup.py` & `oslo.db-9.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/test-requirements.txt` & `oslo.db-9.1.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/tools/test-setup.sh` & `oslo.db-9.1.0/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `oslo.db-9.0.0/tox.ini` & `oslo.db-9.1.0/tox.ini`

 * *Files identical despite different names*

