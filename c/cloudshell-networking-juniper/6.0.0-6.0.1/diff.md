# Comparing `tmp/cloudshell-networking-juniper-6.0.0.tar.gz` & `tmp/cloudshell-networking-juniper-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudshell-networking-juniper-6.0.0.tar", last modified: Mon Jun 26 17:11:59 2023, max compression
+gzip compressed data, was "cloudshell-networking-juniper-6.0.1.tar", last modified: Thu Jun 29 15:11:57 2023, max compression
```

## Comparing `cloudshell-networking-juniper-6.0.0.tar` & `cloudshell-networking-juniper-6.0.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.502566 cloudshell-networking-juniper-6.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.462566 cloudshell-networking-juniper-6.0.0/.tox/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.474566 cloudshell-networking-juniper-6.0.0/.tox/build/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-26 17:11:52.000000 cloudshell-networking-juniper-6.0.0/.tox/build/.tox-info.json
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-26 17:11:59.502566 cloudshell-networking-juniper-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.474566 cloudshell-networking-juniper-6.0.0/cloudshell/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.474566 cloudshell-networking-juniper-6.0.0/cloudshell/networking/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.474566 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.474566 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.478566 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/generic/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/generic/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/junos_generic_snmp_autoload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.482566 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/mibs/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/mibs/HCNUM-TC.json
--rw-r--r--   0 runner    (1001) docker     (123)   657494 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/mibs/JUNIPER-CHASSIS-DEFINES-MIB.json
--rw-r--r--   0 runner    (1001) docker     (123)    30839 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/mibs/JUNIPER-IF-MIB.json
--rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/mibs/JUNIPER-L2CP-FEATURES-MIB.json
--rw-r--r--   0 runner    (1001) docker     (123)    90661 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/mibs/JUNIPER-MIB.json
--rw-r--r--   0 runner    (1001) docker     (123)    17568 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/mibs/JUNIPER-SMI.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.482566 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/snmp_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/snmp_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/snmp_tables/mibs_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.482566 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/cli/juniper_cli_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/cli/juniper_command_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/cli/juniper_ssh_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/cli/juniper_telnet_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.486566 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_actions/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_actions/add_remove_vlan_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_actions/commit_rollback_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_actions/enable_disable_snmp_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_actions/enable_disable_snmp_v3_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_actions/save_restore_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_actions/system_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.486566 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_templates/add_remove_vlan.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_templates/commit_rollback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_templates/enable_disable_snmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_templates/enable_disable_snmp_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_templates/generic_action_error_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_templates/save_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_templates/system_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.490566 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/flows/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/flows/autoload_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/flows/configuration_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/flows/connectivity_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/flows/juniper_enable_disable_snmp_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/flows/juniper_firmware_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/flows/juniper_state_flow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.490566 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/helpers/add_remove_vlan_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/helpers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.490566 cloudshell-networking-juniper-6.0.0/cloudshell_networking_juniper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-26 17:11:59.000000 cloudshell-networking-juniper-6.0.0/cloudshell_networking_juniper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-26 17:11:59.000000 cloudshell-networking-juniper-6.0.0/cloudshell_networking_juniper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:11:59.000000 cloudshell-networking-juniper-6.0.0/cloudshell_networking_juniper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-26 17:11:59.000000 cloudshell-networking-juniper-6.0.0/cloudshell_networking_juniper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 17:11:59.000000 cloudshell-networking-juniper-6.0.0/cloudshell_networking_juniper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:11:59.502566 cloudshell-networking-juniper-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.490566 cloudshell-networking-juniper-6.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.490566 cloudshell-networking-juniper-6.0.0/tests/networking/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.494566 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.494566 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/autoload/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/autoload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.494566 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/cli/test_juniper_ssh_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/cli/test_juniper_telnet_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.498566 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/command_actions/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/command_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/command_actions/test_add_remove_vlan_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/command_actions/test_commit_rollback_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/command_actions/test_enable_disable_snmp_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/command_actions/test_save_restore_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/command_actions/test_system_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.498566 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/command_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/command_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.498566 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/flows/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/flows/test_juniper_enable_disable_snmp_flow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.498566 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/helpers/test_add_remove_vlan_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:11:59.498566 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/snmp/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tests/networking/juniper/snmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 17:11:47.000000 cloudshell-networking-juniper-6.0.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.323769 cloudshell-networking-juniper-6.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.307769 cloudshell-networking-juniper-6.0.1/.tox/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.311769 cloudshell-networking-juniper-6.0.1/.tox/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-29 15:11:48.000000 cloudshell-networking-juniper-6.0.1/.tox/build/.tox-info.json
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-29 15:11:57.323769 cloudshell-networking-juniper-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.311769 cloudshell-networking-juniper-6.0.1/cloudshell/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.311769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.311769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.311769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.311769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/generic/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/junos_generic_snmp_autoload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.315769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/HCNUM-TC.json
+-rw-r--r--   0 runner    (1001) docker     (123)   657494 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-CHASSIS-DEFINES-MIB.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30839 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-IF-MIB.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-L2CP-FEATURES-MIB.json
+-rw-r--r--   0 runner    (1001) docker     (123)    90661 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-MIB.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17568 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-SMI.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.315769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/snmp_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/snmp_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/snmp_tables/mibs_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.315769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/juniper_cli_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/juniper_command_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/juniper_ssh_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/juniper_telnet_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.315769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/add_remove_vlan_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/commit_rollback_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/enable_disable_snmp_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/enable_disable_snmp_v3_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/save_restore_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/system_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.315769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/add_remove_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/commit_rollback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/enable_disable_snmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/enable_disable_snmp_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/generic_action_error_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/save_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/system_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/autoload_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/configuration_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/connectivity_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/juniper_enable_disable_snmp_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/juniper_firmware_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/juniper_state_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/helpers/add_remove_vlan_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/helpers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/cloudshell_networking_juniper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-29 15:11:57.000000 cloudshell-networking-juniper-6.0.1/cloudshell_networking_juniper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-29 15:11:57.000000 cloudshell-networking-juniper-6.0.1/cloudshell_networking_juniper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:11:57.000000 cloudshell-networking-juniper-6.0.1/cloudshell_networking_juniper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-29 15:11:57.000000 cloudshell-networking-juniper-6.0.1/cloudshell_networking_juniper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 15:11:57.000000 cloudshell-networking-juniper-6.0.1/cloudshell_networking_juniper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:11:57.323769 cloudshell-networking-juniper-6.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/tests/networking/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/autoload/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/autoload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/cli/test_juniper_ssh_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/cli/test_juniper_telnet_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_add_remove_vlan_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_commit_rollback_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_enable_disable_snmp_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_save_restore_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_system_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.319769 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.323769 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/flows/test_juniper_enable_disable_snmp_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.323769 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/helpers/test_add_remove_vlan_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:11:57.323769 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/snmp/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tests/networking/juniper/snmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 15:11:41.000000 cloudshell-networking-juniper-6.0.1/version.txt
```

### Comparing `cloudshell-networking-juniper-6.0.0/.tox/build/.tox-info.json` & `cloudshell-networking-juniper-6.0.1/.tox/build/.tox-info.json`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/README.md` & `cloudshell-networking-juniper-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/generic/entities.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/generic/entities.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/junos_generic_snmp_autoload.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/junos_generic_snmp_autoload.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/mibs/HCNUM-TC.json` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/HCNUM-TC.json`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/mibs/JUNIPER-CHASSIS-DEFINES-MIB.json` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-CHASSIS-DEFINES-MIB.json`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/mibs/JUNIPER-IF-MIB.json` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-IF-MIB.json`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/mibs/JUNIPER-L2CP-FEATURES-MIB.json` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-L2CP-FEATURES-MIB.json`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/mibs/JUNIPER-MIB.json` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-MIB.json`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/mibs/JUNIPER-SMI.json` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/mibs/JUNIPER-SMI.json`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/autoload/snmp_tables/mibs_conf.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/autoload/snmp_tables/mibs_conf.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/cli/juniper_cli_configurator.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/juniper_cli_configurator.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/cli/juniper_command_modes.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/juniper_command_modes.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/cli/juniper_ssh_session.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/juniper_ssh_session.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/cli/juniper_telnet_session.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/cli/juniper_telnet_session.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_actions/add_remove_vlan_actions.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/add_remove_vlan_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_actions/commit_rollback_actions.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/commit_rollback_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_actions/enable_disable_snmp_actions.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/enable_disable_snmp_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_actions/enable_disable_snmp_v3_actions.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/enable_disable_snmp_v3_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_actions/save_restore_actions.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/save_restore_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_actions/system_actions.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_actions/system_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_templates/add_remove_vlan.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/add_remove_vlan.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_templates/enable_disable_snmp.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/enable_disable_snmp.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_templates/enable_disable_snmp_v3.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/enable_disable_snmp_v3.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_templates/save_restore.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/save_restore.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/command_templates/system_commands.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/command_templates/system_commands.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/flows/autoload_flow.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/autoload_flow.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/flows/configuration_flow.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/configuration_flow.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,16 +76,18 @@
             raise NotSupportedJunOSError("TFTP is not supported by JunOS")
 
         logger.info(f"Save configuration to {file_dst_url}")
 
         with self.cli_configurator.config_mode_service() as cli_service:
             save_action = SaveRestoreActions(cli_service)
             password = file_dst_url.password
+            # JunOS doesn't support password in URL for SCP
             file_dst_url.password = None
             save_action.save_running(str(file_dst_url), password)
+            file_dst_url.password = password
 
     def _restore_flow(
         self,
         config_path: Url,
         configuration_type: ConfigurationType,
         restore_method: RestoreMethod,
         vrf_management_name: str | None,
@@ -110,18 +112,21 @@
         else:
             restore_type = "override"
 
         with self.cli_configurator.config_mode_service() as cli_service:
             restore_actions = SaveRestoreActions(cli_service)
             commit_rollback_actions = CommitRollbackActions(cli_service)
 
+            # JunOS doesn't support password in URL for SCP
             password = config_path.password
             config_path.password = None
             try:
                 restore_actions.restore_running(
                     restore_type, str(config_path), password
                 )
                 # wait longer for applying changes
                 commit_rollback_actions.commit(timeout=120)
             except CommandExecutionException:
                 commit_rollback_actions.rollback()
                 raise
+            finally:
+                config_path.password = password
```

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/flows/connectivity_flow.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/connectivity_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,40 +76,45 @@
                             raise Exception(
                                 self.__class__.__name__,
                                 "QNQ vlans already exist in vlan range intersection",
                             )
                     for _range in new_range_cutoff:
                         vlan_actions.create_vlan(_range.name, _range.to_string())
 
