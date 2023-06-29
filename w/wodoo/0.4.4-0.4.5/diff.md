# Comparing `tmp/wodoo-0.4.4.tar.gz` & `tmp/wodoo-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wodoo-0.4.4.tar", last modified: Fri Jun 23 13:53:45 2023, max compression
+gzip compressed data, was "wodoo-0.4.5.tar", last modified: Thu Jun 29 07:29:27 2023, max compression
```

## Comparing `wodoo-0.4.4.tar` & `wodoo-0.4.5.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.645421 wodoo-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 13:53:15.000000 wodoo-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-23 13:53:45.645421 wodoo-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-23 13:53:15.000000 wodoo-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 13:53:45.649421 wodoo-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-23 13:53:15.000000 wodoo-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.637421 wodoo-0.4.4/wodoo/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/click_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/click_global_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.641421 wodoo-0.4.4/wodoo/config/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/config/cicd_network_for_project.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/config/default_network
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/config/template_onlyloop.yml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/config/template_withports.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/consts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7012 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/daddy_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/defaults
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.629421 wodoo-0.4.4/wodoo/extra_install/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.629421 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.641421 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/debug.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/entrypoint.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/interactive.sh
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.641421 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/config
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa.pub
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.641421 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.641421 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.641421 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/ari_additional_custom.conf.appendix
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/manager_custom.conf.appendix
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.641421 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.641421 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/freepbx_chown.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.641421 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/
--rwxr-xr-x   0 runner    (1001) docker     (123)      349 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/10-freepbx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.641421 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/10-start
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.645421 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/apache2
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/asterisk
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fail2ban
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fop
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbc.ini
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbcinst.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.645421 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/08-ssh
--rwxr-xr-x   0 runner    (1001) docker     (123)      567 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb
--rwxr-xr-x   0 runner    (1001) docker     (123)    17011 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx
--rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/13-extra-modules
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/15-permissions
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/16-soundlang
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/20-load-default-extensions
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.629421 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.645421 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/authorized_keys
--rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/run_freepbx.sh
--rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_clickhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    30348 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14748 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_control_with_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_db_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_db_snapshots_docker_btrfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_db_snapshots_docker_zfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_db_snapshots_plain_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_docker_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)    50013 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_src.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_talk.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/lib_turnintodev.py
--rw-r--r--   0 runner    (1001) docker     (123)    55120 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/module_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/myconfigparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/odoo_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    25337 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/odoo_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/pudb.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/robo_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.645421 wodoo-0.4.4/wodoo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/tests/MANIFEST
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/tests/gimera.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.645421 wodoo-0.4.4/wodoo/tests/module_respartner_dummyfield1/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/tests/module_respartner_dummyfield1/partnerview.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.645421 wodoo-0.4.4/wodoo/tests/module_respartner_dummyfield2/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/tests/module_respartner_dummyfield2/partnerview.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/testzfs.sh
--rw-r--r--   0 runner    (1001) docker     (123)    42280 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 13:53:41.000000 wodoo-0.4.4/wodoo/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.645421 wodoo-0.4.4/wodoo/wait/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/wait/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/wait/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/wait/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-23 13:53:15.000000 wodoo-0.4.4/wodoo/wait/tcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:53:45.637421 wodoo-0.4.4/wodoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-23 13:53:45.000000 wodoo-0.4.4/wodoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-23 13:53:45.000000 wodoo-0.4.4/wodoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:53:45.000000 wodoo-0.4.4/wodoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 13:53:45.000000 wodoo-0.4.4/wodoo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-23 13:53:45.000000 wodoo-0.4.4/wodoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 13:53:45.000000 wodoo-0.4.4/wodoo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 07:29:10.000000 wodoo-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-06-29 07:29:27.070438 wodoo-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-06-29 07:29:10.000000 wodoo-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-29 07:29:27.070438 wodoo-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-29 07:29:10.000000 wodoo-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.066438 wodoo-0.4.5/wodoo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/click_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/click_global_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.066438 wodoo-0.4.5/wodoo/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/config/cicd_network_for_project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/config/default_network
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/config/template_onlyloop.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/config/template_withports.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/consts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7012 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/daddy_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/defaults
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.062437 wodoo-0.4.5/wodoo/extra_install/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.062437 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/debug.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/entrypoint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/interactive.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/config
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa.pub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/ari_additional_custom.conf.appendix
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/manager_custom.conf.appendix
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/freepbx_chown.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      349 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/10-freepbx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/10-start
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/apache2
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/asterisk
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fail2ban
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fop
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbc.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbcinst.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/08-ssh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      567 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17011 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/13-extra-modules
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/15-permissions
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/16-soundlang
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/20-load-default-extensions
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.062437 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/authorized_keys
+-rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/run_freepbx.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_clickhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31871 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14748 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_control_with_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_db_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_db_snapshots_docker_btrfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_db_snapshots_docker_zfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_db_snapshots_plain_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_docker_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50013 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_src.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_talk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/lib_turnintodev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55119 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/module_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/myconfigparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/odoo_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25337 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/odoo_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/pudb.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/robo_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/wodoo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/tests/MANIFEST
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/tests/gimera.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/wodoo/tests/module_respartner_dummyfield1/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/tests/module_respartner_dummyfield1/partnerview.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/wodoo/tests/module_respartner_dummyfield2/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/tests/module_respartner_dummyfield2/partnerview.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/testzfs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    42346 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 07:29:23.000000 wodoo-0.4.5/wodoo/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.070438 wodoo-0.4.5/wodoo/wait/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/wait/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/wait/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/wait/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-29 07:29:10.000000 wodoo-0.4.5/wodoo/wait/tcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:27.066438 wodoo-0.4.5/wodoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-06-29 07:29:27.000000 wodoo-0.4.5/wodoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-29 07:29:27.000000 wodoo-0.4.5/wodoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:29:27.000000 wodoo-0.4.5/wodoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 07:29:27.000000 wodoo-0.4.5/wodoo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-29 07:29:27.000000 wodoo-0.4.5/wodoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 07:29:27.000000 wodoo-0.4.5/wodoo.egg-info/top_level.txt
```

### Comparing `wodoo-0.4.4/LICENSE` & `wodoo-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/PKG-INFO` & `wodoo-0.4.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: wodoo
-Version: 0.4.4
-Summary: Odoo Framework
-Home-page: https://github.com/marcwimmer/wodoo
-Author: Marc-Christian Wimmer
-License: MIT
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # Odoo Docker Framework
 
 Provides functionalities:
 
 - setup empty new odoo with one bash command `odoo init --version 15.0`
 
 - setup full fleged odoo server environment containing
