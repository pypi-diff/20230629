# Comparing `tmp/facts_finder-0.0.8.tar.gz` & `tmp/facts_finder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facts_finder-0.0.8.tar", last modified: Thu Feb  2 13:34:55 2023, max compression
+gzip compressed data, was "facts_finder-0.0.9.tar", last modified: Sat Feb 25 09:07:05 2023, max compression
```

## Comparing `facts_finder-0.0.8.tar` & `facts_finder-0.0.9.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-02-02 13:34:55.329396 facts_finder-0.0.8/
--rw-rw-rw-   0        0        0     1091 2022-07-10 12:41:56.000000 facts_finder-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      627 2023-02-02 13:34:55.328397 facts_finder-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      170 2022-07-10 12:41:56.000000 facts_finder-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-02 13:34:54.971014 facts_finder-0.0.8/facts_finder/
--rw-rw-rw-   0        0        0      433 2023-02-02 13:33:45.000000 facts_finder-0.0.8/facts_finder/__init__.py
--rw-rw-rw-   0        0        0     3718 2023-02-02 13:23:44.000000 facts_finder-0.0.8/facts_finder/clean.py
-drwxrwxrwx   0        0        0        0 2023-02-02 13:34:55.032223 facts_finder-0.0.8/facts_finder/generators/
--rw-rw-rw-   0        0        0      255 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-02 13:34:55.107180 facts_finder-0.0.8/facts_finder/generators/cisco/
--rw-rw-rw-   0        0        0      698 2023-02-02 13:23:54.000000 facts_finder-0.0.8/facts_finder/generators/cisco/__init__.py
--rw-rw-rw-   0        0        0     1257 2023-02-02 13:23:54.000000 facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_arp_table.py
--rw-rw-rw-   0        0        0     6162 2023-02-02 13:23:54.000000 facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_bgp.py
--rw-rw-rw-   0        0        0     1901 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_cdp.py
--rw-rw-rw-   0        0        0     1133 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_int_description.py
--rw-rw-rw-   0        0        0     1728 2023-02-02 13:23:54.000000 facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_int_status.py
--rw-rw-rw-   0        0        0     1734 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_lldp.py
--rw-rw-rw-   0        0        0     1352 2023-02-02 13:23:54.000000 facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_mac_table.py
--rw-rw-rw-   0        0        0     6688 2023-02-02 13:23:54.000000 facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_running_interfaces.py
--rw-rw-rw-   0        0        0     4501 2023-02-02 13:23:54.000000 facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_running_system.py
--rw-rw-rw-   0        0        0     2602 2023-02-02 13:23:54.000000 facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_running_vrfs.py
--rw-rw-rw-   0        0        0     1236 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_version.py
--rw-rw-rw-   0        0        0     6663 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/cisco/common.py
--rw-rw-rw-   0        0        0     6397 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/cisco_parser.py
--rw-rw-rw-   0        0        0      252 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/device.py
--rw-rw-rw-   0        0        0     1853 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/facts_gen.py
-drwxrwxrwx   0        0        0        0 2023-02-02 13:34:55.182503 facts_finder-0.0.8/facts_finder/generators/juniper/
--rw-rw-rw-   0        0        0      647 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/juniper/__init__.py
--rw-rw-rw-   0        0        0     2219 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_arp_table.py
--rw-rw-rw-   0        0        0     2758 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_chassis_hardware.py
--rw-rw-rw-   0        0        0     1146 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_int_description.py
--rw-rw-rw-   0        0        0     1613 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_lldp.py
--rw-rw-rw-   0        0        0      406 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_running.py
--rw-rw-rw-   0        0        0     6832 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_running_bgp.py
--rw-rw-rw-   0        0        0    14900 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_running_interfaces.py
--rw-rw-rw-   0        0        0     3269 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_running_routing_instances.py
--rw-rw-rw-   0        0        0     7607 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_running_system.py
--rw-rw-rw-   0        0        0     1043 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_version.py
--rw-rw-rw-   0        0        0     1568 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/juniper/common.py
--rw-rw-rw-   0        0        0     5323 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/juniper_parser.py
--rw-rw-rw-   0        0        0     3539 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/generators/merger.py
-drwxrwxrwx   0        0        0        0 2023-02-02 13:34:55.214266 facts_finder-0.0.8/facts_finder/mergers/
--rw-rw-rw-   0        0        0      199 2023-02-02 13:23:52.000000 facts_finder-0.0.8/facts_finder/mergers/__init__.py
--rw-rw-rw-   0        0        0      945 2023-02-02 13:23:52.000000 facts_finder-0.0.8/facts_finder/mergers/cisco.py
--rw-rw-rw-   0        0        0     4714 2023-02-02 13:23:52.000000 facts_finder-0.0.8/facts_finder/mergers/common.py
--rw-rw-rw-   0        0        0     1544 2023-02-02 13:23:52.000000 facts_finder-0.0.8/facts_finder/mergers/juniper.py
-drwxrwxrwx   0        0        0        0 2023-02-02 13:34:55.220253 facts_finder-0.0.8/facts_finder/modifiers/
--rw-rw-rw-   0        0        0      139 2023-02-02 13:23:52.000000 facts_finder-0.0.8/facts_finder/modifiers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-02 13:34:55.246362 facts_finder-0.0.8/facts_finder/modifiers/cisco/
--rw-rw-rw-   0        0        0      345 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/modifiers/cisco/__init__.py
--rw-rw-rw-   0        0        0     6565 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/modifiers/cisco/cisco_tables.py
--rw-rw-rw-   0        0        0     1425 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/modifiers/cisco/cisco_var.py
--rw-rw-rw-   0        0        0     1250 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/modifiers/cisco/cisco_vrfs.py
-drwxrwxrwx   0        0        0        0 2023-02-02 13:34:55.259175 facts_finder-0.0.8/facts_finder/modifiers/cisco/commands/
--rw-rw-rw-   0        0        0        0 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/modifiers/cisco/commands/__init__.py
--rw-rw-rw-   0        0        0     3248 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/modifiers/cisco/commands/cmd_dict.py
--rw-rw-rw-   0        0        0     2353 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/modifiers/cisco/merger.py
-drwxrwxrwx   0        0        0        0 2023-02-02 13:34:55.272180 facts_finder-0.0.8/facts_finder/modifiers/commons/
--rw-rw-rw-   0        0        0      303 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/modifiers/commons/__init__.py
--rw-rw-rw-   0        0        0     5750 2023-02-02 13:23:52.000000 facts_finder-0.0.8/facts_finder/modifiers/commons/modifier_commons.py
-drwxrwxrwx   0        0        0        0 2023-02-02 13:34:55.294117 facts_finder-0.0.8/facts_finder/modifiers/juniper/
--rw-rw-rw-   0        0        0      303 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/modifiers/juniper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-02 13:34:55.326433 facts_finder-0.0.8/facts_finder/modifiers/juniper/commands/
--rw-rw-rw-   0        0        0        0 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/modifiers/juniper/commands/__init__.py
--rw-rw-rw-   0        0        0     1201 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/modifiers/juniper/commands/cmd_dict.py
--rw-rw-rw-   0        0        0     2045 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/modifiers/juniper/juniper_tables.py
--rw-rw-rw-   0        0        0      764 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/modifiers/juniper/juniper_var.py
--rw-rw-rw-   0        0        0     1849 2023-02-02 13:23:53.000000 facts_finder-0.0.8/facts_finder/modifiers/juniper/merger.py
--rw-rw-rw-   0        0        0     2868 2023-02-02 13:23:44.000000 facts_finder-0.0.8/facts_finder/rearrange.py
-drwxrwxrwx   0        0        0        0 2023-02-02 13:34:54.990262 facts_finder-0.0.8/facts_finder.egg-info/
--rw-rw-rw-   0        0        0      627 2023-02-02 13:34:54.000000 facts_finder-0.0.8/facts_finder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2712 2023-02-02 13:34:54.000000 facts_finder-0.0.8/facts_finder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-02 13:34:54.000000 facts_finder-0.0.8/facts_finder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-02-02 13:34:54.000000 facts_finder-0.0.8/facts_finder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-02 13:34:54.000000 facts_finder-0.0.8/facts_finder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-02 13:34:55.330396 facts_finder-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      970 2023-02-02 13:33:24.000000 facts_finder-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-25 09:07:05.216586 facts_finder-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2022-07-10 12:41:56.000000 facts_finder-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      627 2023-02-25 09:07:05.215580 facts_finder-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2022-07-10 12:41:56.000000 facts_finder-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-25 09:07:04.657174 facts_finder-0.0.9/facts_finder/
+-rw-rw-rw-   0        0        0      433 2023-02-25 08:00:11.000000 facts_finder-0.0.9/facts_finder/__init__.py
+-rw-rw-rw-   0        0        0     3718 2023-02-25 07:55:54.000000 facts_finder-0.0.9/facts_finder/clean.py
+drwxrwxrwx   0        0        0        0 2023-02-25 09:07:04.745553 facts_finder-0.0.9/facts_finder/generators/
+-rw-rw-rw-   0        0        0      255 2023-02-25 07:56:15.000000 facts_finder-0.0.9/facts_finder/generators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-25 09:07:04.870606 facts_finder-0.0.9/facts_finder/generators/cisco/
+-rw-rw-rw-   0        0        0      698 2023-02-25 07:56:37.000000 facts_finder-0.0.9/facts_finder/generators/cisco/__init__.py
+-rw-rw-rw-   0        0        0     1257 2023-02-25 07:56:37.000000 facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_arp_table.py
+-rw-rw-rw-   0        0        0     6162 2023-02-25 07:56:37.000000 facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_bgp.py
+-rw-rw-rw-   0        0        0     1901 2023-02-25 07:56:37.000000 facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_cdp.py
+-rw-rw-rw-   0        0        0     1133 2023-02-25 07:56:37.000000 facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_int_description.py
+-rw-rw-rw-   0        0        0     1728 2023-02-25 07:56:37.000000 facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_int_status.py
+-rw-rw-rw-   0        0        0     1734 2023-02-25 07:56:37.000000 facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_lldp.py
+-rw-rw-rw-   0        0        0     1352 2023-02-25 07:56:37.000000 facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_mac_table.py
+-rw-rw-rw-   0        0        0     7578 2023-02-25 07:56:37.000000 facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_running_interfaces.py
+-rw-rw-rw-   0        0        0     4502 2023-02-25 07:56:37.000000 facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_running_system.py
+-rw-rw-rw-   0        0        0     2602 2023-02-25 07:56:37.000000 facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_running_vrfs.py
+-rw-rw-rw-   0        0        0     1236 2023-02-25 07:56:37.000000 facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_version.py
+-rw-rw-rw-   0        0        0     6663 2023-02-25 07:56:37.000000 facts_finder-0.0.9/facts_finder/generators/cisco/common.py
+-rw-rw-rw-   0        0        0     6397 2023-02-25 07:56:15.000000 facts_finder-0.0.9/facts_finder/generators/cisco_parser.py
+-rw-rw-rw-   0        0        0      252 2023-02-25 07:56:15.000000 facts_finder-0.0.9/facts_finder/generators/device.py
+-rw-rw-rw-   0        0        0     1853 2023-02-25 07:56:15.000000 facts_finder-0.0.9/facts_finder/generators/facts_gen.py
+drwxrwxrwx   0        0        0        0 2023-02-25 09:07:04.989157 facts_finder-0.0.9/facts_finder/generators/juniper/
+-rw-rw-rw-   0        0        0      647 2023-02-25 07:56:58.000000 facts_finder-0.0.9/facts_finder/generators/juniper/__init__.py
+-rw-rw-rw-   0        0        0     2219 2023-02-25 07:56:58.000000 facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_arp_table.py
+-rw-rw-rw-   0        0        0     2758 2023-02-25 07:56:58.000000 facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_chassis_hardware.py
+-rw-rw-rw-   0        0        0     1146 2023-02-25 07:56:58.000000 facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_int_description.py
+-rw-rw-rw-   0        0        0     1613 2023-02-25 07:56:58.000000 facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_lldp.py
+-rw-rw-rw-   0        0        0      406 2023-02-25 07:56:58.000000 facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_running.py
+-rw-rw-rw-   0        0        0     6832 2023-02-25 07:56:58.000000 facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_running_bgp.py
+-rw-rw-rw-   0        0        0    14900 2023-02-25 07:56:58.000000 facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_running_interfaces.py
+-rw-rw-rw-   0        0        0     3269 2023-02-25 07:56:58.000000 facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_running_routing_instances.py
+-rw-rw-rw-   0        0        0     7607 2023-02-25 07:56:58.000000 facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_running_system.py
+-rw-rw-rw-   0        0        0     1043 2023-02-25 07:56:58.000000 facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_version.py
+-rw-rw-rw-   0        0        0     1568 2023-02-25 07:56:58.000000 facts_finder-0.0.9/facts_finder/generators/juniper/common.py
+-rw-rw-rw-   0        0        0     5323 2023-02-25 07:56:15.000000 facts_finder-0.0.9/facts_finder/generators/juniper_parser.py
+-rw-rw-rw-   0        0        0     3539 2023-02-25 07:56:15.000000 facts_finder-0.0.9/facts_finder/generators/merger.py
+drwxrwxrwx   0        0        0        0 2023-02-25 09:07:05.025380 facts_finder-0.0.9/facts_finder/mergers/
+-rw-rw-rw-   0        0        0      199 2023-02-25 07:57:38.000000 facts_finder-0.0.9/facts_finder/mergers/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-02-25 07:57:38.000000 facts_finder-0.0.9/facts_finder/mergers/cisco.py
+-rw-rw-rw-   0        0        0     4714 2023-02-25 07:57:38.000000 facts_finder-0.0.9/facts_finder/mergers/common.py
+-rw-rw-rw-   0        0        0     1544 2023-02-25 07:57:38.000000 facts_finder-0.0.9/facts_finder/mergers/juniper.py
+drwxrwxrwx   0        0        0        0 2023-02-25 09:07:05.035356 facts_finder-0.0.9/facts_finder/modifiers/
+-rw-rw-rw-   0        0        0      139 2023-02-25 07:57:50.000000 facts_finder-0.0.9/facts_finder/modifiers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-25 09:07:05.093908 facts_finder-0.0.9/facts_finder/modifiers/cisco/
+-rw-rw-rw-   0        0        0      345 2023-02-25 07:58:24.000000 facts_finder-0.0.9/facts_finder/modifiers/cisco/__init__.py
+-rw-rw-rw-   0        0        0     6565 2023-02-25 07:58:24.000000 facts_finder-0.0.9/facts_finder/modifiers/cisco/cisco_tables.py
+-rw-rw-rw-   0        0        0     1425 2023-02-25 07:58:24.000000 facts_finder-0.0.9/facts_finder/modifiers/cisco/cisco_var.py
+-rw-rw-rw-   0        0        0     1250 2023-02-25 07:58:24.000000 facts_finder-0.0.9/facts_finder/modifiers/cisco/cisco_vrfs.py
+drwxrwxrwx   0        0        0        0 2023-02-25 09:07:05.112857 facts_finder-0.0.9/facts_finder/modifiers/cisco/commands/
+-rw-rw-rw-   0        0        0        0 2023-02-25 07:58:37.000000 facts_finder-0.0.9/facts_finder/modifiers/cisco/commands/__init__.py
+-rw-rw-rw-   0        0        0     3248 2023-02-25 07:58:38.000000 facts_finder-0.0.9/facts_finder/modifiers/cisco/commands/cmd_dict.py
+-rw-rw-rw-   0        0        0     2353 2023-02-25 07:58:24.000000 facts_finder-0.0.9/facts_finder/modifiers/cisco/merger.py
+drwxrwxrwx   0        0        0        0 2023-02-25 09:07:05.139783 facts_finder-0.0.9/facts_finder/modifiers/commons/
+-rw-rw-rw-   0        0        0      303 2023-02-25 07:59:02.000000 facts_finder-0.0.9/facts_finder/modifiers/commons/__init__.py
+-rw-rw-rw-   0        0        0     5750 2023-02-25 07:59:02.000000 facts_finder-0.0.9/facts_finder/modifiers/commons/modifier_commons.py
+drwxrwxrwx   0        0        0        0 2023-02-25 09:07:05.196638 facts_finder-0.0.9/facts_finder/modifiers/juniper/
+-rw-rw-rw-   0        0        0      303 2023-02-25 07:59:22.000000 facts_finder-0.0.9/facts_finder/modifiers/juniper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-25 09:07:05.213586 facts_finder-0.0.9/facts_finder/modifiers/juniper/commands/
+-rw-rw-rw-   0        0        0        0 2023-02-25 07:59:37.000000 facts_finder-0.0.9/facts_finder/modifiers/juniper/commands/__init__.py
+-rw-rw-rw-   0        0        0     1201 2023-02-25 07:59:37.000000 facts_finder-0.0.9/facts_finder/modifiers/juniper/commands/cmd_dict.py
+-rw-rw-rw-   0        0        0     2045 2023-02-25 07:59:22.000000 facts_finder-0.0.9/facts_finder/modifiers/juniper/juniper_tables.py
+-rw-rw-rw-   0        0        0      764 2023-02-25 07:59:22.000000 facts_finder-0.0.9/facts_finder/modifiers/juniper/juniper_var.py
+-rw-rw-rw-   0        0        0     1849 2023-02-25 07:59:22.000000 facts_finder-0.0.9/facts_finder/modifiers/juniper/merger.py
+-rw-rw-rw-   0        0        0     2964 2023-02-25 07:55:54.000000 facts_finder-0.0.9/facts_finder/rearrange.py
+drwxrwxrwx   0        0        0        0 2023-02-25 09:07:04.678372 facts_finder-0.0.9/facts_finder.egg-info/
+-rw-rw-rw-   0        0        0      627 2023-02-25 09:07:04.000000 facts_finder-0.0.9/facts_finder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2712 2023-02-25 09:07:04.000000 facts_finder-0.0.9/facts_finder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-25 09:07:04.000000 facts_finder-0.0.9/facts_finder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-02-25 09:07:04.000000 facts_finder-0.0.9/facts_finder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-02-25 09:07:04.000000 facts_finder-0.0.9/facts_finder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-02-25 09:07:05.216586 facts_finder-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      970 2023-02-25 08:02:57.000000 facts_finder-0.0.9/setup.py
```

### Comparing `facts_finder-0.0.8/LICENSE` & `facts_finder-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/PKG-INFO` & `facts_finder-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facts_finder
-Version: 0.0.8
+Version: 0.0.9
 Summary: facts_finder for Networking Geeks
 Home-page: https://github.com/alias1978/facts_finder
 Author: ALIASGAR - ALI
 Author-email: aholo2000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `facts_finder-0.0.8/facts_finder/clean.py` & `facts_finder-0.0.9/facts_finder/clean.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/cisco/__init__.py` & `facts_finder-0.0.9/facts_finder/generators/cisco/__init__.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_arp_table.py` & `facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_arp_table.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_bgp.py` & `facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_bgp.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_cdp.py` & `facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_cdp.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_int_description.py` & `facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_int_description.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_int_status.py` & `facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_int_status.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_lldp.py` & `facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_lldp.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_mac_table.py` & `facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_mac_table.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_running_interfaces.py` & `facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_running_interfaces.py`

 * *Files 14% similar despite different names*