-                vlan_actions.clean_port(port)
                 vlan_actions.assign_member(port, vlan_range, port_mode)
                 commit_rollback_actions.commit(timeout=120)
                 return ConnectivityActionResult.success_result(action, "Success")
             except CommandExecutionException:
                 commit_rollback_actions.rollback()
                 raise
 
     def _remove_vlan(self, action: ConnectivityActionModel) -> ConnectivityActionResult:
         vlan_range = action.connection_params.vlan_id
         port_name = action.action_target.name
         port = AddRemoveVlanHelper.extract_port_name(port_name)
         with self._cli_configurator.config_mode_service() as cli_service:
             commit_rollback_actions = CommitRollbackActions(cli_service)
             vlan_actions = AddRemoveVlanActions(cli_service)
+
             try:
-                existing_ranges = VlanRangeOperations.create_from_dict(
-                    vlan_actions.get_vlans()
-                )
-                range_instance = VlanRange(VlanRange.range_from_string(vlan_range))
-                range_intersection = VlanRangeOperations.find_intersection(
-                    [range_instance], existing_ranges
-                )
+                if not vlan_range:  # remove all VLANs from port
+                    vlan_actions.clean_port(port)
+                    commit_rollback_actions.commit()
+                else:
+                    existing_ranges = VlanRangeOperations.create_from_dict(
+                        vlan_actions.get_vlans()
+                    )
+                    range_instance = VlanRange(VlanRange.range_from_string(vlan_range))
+                    range_intersection = VlanRangeOperations.find_intersection(
+                        [range_instance], existing_ranges
+                    )
 