@@ -56,14 +44,55 @@
 odoo reload
 odoo -f db reset
 odoo up -d
 
 # now open browser on http://localhost
 ```
 
+## How to extend odoo docker image
+
+* make folder ```docker/odoo``` in your source repo
+* add file:
+
+```
+# docker/odoo/docker-compose.run_odoo_version.14.0.yml
+services:
+  odoo_appendix:
+    build:
+        context: $CUSTOMS_DIR/docker/odoo
+        dockerfile: $CUSTOMS_DIR/docker/odoo/Dockerfile
+```
+* add Docker file:
+
+```
+# docker/odoo/Dockerfile
+FROM ubuntu:22.04
+RUN apt update && \
+apt install -y tar && \
+mkdir /tmp/pack
+
+ADD ibm-iaccess-1.1.0.27-1.0.amd64.deb /tmp/pack
+ADD install.sh /tmp/pack/install.sh
+ADD odbc.ini /tmp/pack/odbc.ini
+
+RUN chmod a+x /tmp/pack/install.sh
+RUN tar cfz /odoo_install_appendix.tar.gz /tmp/pack
+```
+
+# add Dockerfile.appendix
+```
+COPY --from=${PROJECT_NAME}_odoo_appendix /odoo_install_appendix.tar.gz /tmp/install_appendix.tar.gz
+RUN \
+mkdir /tmp/install_package && \
+cd /tmp/install_package && \
+tar xfz /tmp/install_appendix.tar.gz && \
+ls -lhtra && \
+./install.sh
+```
+
 ## Store settings in ./odoo of source code
 
 
 ## How to extend an existing service
 
 - make a docker-compose file like ~/.odoo/docker-compose.yml
 
@@ -204,8 +233,8 @@
 ```
 
 # Performance Check
 
 ```python
 pipx runpip wodoo install line_profiler
 ~/.local/pipx/venvs/wodoo/bin/python3 -mkernprof -l -v odoo reload
-```
+```
```

### Comparing `wodoo-0.4.4/README.md` & `wodoo-0.4.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: wodoo
+Version: 0.4.5
+Summary: Odoo Framework
+Home-page: https://github.com/marcwimmer/wodoo
+Author: Marc-Christian Wimmer
+License: MIT
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 # Odoo Docker Framework
 
 Provides functionalities:
 
 - setup empty new odoo with one bash command `odoo init --version 15.0`
 
 - setup full fleged odoo server environment containing