```diff
@@ -206,14 +206,40 @@
 			port_dict['ospf_auth_type'] = l.strip().split()[-1]
 		if not auth and not auth_type: return None
 
 	def interface_ospf_auth(self):
 		func = self.get_int_ospf_auth
 		merge_dict(self.interface_dict, self.interface_read(func))
 
+
+	@staticmethod
+	def get_interface_v4_helpers(port_dict, l):
+		if l.strip().startswith("ip helper-address"):
+			if not port_dict.get('v4_helpers'):
+				port_dict['v4_helpers'] = l.strip().split()[-1]
+			else:
+				port_dict['v4_helpers'] += '\n'+l.strip().split()[-1]
+
+	def interface_v4_helpers(self):
+		func = self.get_interface_v4_helpers
+		merge_dict(self.interface_dict, self.interface_read(func))
+
+	@staticmethod
+	def get_interface_v6_helpers(port_dict, l):
+		if l.strip().startswith("ipv6 dhcp relay destination"):
+			if not port_dict.get('v6_helpers'):
+				port_dict['v6_helpers'] = l.strip().split()[-1]
+			else:
+				port_dict['v6_helpers'] += '\n'+l.strip().split()[-1]
+
+	def interface_v6_helpers(self):
+		func = self.get_interface_v6_helpers
+		merge_dict(self.interface_dict, self.interface_read(func))
+
+
 	# # Add more interface related methods as needed.
 
 
 # ------------------------------------------------------------------------------
 
 
 def get_interfaces_running(cmd_op, *args):
@@ -226,18 +252,19 @@
 	Returns:
 		dict: output dictionary with parsed with system fields
 	"""    	
 	R  = RunningInterfaces(cmd_op)
 	# R.interface_ips()
 	# R.interface_v6_ips()
 	# R.interface_vlans()
-	# R.interface_channel_group()
+	R.interface_channel_group()
 	# R.interface_vrf()
 	R.interface_ospf_auth()
 	R.interface_udld()
+	R.interface_v4_helpers()
+	R.interface_v6_helpers()
 
 	# # update more interface related methods as needed.
-
 	if not R.interface_dict:
 		R.interface_dict['dummy_int'] = ""
 	return R.interface_dict
```