-                vlan_actions.delete_member(port, vlan_range)
-                commit_rollback_actions.commit()
-                for _range in range_intersection:
-                    vlan_actions.delete_vlan(_range.name)
-                commit_rollback_actions.commit()
-                return ConnectivityActionResult.success_result(action, "Success")
+                    vlan_actions.delete_member(port, vlan_range)
+                    commit_rollback_actions.commit()
+                    for _range in range_intersection:
+                        vlan_actions.delete_vlan(_range.name)
+                    commit_rollback_actions.commit()
             except CommandExecutionException:
                 commit_rollback_actions.rollback()
                 raise
+
+        return ConnectivityActionResult.success_result(action, "Success")
```

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/flows/juniper_enable_disable_snmp_flow.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/juniper_enable_disable_snmp_flow.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/flows/juniper_firmware_flow.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/flows/juniper_firmware_flow.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell/networking/juniper/helpers/add_remove_vlan_helper.py` & `cloudshell-networking-juniper-6.0.1/cloudshell/networking/juniper/helpers/add_remove_vlan_helper.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/cloudshell_networking_juniper.egg-info/SOURCES.txt` & `cloudshell-networking-juniper-6.0.1/cloudshell_networking_juniper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/setup.py` & `cloudshell-networking-juniper-6.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/tests/networking/juniper/cli/test_juniper_ssh_session.py` & `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/cli/test_juniper_ssh_session.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/tests/networking/juniper/cli/test_juniper_telnet_session.py` & `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/cli/test_juniper_telnet_session.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/tests/networking/juniper/command_actions/test_add_remove_vlan_actions.py` & `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_add_remove_vlan_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/tests/networking/juniper/command_actions/test_commit_rollback_actions.py` & `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_commit_rollback_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/tests/networking/juniper/command_actions/test_enable_disable_snmp_actions.py` & `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_enable_disable_snmp_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/tests/networking/juniper/command_actions/test_save_restore_actions.py` & `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_save_restore_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/tests/networking/juniper/command_actions/test_system_actions.py` & `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/command_actions/test_system_actions.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/tests/networking/juniper/flows/test_juniper_enable_disable_snmp_flow.py` & `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/flows/test_juniper_enable_disable_snmp_flow.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/tests/networking/juniper/helpers/test_add_remove_vlan_helper.py` & `cloudshell-networking-juniper-6.0.1/tests/networking/juniper/helpers/test_add_remove_vlan_helper.py`

 * *Files identical despite different names*

### Comparing `cloudshell-networking-juniper-6.0.0/tox.ini` & `cloudshell-networking-juniper-6.0.1/tox.ini`

 * *Files identical despite different names*