@@ -44,14 +56,55 @@
 odoo reload
 odoo -f db reset
 odoo up -d
 
 # now open browser on http://localhost
 ```
 
+## How to extend odoo docker image
+
+* make folder ```docker/odoo``` in your source repo
+* add file:
+
+```
+# docker/odoo/docker-compose.run_odoo_version.14.0.yml
+services:
+  odoo_appendix:
+    build:
+        context: $CUSTOMS_DIR/docker/odoo
+        dockerfile: $CUSTOMS_DIR/docker/odoo/Dockerfile
+```
+* add Docker file:
+
+```
+# docker/odoo/Dockerfile
+FROM ubuntu:22.04
+RUN apt update && \
+apt install -y tar && \
+mkdir /tmp/pack
+
+ADD ibm-iaccess-1.1.0.27-1.0.amd64.deb /tmp/pack
+ADD install.sh /tmp/pack/install.sh
+ADD odbc.ini /tmp/pack/odbc.ini
+
+RUN chmod a+x /tmp/pack/install.sh
+RUN tar cfz /odoo_install_appendix.tar.gz /tmp/pack
+```
+
+# add Dockerfile.appendix
+```
+COPY --from=${PROJECT_NAME}_odoo_appendix /odoo_install_appendix.tar.gz /tmp/install_appendix.tar.gz
+RUN \
+mkdir /tmp/install_package && \
+cd /tmp/install_package && \
+tar xfz /tmp/install_appendix.tar.gz && \
+ls -lhtra && \
+./install.sh
+```
+
 ## Store settings in ./odoo of source code
 
 
 ## How to extend an existing service
 
 - make a docker-compose file like ~/.odoo/docker-compose.yml
 
@@ -192,8 +245,8 @@
 ```
 
 # Performance Check
 
 ```python
 pipx runpip wodoo install line_profiler
 ~/.local/pipx/venvs/wodoo/bin/python3 -mkernprof -l -v odoo reload
-```
+```
```