### Comparing `facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_running_system.py` & `facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_running_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 				if 'key' in spl:
 					i = spl.index('key')
 					if str(spl[i+1]) == '7':
 						key = decrypt_type7(spl[i+2])
 					else:
 						key = spl[i+1]
 				if 'port' in spl:
-					port = spl[spl.index('key')+1]
+					port = spl[spl.index('port')+1]
 		dic = {}
 		for i, srv in enumerate(servers):
 			dic['tacacs_server_' + str(i+1)] = srv
 		dic['tacacs_key'] = key
 		dic['tacacs_tcp_port'] = port
 		return dic
```

### Comparing `facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_running_vrfs.py` & `facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_running_vrfs.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/cisco/_cmd_parse_version.py` & `facts_finder-0.0.9/facts_finder/generators/cisco/_cmd_parse_version.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/cisco/common.py` & `facts_finder-0.0.9/facts_finder/generators/cisco/common.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/cisco_parser.py` & `facts_finder-0.0.9/facts_finder/generators/cisco_parser.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/facts_gen.py` & `facts_finder-0.0.9/facts_finder/generators/facts_gen.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/juniper/__init__.py` & `facts_finder-0.0.9/facts_finder/generators/juniper/__init__.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_arp_table.py` & `facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_arp_table.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_chassis_hardware.py` & `facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_chassis_hardware.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_int_description.py` & `facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_int_description.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_lldp.py` & `facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_lldp.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_running_bgp.py` & `facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_running_bgp.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_running_interfaces.py` & `facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_running_interfaces.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_running_routing_instances.py` & `facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_running_routing_instances.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_running_system.py` & `facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_running_system.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/juniper/_cmd_parse_version.py` & `facts_finder-0.0.9/facts_finder/generators/juniper/_cmd_parse_version.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/juniper/common.py` & `facts_finder-0.0.9/facts_finder/generators/juniper/common.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/juniper_parser.py` & `facts_finder-0.0.9/facts_finder/generators/juniper_parser.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/generators/merger.py` & `facts_finder-0.0.9/facts_finder/generators/merger.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/mergers/cisco.py` & `facts_finder-0.0.9/facts_finder/mergers/cisco.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/mergers/common.py` & `facts_finder-0.0.9/facts_finder/mergers/common.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/mergers/juniper.py` & `facts_finder-0.0.9/facts_finder/mergers/juniper.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/modifiers/cisco/cisco_tables.py` & `facts_finder-0.0.9/facts_finder/modifiers/cisco/cisco_tables.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/modifiers/cisco/cisco_var.py` & `facts_finder-0.0.9/facts_finder/modifiers/cisco/cisco_var.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/modifiers/cisco/cisco_vrfs.py` & `facts_finder-0.0.9/facts_finder/modifiers/cisco/cisco_vrfs.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/modifiers/cisco/commands/cmd_dict.py` & `facts_finder-0.0.9/facts_finder/modifiers/cisco/commands/cmd_dict.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/modifiers/cisco/merger.py` & `facts_finder-0.0.9/facts_finder/modifiers/cisco/merger.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/modifiers/commons/modifier_commons.py` & `facts_finder-0.0.9/facts_finder/modifiers/commons/modifier_commons.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/modifiers/juniper/commands/cmd_dict.py` & `facts_finder-0.0.9/facts_finder/modifiers/juniper/commands/cmd_dict.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/modifiers/juniper/juniper_tables.py` & `facts_finder-0.0.9/facts_finder/modifiers/juniper/juniper_tables.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/modifiers/juniper/juniper_var.py` & `facts_finder-0.0.9/facts_finder/modifiers/juniper/juniper_var.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/modifiers/juniper/merger.py` & `facts_finder-0.0.9/facts_finder/modifiers/juniper/merger.py`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/facts_finder/rearrange.py` & `facts_finder-0.0.9/facts_finder/rearrange.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 
 IF_PROPS = {
 	1: ["filter", "interface", "int_number",  ],
 	2: [ "link_status", "protocol_status", "speed", "duplex", "media_type", ],
 	3: ["nbr_dev_type", "nbr_hostname", "nbr_ip", "nbr_platform", "nbr_serial", "nbr_vlan", "nbr_interface",],
 	4: ["switchport", "admin_mode", "switchport_negotiation", "interface_mode", "access_vlan", "voice_vlan", 
 		"native_vlan", "vlan_members",],
-	5: ["subnet", "h4block",],
+	5: ["subnet", "h4block", "v4_helpers", "v6_helpers", ],
 	6: ["ospf_auth", "ospf_auth_type",],
-	7: ["intvrf", "channel_grp",],
+	7: ["intvrf", "channel_group_interface", "channel_grp", "channel_group_mode"],
 	8: ["description", "int_type", "int_filter", "dist_n", "dist_i",  ],
 	9: ["vlan_index", "vlan_type", "vlan_description",],
+	10:["int_udld",]
 }
 
 BGP_PROPS = [ 
 	"filter", "bgp neighbor", "bgp_vrf", "address-family", "bgp_peergrp", "bgp_peer_description", "bgp_peer_password", 
 	"bgp_peer_ip", "bgp_peer_as", "local-as", "update-source", "route-map in", "route-map out", "unsuppress-map",
 ]
```

### Comparing `facts_finder-0.0.8/facts_finder.egg-info/PKG-INFO` & `facts_finder-0.0.9/facts_finder.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facts-finder
-Version: 0.0.8
+Version: 0.0.9
 Summary: facts_finder for Networking Geeks
 Home-page: https://github.com/alias1978/facts_finder
 Author: ALIASGAR - ALI
 Author-email: aholo2000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `facts_finder-0.0.8/facts_finder.egg-info/SOURCES.txt` & `facts_finder-0.0.9/facts_finder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `facts_finder-0.0.8/setup.py` & `facts_finder-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="facts_finder",
-    version="0.0.8",
+    version="0.0.9",
     author="ALIASGAR - ALI",
     author_email="aholo2000@gmail.com",
     description="facts_finder for Networking Geeks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alias1978/facts_finder",
     # package_data={
```