### Comparing `wodoo-0.4.4/setup.py` & `wodoo-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/__init__.py` & `wodoo-0.4.5/wodoo/__init__.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/cli.py` & `wodoo-0.4.5/wodoo/cli.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/click_config.py` & `wodoo-0.4.5/wodoo/click_config.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/click_global_commands.py` & `wodoo-0.4.5/wodoo/click_global_commands.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/consts.py` & `wodoo-0.4.5/wodoo/consts.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     'odoo_data_dir': "~/.odoo/files",
     'user_conf_dir': "~/.odoo",
     'cicd_delegator': '~/.odoo/cicd_delegator',
     'images': '~/.odoo/images',
 }
 
 default_files = {
+    'odoo_docker_file': '${run}/Dockerfile.odoo',
     'after_reload_script': "/usr/local/bin/after-odoo-reload.sh",
     'after_up_script': "/usr/local/bin/after-odoo-up.sh",
     'odoo_config_file_additions': "~/.odoo/odoo.config",
     'odoo_config_file_additions.project': "~/.odoo/odoo.config.${project_name}",
     'project_settings': "~/.odoo/settings.${project_name}",
     'project_docker_compose.home': "~/.odoo/docker-compose.yml",
     'project_docker_compose.home.project': "~/.odoo/docker-compose.${project_name}.yml",
```

### Comparing `wodoo-0.4.4/wodoo/daddy_cleanup.py` & `wodoo-0.4.5/wodoo/daddy_cleanup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/defaults` & `wodoo-0.4.5/wodoo/defaults`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt` & `wodoo-0.4.5/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml` & `wodoo-0.4.5/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa` & `wodoo-0.4.5/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt` & `wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile` & `wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml` & `wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files` & `wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv` & `wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb` & `wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx` & `wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings` & `wodoo-0.4.5/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/lib_backup.py` & `wodoo-0.4.5/wodoo/lib_backup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/lib_clickhelpers.py` & `wodoo-0.4.5/wodoo/lib_clickhelpers.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/lib_composer.py` & `wodoo-0.4.5/wodoo/lib_composer.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from .tools import __replace_all_envs_in_str
 from .tools import __running_as_root_or_sudo
 from .tools import _makedirs
 from .tools import __try_to_set_owner
 from .tools import whoami
 from .tools import abort
 from .tools import _get_version
+from .tools import rsync
 from .cli import cli, pass_config, Commands
 from .lib_clickhelpers import AliasedGroup
 from .odoo_config import MANIFEST
 from .tools import execute_script
 from .tools import ensure_project_name
 
 
@@ -301,14 +302,15 @@
     _export_settings(config, forced_values)
     _prepare_filesystem(config)
     _execute_after_settings(config)
 
     _prepare_yml_files_from_template_files(
         config, additional_docker_configuration_files
     )
+    _merge_odoo_dockerfile(config)
 
     click.echo("Built the docker-compose file.")
 
 
 def _download_images(config, images_url):
     from . import consts
 
@@ -549,14 +551,15 @@
     _files2 = []
     for x in _files:
         if x in _files2:
             continue
         _files2.append(x)
     _files = _files2
     del _files2
+
     _prepare_docker_compose_files(config, config.files["docker_compose"], _files)
 
 
 def __resolve_custom_merge(whole_content, value):
     for k in list(value.keys()):
         if k == "__custom_merge":
             insert = whole_content["services"][value[k]]
@@ -979,8 +982,44 @@
         return
 
     from .lib_src import _turn_into_odoosh
 
     _turn_into_odoosh(ctx, customs_dir())
 
 
+def _merge_odoo_dockerfile(config):
+    """
+    If customs contains dockerfile, then append their execution
+    in the main dockerfile
+    """
+    import yaml
+    content = config.files['docker_compose'].read_text()
+    content = yaml.safe_load(content)
+    for service in content['services']:
+        servicename = service
+        service = content['services'][service]
+        dockerfile = service.get('build', {})
+        if isinstance(dockerfile, str):
+            continue
+        dockerfile = dockerfile.get('dockerfile')
+        if not dockerfile:
+            continue
+        if 'odoo/images/odoo' in dockerfile:
+            shutil.copy(dockerfile, config.files['odoo_docker_file'])
+            dockerfile1 = dockerfile
+            service['build']['dockerfile'] = str(config.files['odoo_docker_file'])
+        del dockerfile
+    content = yaml.dump(content, default_flow_style=False)
+    config.files['docker_compose'].write_text(content)
+
+    # copy dockerfile to new location
+    click.secho(f"Copying {dockerfile1} to {config.files['odoo_docker_file']}")
+    config.files['odoo_docker_file'].write_text(Path(dockerfile1).read_text())
+    for file in bash_find(config.WORKING_DIR, "Dockerfile.appendix"):
+        appendix = file.read_text()
+        file = config.files['odoo_docker_file']
+        content = file.read_text() + "\n" + appendix
+        content = content.replace("${PROJECT_NAME}", config.project_name)
+        file.write_text(content)
+
+
 Commands.register(do_reload, "reload")
```

### Comparing `wodoo-0.4.4/wodoo/lib_control.py` & `wodoo-0.4.5/wodoo/lib_control.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/lib_control_with_docker.py` & `wodoo-0.4.5/wodoo/lib_control_with_docker.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/lib_db.py` & `wodoo-0.4.5/wodoo/lib_db.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/lib_db_snapshots.py` & `wodoo-0.4.5/wodoo/lib_db_snapshots.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/lib_db_snapshots_docker_btrfs.py` & `wodoo-0.4.5/wodoo/lib_db_snapshots_docker_btrfs.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/lib_db_snapshots_docker_zfs.py` & `wodoo-0.4.5/wodoo/lib_db_snapshots_docker_zfs.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/lib_db_snapshots_plain_postgres.py` & `wodoo-0.4.5/wodoo/lib_db_snapshots_plain_postgres.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/lib_docker_registry.py` & `wodoo-0.4.5/wodoo/lib_docker_registry.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/lib_lang.py` & `wodoo-0.4.5/wodoo/lib_lang.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/lib_module.py` & `wodoo-0.4.5/wodoo/lib_module.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/lib_setup.py` & `wodoo-0.4.5/wodoo/lib_setup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/lib_src.py` & `wodoo-0.4.5/wodoo/lib_src.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/lib_talk.py` & `wodoo-0.4.5/wodoo/lib_talk.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/lib_turnintodev.py` & `wodoo-0.4.5/wodoo/lib_turnintodev.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/module_tools.py` & `wodoo-0.4.5/wodoo/module_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -757,16 +757,16 @@
                     if dep not in remark_about_missing_module_info:
                         remark_about_missing_module_info.add(dep)
                         click.secho(
                             (
                                 f"Module not found at resolving dependencies: {dep}"
                                 ". Not necessarily a problem at auto install modules."
                             ),
-                            fg="yellow",
-                            bold=True,
+                            fg="blue",
+                            bold=False,
                         )
                     dep_mod = Module(None, force_name=dep)
 
                 result.add(dep_mod)
                 if dep_mod in dep_tree_cache:
                     result |= set(dep_tree_cache[dep_mod])
                     continue
```

### Comparing `wodoo-0.4.4/wodoo/myconfigparser.py` & `wodoo-0.4.5/wodoo/myconfigparser.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/odoo_config.py` & `wodoo-0.4.5/wodoo/odoo_config.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/odoo_parser.py` & `wodoo-0.4.5/wodoo/odoo_parser.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/robo_helpers.py` & `wodoo-0.4.5/wodoo/robo_helpers.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/settings.py` & `wodoo-0.4.5/wodoo/settings.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/testzfs.sh` & `wodoo-0.4.5/wodoo/testzfs.sh`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/tools.py` & `wodoo-0.4.5/wodoo/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -965,16 +965,18 @@
 
 
 def rsync(src, dest, options="-ar", exclude=None):
     exclude = exclude or ""
     exclude_option = []
     for x in exclude:
         exclude_option += ["--exclude", x]
+    if not isinstance(options, list):
+        options = [options]
     subprocess.check_call(
-        ["rsync", str(src) + "/", str(dest) + "/", options] + exclude_option
+        ["rsync", str(src) + "/", str(dest) + "/"] + options + exclude_option
     )
 
 
 def copy_dir_contents(dir, dest_dir, exclude=None):
     assert dir.is_dir()
     assert dest_dir.is_dir()
     exclude = exclude or []
@@ -1494,15 +1496,14 @@
     remember = os.getcwd()
     os.chdir(path)
     try:
         yield
     finally:
         os.chdir(remember)
 
-
 @contextmanager
 def atomic_write(file):
     tempfile = file.parent / f"{file.name}.{uuid.uuid4()}"
     try:
         yield tempfile
 
         if file.exists():
```

### Comparing `wodoo-0.4.4/wodoo/wait/decorator.py` & `wodoo-0.4.5/wodoo/wait/decorator.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/wait/log.py` & `wodoo-0.4.5/wodoo/wait/log.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo/wait/tcp.py` & `wodoo-0.4.5/wodoo/wait/tcp.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.4/wodoo.egg-info/PKG-INFO` & `wodoo-0.4.5/wodoo.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wodoo
-Version: 0.4.4
+Version: 0.4.5
 Summary: Odoo Framework
 Home-page: https://github.com/marcwimmer/wodoo
 Author: Marc-Christian Wimmer
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -56,14 +56,55 @@
 odoo reload
 odoo -f db reset
 odoo up -d
 
 # now open browser on http://localhost
 ```
 
+## How to extend odoo docker image
+
+* make folder ```docker/odoo``` in your source repo
+* add file:
+
+```
+# docker/odoo/docker-compose.run_odoo_version.14.0.yml
+services:
+  odoo_appendix:
+    build:
+        context: $CUSTOMS_DIR/docker/odoo
+        dockerfile: $CUSTOMS_DIR/docker/odoo/Dockerfile
+```
+* add Docker file:
+
+```
+# docker/odoo/Dockerfile
+FROM ubuntu:22.04
+RUN apt update && \
+apt install -y tar && \
+mkdir /tmp/pack
+
+ADD ibm-iaccess-1.1.0.27-1.0.amd64.deb /tmp/pack
+ADD install.sh /tmp/pack/install.sh
+ADD odbc.ini /tmp/pack/odbc.ini
+
+RUN chmod a+x /tmp/pack/install.sh
+RUN tar cfz /odoo_install_appendix.tar.gz /tmp/pack
+```
+
+# add Dockerfile.appendix
+```
+COPY --from=${PROJECT_NAME}_odoo_appendix /odoo_install_appendix.tar.gz /tmp/install_appendix.tar.gz
+RUN \
+mkdir /tmp/install_package && \
+cd /tmp/install_package && \
+tar xfz /tmp/install_appendix.tar.gz && \
+ls -lhtra && \
+./install.sh
+```
+
 ## Store settings in ./odoo of source code
 
 
 ## How to extend an existing service
 
 - make a docker-compose file like ~/.odoo/docker-compose.yml
```

### Comparing `wodoo-0.4.4/wodoo.egg-info/SOURCES.txt` & `wodoo-0.4.5/wodoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

