# Comparing `tmp/ipfabric-6.2.4.tar.gz` & `tmp/ipfabric-6.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric-6.2.4.tar", max compression
+gzip compressed data, was "ipfabric-6.2.5.tar", max compression
```

## Comparing `ipfabric-6.2.4.tar` & `ipfabric-6.2.5.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1790 2023-05-02 13:05:28.009049 ipfabric-6.2.4/ipfabric/__init__.py
--rw-r--r--   0        0        0    17412 2023-06-01 16:01:19.082057 ipfabric-6.2.4/ipfabric/api.py
--rw-r--r--   0        0        0    10890 2023-06-01 16:01:19.085671 ipfabric-6.2.4/ipfabric/client.py
--rw-r--r--   0        0        0      434 2023-06-01 16:01:19.090676 ipfabric-6.2.4/ipfabric/models/__init__.py
--rw-r--r--   0        0        0    14821 2023-06-01 16:04:36.684130 ipfabric-6.2.4/ipfabric/models/device.py
--rw-r--r--   0        0        0     5842 2023-06-01 16:01:19.099648 ipfabric-6.2.4/ipfabric/models/intent.py
--rw-r--r--   0        0        0     2786 2023-04-24 14:44:33.818272 ipfabric-6.2.4/ipfabric/models/intent_check.py
--rw-r--r--   0        0        0     2092 2023-06-01 16:01:19.103555 ipfabric-6.2.4/ipfabric/models/inventory.py
--rw-r--r--   0        0        0     6964 2023-06-01 16:01:19.107556 ipfabric-6.2.4/ipfabric/models/jobs.py
--rw-r--r--   0        0        0    12327 2023-06-01 16:01:19.111651 ipfabric-6.2.4/ipfabric/models/snapshot.py
--rw-r--r--   0        0        0    19209 2023-06-01 16:01:19.116236 ipfabric-6.2.4/ipfabric/models/table.py
--rw-r--r--   0        0        0     2830 2023-04-24 14:44:33.820322 ipfabric-6.2.4/ipfabric/models/technology/__init__.py
--rw-r--r--   0        0        0     1156 2023-04-24 14:44:33.821325 ipfabric-6.2.4/ipfabric/models/technology/addressing.py
--rw-r--r--   0        0        0      488 2023-04-24 14:44:33.821325 ipfabric-6.2.4/ipfabric/models/technology/cloud.py
--rw-r--r--   0        0        0     2173 2023-04-24 14:44:33.821325 ipfabric-6.2.4/ipfabric/models/technology/dhcp.py
--rw-r--r--   0        0        0     1002 2023-04-24 14:44:33.821325 ipfabric-6.2.4/ipfabric/models/technology/fhrp.py
--rw-r--r--   0        0        0     7018 2023-04-24 14:44:33.822322 ipfabric-6.2.4/ipfabric/models/technology/interfaces.py
--rw-r--r--   0        0        0      324 2023-04-24 14:44:33.822322 ipfabric-6.2.4/ipfabric/models/technology/ip_telephony.py
--rw-r--r--   0        0        0      843 2023-04-24 14:44:33.822322 ipfabric-6.2.4/ipfabric/models/technology/load_balancing.py
--rw-r--r--   0        0        0      470 2023-04-24 14:44:33.823320 ipfabric-6.2.4/ipfabric/models/technology/managed_networks.py
--rw-r--r--   0        0        0     5644 2023-04-24 14:44:33.823320 ipfabric-6.2.4/ipfabric/models/technology/management.py
--rw-r--r--   0        0        0     2045 2023-04-24 14:44:33.823320 ipfabric-6.2.4/ipfabric/models/technology/mpls.py
--rw-r--r--   0        0        0     2783 2023-04-24 14:44:33.824322 ipfabric-6.2.4/ipfabric/models/technology/multicast.py
--rw-r--r--   0        0        0      759 2023-04-24 14:44:33.824322 ipfabric-6.2.4/ipfabric/models/technology/neighbors.py
--rw-r--r--   0        0        0      633 2023-04-24 14:44:33.825321 ipfabric-6.2.4/ipfabric/models/technology/oam.py
--rw-r--r--   0        0        0     3529 2023-04-24 14:44:33.825321 ipfabric-6.2.4/ipfabric/models/technology/platforms.py
--rw-r--r--   0        0        0     1231 2023-04-24 14:44:33.826320 ipfabric-6.2.4/ipfabric/models/technology/port_channels.py
--rw-r--r--   0        0        0     1078 2023-04-24 14:44:33.826320 ipfabric-6.2.4/ipfabric/models/technology/qos.py
--rw-r--r--   0        0        0     4773 2023-04-24 14:44:33.827321 ipfabric-6.2.4/ipfabric/models/technology/routing.py
--rw-r--r--   0        0        0     2159 2023-04-24 14:44:33.827321 ipfabric-6.2.4/ipfabric/models/technology/sdn.py
--rw-r--r--   0        0        0      431 2023-04-24 14:44:33.827321 ipfabric-6.2.4/ipfabric/models/technology/sdwan.py
--rw-r--r--   0        0        0     2062 2023-04-24 14:44:33.828325 ipfabric-6.2.4/ipfabric/models/technology/security.py
--rw-r--r--   0        0        0     2228 2023-04-24 14:44:33.828325 ipfabric-6.2.4/ipfabric/models/technology/stp.py
--rw-r--r--   0        0        0      856 2023-04-24 14:44:33.829324 ipfabric-6.2.4/ipfabric/models/technology/vlans.py
--rw-r--r--   0        0        0      867 2023-04-24 14:44:33.829324 ipfabric-6.2.4/ipfabric/models/technology/wireless.py
--rw-r--r--   0        0        0      805 2023-02-09 20:01:36.099334 ipfabric-6.2.4/ipfabric/settings/__init__.py
--rw-r--r--   0        0        0     3602 2023-05-31 13:43:53.851771 ipfabric-6.2.4/ipfabric/settings/api_tokens.py
--rw-r--r--   0        0        0     6187 2023-04-24 14:44:33.840110 ipfabric-6.2.4/ipfabric/settings/attributes.py
--rw-r--r--   0        0        0     8719 2022-12-14 14:57:33.723874 ipfabric-6.2.4/ipfabric/settings/authentication.py
--rw-r--r--   0        0        0     1027 2022-12-14 14:57:33.723874 ipfabric-6.2.4/ipfabric/settings/discovery.py
--rw-r--r--   0        0        0     2096 2023-02-09 20:15:13.578462 ipfabric-6.2.4/ipfabric/settings/seeds.py
--rw-r--r--   0        0        0     1413 2023-04-24 14:44:33.844128 ipfabric-6.2.4/ipfabric/settings/site_separation.py
--rw-r--r--   0        0        0     5247 2023-05-31 13:43:53.858770 ipfabric-6.2.4/ipfabric/settings/user_mgmt.py
--rw-r--r--   0        0        0     1875 2023-04-24 14:44:33.866077 ipfabric-6.2.4/ipfabric/settings/vendor_api.py
--rw-r--r--   0        0        0     6439 2023-04-24 14:44:33.870769 ipfabric-6.2.4/ipfabric/settings/vendor_api_models.py
--rw-r--r--   0        0        0      430 2022-12-12 21:56:50.511542 ipfabric-6.2.4/ipfabric/tools/__init__.py
--rw-r--r--   0        0        0     7876 2023-04-24 14:44:33.876769 ipfabric-6.2.4/ipfabric/tools/configuration.py
--rw-r--r--   0        0        0     5606 2023-01-03 15:30:13.772885 ipfabric-6.2.4/ipfabric/tools/discovery_history.py
--rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.4/ipfabric/tools/factory_defaults/__init__.py
--rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.4/ipfabric/tools/factory_defaults/v4/4/__init__.py
--rw-r--r--   0        0        0     3152 2022-08-18 15:07:02.565190 ipfabric-6.2.4/ipfabric/tools/factory_defaults/v4/4/dashboard.json
--rw-r--r--   0        0        0     5814 2022-08-18 15:07:02.566156 ipfabric-6.2.4/ipfabric/tools/factory_defaults/v4/4/groups.json
--rw-r--r--   0        0        0   121431 2022-08-18 15:07:02.568156 ipfabric-6.2.4/ipfabric/tools/factory_defaults/v4/4/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.4/ipfabric/tools/factory_defaults/v4/__init__.py
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.4/ipfabric/tools/factory_defaults/v5/0/__init__.py
--rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.4/ipfabric/tools/factory_defaults/v5/0/dashboard.json
--rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.4/ipfabric/tools/factory_defaults/v5/0/groups.json
--rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.4/ipfabric/tools/factory_defaults/v5/0/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.4/ipfabric/tools/factory_defaults/v5/__init__.py
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.4/ipfabric/tools/factory_defaults/v6/0/__init__.py
--rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.4/ipfabric/tools/factory_defaults/v6/0/dashboard.json
--rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.4/ipfabric/tools/factory_defaults/v6/0/groups.json
--rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.4/ipfabric/tools/factory_defaults/v6/0/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.4/ipfabric/tools/factory_defaults/v6/__init__.py
--rw-r--r--   0        0        0     4511 2023-04-24 14:44:33.881459 ipfabric-6.2.4/ipfabric/tools/nist.py
--rw-r--r--   0        0        0     5784 2023-04-24 14:44:33.886456 ipfabric-6.2.4/ipfabric/tools/restore_intents.py
--rw-r--r--   0        0        0     2519 2023-04-24 14:44:33.891098 ipfabric-6.2.4/ipfabric/tools/shared.py
--rw-r--r--   0        0        0     2396 2023-04-24 14:44:33.895102 ipfabric-6.2.4/ipfabric/tools/site_seperation_report.py
--rw-r--r--   0        0        0     2573 2023-04-24 14:44:33.902766 ipfabric-6.2.4/ipfabric/tools/vulnerabilities.py
--rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.2.4/LICENSE
--rw-r--r--   0        0        0     2054 2023-06-01 16:07:41.194857 ipfabric-6.2.4/pyproject.toml
--rw-r--r--   0        0        0     3705 2023-04-24 14:44:33.756295 ipfabric-6.2.4/README.md
--rw-r--r--   0        0        0     5280 1970-01-01 00:00:00.000000 ipfabric-6.2.4/setup.py
--rw-r--r--   0        0        0     5192 1970-01-01 00:00:00.000000 ipfabric-6.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1790 2023-05-02 13:05:28.009049 ipfabric-6.2.5/ipfabric/__init__.py
+-rw-r--r--   0        0        0    17412 2023-06-01 16:01:19.082057 ipfabric-6.2.5/ipfabric/api.py
+-rw-r--r--   0        0        0    10890 2023-06-01 16:01:19.085671 ipfabric-6.2.5/ipfabric/client.py
+-rw-r--r--   0        0        0      434 2023-06-01 16:01:19.090676 ipfabric-6.2.5/ipfabric/models/__init__.py
+-rw-r--r--   0        0        0    14821 2023-06-29 11:39:54.725144 ipfabric-6.2.5/ipfabric/models/device.py
+-rw-r--r--   0        0        0     5842 2023-06-01 16:01:19.099648 ipfabric-6.2.5/ipfabric/models/intent.py
+-rw-r--r--   0        0        0     2786 2023-04-24 14:44:33.818272 ipfabric-6.2.5/ipfabric/models/intent_check.py
+-rw-r--r--   0        0        0     2092 2023-06-01 16:01:19.103555 ipfabric-6.2.5/ipfabric/models/inventory.py
+-rw-r--r--   0        0        0     6964 2023-06-01 16:01:19.107556 ipfabric-6.2.5/ipfabric/models/jobs.py
+-rw-r--r--   0        0        0    12327 2023-06-01 16:01:19.111651 ipfabric-6.2.5/ipfabric/models/snapshot.py
+-rw-r--r--   0        0        0    19772 2023-06-29 11:39:54.726143 ipfabric-6.2.5/ipfabric/models/table.py
+-rw-r--r--   0        0        0     2830 2023-04-24 14:44:33.820322 ipfabric-6.2.5/ipfabric/models/technology/__init__.py
+-rw-r--r--   0        0        0     1156 2023-04-24 14:44:33.821325 ipfabric-6.2.5/ipfabric/models/technology/addressing.py
+-rw-r--r--   0        0        0      488 2023-04-24 14:44:33.821325 ipfabric-6.2.5/ipfabric/models/technology/cloud.py
+-rw-r--r--   0        0        0     2173 2023-04-24 14:44:33.821325 ipfabric-6.2.5/ipfabric/models/technology/dhcp.py
+-rw-r--r--   0        0        0     1002 2023-04-24 14:44:33.821325 ipfabric-6.2.5/ipfabric/models/technology/fhrp.py
+-rw-r--r--   0        0        0     7018 2023-04-24 14:44:33.822322 ipfabric-6.2.5/ipfabric/models/technology/interfaces.py
+-rw-r--r--   0        0        0      324 2023-04-24 14:44:33.822322 ipfabric-6.2.5/ipfabric/models/technology/ip_telephony.py
+-rw-r--r--   0        0        0      843 2023-04-24 14:44:33.822322 ipfabric-6.2.5/ipfabric/models/technology/load_balancing.py
+-rw-r--r--   0        0        0      470 2023-04-24 14:44:33.823320 ipfabric-6.2.5/ipfabric/models/technology/managed_networks.py
+-rw-r--r--   0        0        0     5644 2023-04-24 14:44:33.823320 ipfabric-6.2.5/ipfabric/models/technology/management.py
+-rw-r--r--   0        0        0     2045 2023-04-24 14:44:33.823320 ipfabric-6.2.5/ipfabric/models/technology/mpls.py
+-rw-r--r--   0        0        0     2783 2023-04-24 14:44:33.824322 ipfabric-6.2.5/ipfabric/models/technology/multicast.py
+-rw-r--r--   0        0        0      759 2023-04-24 14:44:33.824322 ipfabric-6.2.5/ipfabric/models/technology/neighbors.py
+-rw-r--r--   0        0        0      633 2023-04-24 14:44:33.825321 ipfabric-6.2.5/ipfabric/models/technology/oam.py
+-rw-r--r--   0        0        0     3529 2023-04-24 14:44:33.825321 ipfabric-6.2.5/ipfabric/models/technology/platforms.py
+-rw-r--r--   0        0        0     1231 2023-04-24 14:44:33.826320 ipfabric-6.2.5/ipfabric/models/technology/port_channels.py
+-rw-r--r--   0        0        0     1078 2023-04-24 14:44:33.826320 ipfabric-6.2.5/ipfabric/models/technology/qos.py
+-rw-r--r--   0        0        0     4773 2023-04-24 14:44:33.827321 ipfabric-6.2.5/ipfabric/models/technology/routing.py
+-rw-r--r--   0        0        0     2159 2023-04-24 14:44:33.827321 ipfabric-6.2.5/ipfabric/models/technology/sdn.py
+-rw-r--r--   0        0        0      431 2023-04-24 14:44:33.827321 ipfabric-6.2.5/ipfabric/models/technology/sdwan.py
+-rw-r--r--   0        0        0     2062 2023-04-24 14:44:33.828325 ipfabric-6.2.5/ipfabric/models/technology/security.py
+-rw-r--r--   0        0        0     2228 2023-04-24 14:44:33.828325 ipfabric-6.2.5/ipfabric/models/technology/stp.py
+-rw-r--r--   0        0        0      856 2023-04-24 14:44:33.829324 ipfabric-6.2.5/ipfabric/models/technology/vlans.py
+-rw-r--r--   0        0        0      867 2023-04-24 14:44:33.829324 ipfabric-6.2.5/ipfabric/models/technology/wireless.py
+-rw-r--r--   0        0        0      805 2023-02-09 20:01:36.099334 ipfabric-6.2.5/ipfabric/settings/__init__.py
+-rw-r--r--   0        0        0     3602 2023-05-31 13:43:53.851771 ipfabric-6.2.5/ipfabric/settings/api_tokens.py
+-rw-r--r--   0        0        0     6187 2023-04-24 14:44:33.840110 ipfabric-6.2.5/ipfabric/settings/attributes.py
+-rw-r--r--   0        0        0     8719 2022-12-14 14:57:33.723874 ipfabric-6.2.5/ipfabric/settings/authentication.py
+-rw-r--r--   0        0        0     1027 2022-12-14 14:57:33.723874 ipfabric-6.2.5/ipfabric/settings/discovery.py
+-rw-r--r--   0        0        0     2096 2023-02-09 20:15:13.578462 ipfabric-6.2.5/ipfabric/settings/seeds.py
+-rw-r--r--   0        0        0     1413 2023-04-24 14:44:33.844128 ipfabric-6.2.5/ipfabric/settings/site_separation.py
+-rw-r--r--   0        0        0     5247 2023-05-31 13:43:53.858770 ipfabric-6.2.5/ipfabric/settings/user_mgmt.py
+-rw-r--r--   0        0        0     1875 2023-04-24 14:44:33.866077 ipfabric-6.2.5/ipfabric/settings/vendor_api.py
+-rw-r--r--   0        0        0     6439 2023-04-24 14:44:33.870769 ipfabric-6.2.5/ipfabric/settings/vendor_api_models.py
+-rw-r--r--   0        0        0      430 2022-12-12 21:56:50.511542 ipfabric-6.2.5/ipfabric/tools/__init__.py
+-rw-r--r--   0        0        0     7876 2023-04-24 14:44:33.876769 ipfabric-6.2.5/ipfabric/tools/configuration.py
+-rw-r--r--   0        0        0     5606 2023-01-03 15:30:13.772885 ipfabric-6.2.5/ipfabric/tools/discovery_history.py
+-rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.5/ipfabric/tools/factory_defaults/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v4/4/__init__.py
+-rw-r--r--   0        0        0     3152 2022-08-18 15:07:02.565190 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v4/4/dashboard.json
+-rw-r--r--   0        0        0     5814 2022-08-18 15:07:02.566156 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v4/4/groups.json
+-rw-r--r--   0        0        0   121431 2022-08-18 15:07:02.568156 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v4/4/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v4/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v5/0/__init__.py
+-rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v5/0/dashboard.json
+-rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v5/0/groups.json
+-rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v5/0/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v5/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v6/0/__init__.py
+-rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v6/0/dashboard.json
+-rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v6/0/groups.json
+-rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v6/0/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.5/ipfabric/tools/factory_defaults/v6/__init__.py
+-rw-r--r--   0        0        0     4511 2023-04-24 14:44:33.881459 ipfabric-6.2.5/ipfabric/tools/nist.py
+-rw-r--r--   0        0        0     5784 2023-04-24 14:44:33.886456 ipfabric-6.2.5/ipfabric/tools/restore_intents.py
+-rw-r--r--   0        0        0     2519 2023-04-24 14:44:33.891098 ipfabric-6.2.5/ipfabric/tools/shared.py
+-rw-r--r--   0        0        0     2396 2023-04-24 14:44:33.895102 ipfabric-6.2.5/ipfabric/tools/site_seperation_report.py
+-rw-r--r--   0        0        0     2573 2023-04-24 14:44:33.902766 ipfabric-6.2.5/ipfabric/tools/vulnerabilities.py
+-rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.2.5/LICENSE
+-rw-r--r--   0        0        0     2054 2023-06-29 11:42:31.639411 ipfabric-6.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3705 2023-04-24 14:44:33.756295 ipfabric-6.2.5/README.md
+-rw-r--r--   0        0        0     5280 1970-01-01 00:00:00.000000 ipfabric-6.2.5/setup.py
+-rw-r--r--   0        0        0     5192 1970-01-01 00:00:00.000000 ipfabric-6.2.5/PKG-INFO
```

### Comparing `ipfabric-6.2.4/ipfabric/__init__.py` & `ipfabric-6.2.5/ipfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/api.py` & `ipfabric-6.2.5/ipfabric/api.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/client.py` & `ipfabric-6.2.5/ipfabric/client.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/device.py` & `ipfabric-6.2.5/ipfabric/models/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 
 logger = logging.getLogger("ipfabric")
 
 
 class DeviceConfig(BaseModel):
     status: str
-    current: Optional[str] = Field(alias='currentConfig')
-    start: Optional[str] = Field(alias='startupConfig')
+    current: Optional[str] = Field(alias="currentConfig")
+    start: Optional[str] = Field(alias="startupConfig")
 
 
 class Device(BaseModel):
     attributes: dict
     domain: Optional[str]
     family: Optional[str]
     fqdn: Optional[str]
```

### Comparing `ipfabric-6.2.4/ipfabric/models/intent.py` & `ipfabric-6.2.5/ipfabric/models/intent.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/intent_check.py` & `ipfabric-6.2.5/ipfabric/models/intent_check.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/inventory.py` & `ipfabric-6.2.5/ipfabric/models/inventory.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/jobs.py` & `ipfabric-6.2.5/ipfabric/models/jobs.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/snapshot.py` & `ipfabric-6.2.5/ipfabric/models/snapshot.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/table.py` & `ipfabric-6.2.5/ipfabric/models/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,24 +218,33 @@
             tuple[list, list]: List of columns to use in query, List of columns to use when sorting data
         """
         # get all columns for the table
         table_columns = set(self.client.get_columns(self.endpoint))
 
         # get any nested columns
         nested_cols_for_return = None
-        # get a row of data
-        one_row_of_data = self.fetch(limit=1)
-        # loop over each column in the table columns
-        for col in table_columns:
-            # check if the data returned has nested columns
-            if isinstance(one_row_of_data[0][col], list):
-                # get all the nested column names
-                nested_cols = set(one_row_of_data[0][col][0].keys())
-                # create a set of nested column names requested by the user
-                nested_cols_for_return = {col for col in nested_cols if col in nested_keys}
+        # if the user passed nested_column_returns
+        if nested_keys:
+            # get a row of data
+            one_row_of_data = self.fetch(limit=1)
+            # loop over each column in the table columns
+            for col in table_columns:
+                # check if the data returned has nested columns
+                if isinstance(one_row_of_data[0][col], list):
+                    logger.debug(f"Column: {col}, one row of data: {one_row_of_data}")
+                    check_len_of_data = len(one_row_of_data[0][col])
+                    if check_len_of_data >= 0:
+                        logger.warning(
+                            "Nested Column was Detected, but no data was present to determine if there are any nested columns, skipping"
+                        )
+                        continue
+                    # get all the nested column names
+                    nested_cols = set(one_row_of_data[0][col][0].keys())
+                    # create a set of nested column names requested by the user
+                    nested_cols_for_return = {col for col in nested_cols if col in nested_keys}
 
         # Must always ignore some columns
         columns_ignore.update(IGNORE_COLUMNS)
 
         cols_for_return = set()
         # user passes unique_keys
         if unique_keys:
```

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/__init__.py` & `ipfabric-6.2.5/ipfabric/models/technology/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/addressing.py` & `ipfabric-6.2.5/ipfabric/models/technology/addressing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/dhcp.py` & `ipfabric-6.2.5/ipfabric/models/technology/dhcp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/fhrp.py` & `ipfabric-6.2.5/ipfabric/models/technology/fhrp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/interfaces.py` & `ipfabric-6.2.5/ipfabric/models/technology/interfaces.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/load_balancing.py` & `ipfabric-6.2.5/ipfabric/models/technology/load_balancing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/management.py` & `ipfabric-6.2.5/ipfabric/models/technology/management.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/mpls.py` & `ipfabric-6.2.5/ipfabric/models/technology/mpls.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/multicast.py` & `ipfabric-6.2.5/ipfabric/models/technology/multicast.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/neighbors.py` & `ipfabric-6.2.5/ipfabric/models/technology/neighbors.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/oam.py` & `ipfabric-6.2.5/ipfabric/models/technology/oam.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/platforms.py` & `ipfabric-6.2.5/ipfabric/models/technology/platforms.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/port_channels.py` & `ipfabric-6.2.5/ipfabric/models/technology/port_channels.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/qos.py` & `ipfabric-6.2.5/ipfabric/models/technology/qos.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/routing.py` & `ipfabric-6.2.5/ipfabric/models/technology/routing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/sdn.py` & `ipfabric-6.2.5/ipfabric/models/technology/sdn.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/security.py` & `ipfabric-6.2.5/ipfabric/models/technology/security.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/stp.py` & `ipfabric-6.2.5/ipfabric/models/technology/stp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/vlans.py` & `ipfabric-6.2.5/ipfabric/models/technology/vlans.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/models/technology/wireless.py` & `ipfabric-6.2.5/ipfabric/models/technology/wireless.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/settings/__init__.py` & `ipfabric-6.2.5/ipfabric/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/settings/api_tokens.py` & `ipfabric-6.2.5/ipfabric/settings/api_tokens.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/settings/attributes.py` & `ipfabric-6.2.5/ipfabric/settings/attributes.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/settings/authentication.py` & `ipfabric-6.2.5/ipfabric/settings/authentication.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/settings/discovery.py` & `ipfabric-6.2.5/ipfabric/settings/discovery.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/settings/seeds.py` & `ipfabric-6.2.5/ipfabric/settings/seeds.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/settings/site_separation.py` & `ipfabric-6.2.5/ipfabric/settings/site_separation.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/settings/user_mgmt.py` & `ipfabric-6.2.5/ipfabric/settings/user_mgmt.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/settings/vendor_api.py` & `ipfabric-6.2.5/ipfabric/settings/vendor_api.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/settings/vendor_api_models.py` & `ipfabric-6.2.5/ipfabric/settings/vendor_api_models.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/tools/configuration.py` & `ipfabric-6.2.5/ipfabric/tools/configuration.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/tools/discovery_history.py` & `ipfabric-6.2.5/ipfabric/tools/discovery_history.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/tools/factory_defaults/v4/4/dashboard.json` & `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v4/4/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/tools/factory_defaults/v4/4/groups.json` & `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v4/4/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/tools/factory_defaults/v4/4/intents.json` & `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v4/4/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/tools/factory_defaults/v5/0/dashboard.json` & `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v5/0/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/tools/factory_defaults/v5/0/groups.json` & `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v5/0/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/tools/factory_defaults/v5/0/intents.json` & `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v5/0/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/tools/factory_defaults/v6/0/dashboard.json` & `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v6/0/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/tools/factory_defaults/v6/0/groups.json` & `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v6/0/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/tools/factory_defaults/v6/0/intents.json` & `ipfabric-6.2.5/ipfabric/tools/factory_defaults/v6/0/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/tools/nist.py` & `ipfabric-6.2.5/ipfabric/tools/nist.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/tools/restore_intents.py` & `ipfabric-6.2.5/ipfabric/tools/restore_intents.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/tools/shared.py` & `ipfabric-6.2.5/ipfabric/tools/shared.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/tools/site_seperation_report.py` & `ipfabric-6.2.5/ipfabric/tools/site_seperation_report.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/ipfabric/tools/vulnerabilities.py` & `ipfabric-6.2.5/ipfabric/tools/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/LICENSE` & `ipfabric-6.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/pyproject.toml` & `ipfabric-6.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipfabric"
-version = "v6.2.4"
+version = "v6.2.5"
 description = "Python package for interacting with IP Fabric"
 authors = [
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
     "Cristian Cordero <cristian.cordero@ipfabric.io>",
     "Community Fabric <communityfabric@ipfabric.io>"
 ]
 license = "MIT"
```

### Comparing `ipfabric-6.2.4/README.md` & `ipfabric-6.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.4/setup.py` & `ipfabric-6.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
               'openpyxl>=3.0.9,<4.0.0',
               'tabulate>=0.8.9,<0.10.0',
               'python-json-logger>=2.0.4,<3.0.0',
               'pyyaml>=6.0,<7.0']}
 
 setup_kwargs = {
     'name': 'ipfabric',
-    'version': '6.2.4',
+    'version': '6.2.5',
     'description': 'Python package for interacting with IP Fabric',
     'long_description': '# IP Fabric \n\nIPFabric is a Python module for connecting to and communicating against an IP Fabric instance.\n\n## About\n\nFounded in 2015, [IP Fabric](https://ipfabric.io/) develops network infrastructure visibility and analytics solution to\nhelp enterprise network and security teams with network assurance and automation across multi-domain heterogeneous\nenvironments. From in-depth discovery, through graph visualization, to packet walks and complete network history, IP\nFabric enables to confidently replace manual tasks necessary to handle growing network complexity driven by relentless\ndigital transformation. \n\n## v7.0.0 Deprecation Notices\n\nIn `ipfabric>=v7.0.0` the following will be deprecated:\n\n- `ipfabric_diagrams` package will move to `ipfabric.diagrams`\n- Python 3.7 support will be removed.\n- The use of `token=\'<TOKEN>\'` or `username=\'<USER>\', password=\'<PASS>\'` in `IPFClient()` will be removed:\n  - Token: `IPFClient(auth=\'TOKEN\')`\n  - User/Pass: `IPFClient(auth=(\'USER\', \'PASS\'))`\n  - `.env` file will only accept `IPF_TOKEN` or (`IPF_USERNAME` and `IPF_PASSWORD`) and not `auth`\n\n## Versioning\n\nStarting with IP Fabric version 5.0.x the python-ipfabric and python-ipfabric-diagrams will need to\nmatch your IP Fabric version.  The API\'s are changing and instead of `api/v1` they will now be `api/v5.0`.\n\nVersion 5.1 will have backwards compatability with version 5.0 however 6.0 will not support any 5.x versions.\nBy ensuring that your ipfabric SDK\'s match your IP Fabric Major Version will ensure compatibility and will continue to work.\n\n## Installation\n\n```\npip install ipfabric\n```\n\n## Introduction\n\nPlease take a look at [API Programmability - Part 1: The Basics](https://ipfabric.io/blog/api-programmability-part-1/)\nfor instructions on creating an API token.\n\nMost of the methods and features can be located in [Examples](examples) to show how to use this package. \nAnother great introduction to this package can be found at [API Programmability - Part 2: Python](https://ipfabric.io/blog/api-programmability-python/)\n\n## Diagrams\n\nDiagramming in IP Fabric version v4.3 and above has been moved to it\'s own package.\n\nDiagramming will move back to this project in v7.0\n\n```\npip install ipfabric-diagrams\n```\n\n## Authentication\n### Username/Password\nSupply in client:\n```python\nfrom ipfabric import IPFClient\nipf = IPFClient(\'https://demo3.ipfabric.io/\', auth=(\'user\', \'pass\'))\n```\n\n### Token\n```python\nfrom ipfabric import IPFClient\nipf = IPFClient(\'https://demo3.ipfabric.io/\', auth=\'token\')\n```\n\n### Environment \nThe easiest way to use this package is with a `.env` file.  You can copy the sample and edit it with your environment variables. \n\n```commandline\ncp sample.env .env\n```\n\nThis contains the following variables which can also be set as environment variables instead of a .env file.\n```\nIPF_URL="https://demo3.ipfabric.io"\nIPF_TOKEN=TOKEN\nIPF_VERIFY=true\n```\n\nOr if using Username/Password:\n```\nIPF_URL="https://demo3.ipfabric.io"\nIPF_USERNAME=USER\nIPF_PASSWORD=PASS\n```\n\n## Development\n\n### Poetry Installation\n\nIPFabric uses [Poetry](https://pypi.org/project/poetry/) to make setting up a virtual environment with all dependencies\ninstalled quick and easy.\n\nInstall poetry globally:\n```\npip install poetry\n```\n\nTo install a virtual environment run the following command in the root of this directory.\n\n```\npoetry install\n```\n\nTo run examples, install extras:\n```\npoetry install ipfabric -E examples\n```\n\n### Test and Build\n\n```\npoetry run pytest\npoetry build\n```\n\nPrior to pushing changes run:\n```\npoetry run black ipfabric\npoetry update\n```\n',
     'author': 'Justin Jeffery',
     'author_email': 'justin.jeffery@ipfabric.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/ip-fabric/integrations/python-ipfabric',
```

### Comparing `ipfabric-6.2.4/PKG-INFO` & `ipfabric-6.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfabric
-Version: 6.2.4
+Version: 6.2.5
 Summary: Python package for interacting with IP Fabric
 Home-page: https://gitlab.com/ip-fabric/integrations/python-ipfabric
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Justin Jeffery
 Author-email: justin.jeffery@ipfabric.io
 Requires-Python: >=3.7.1,<4.0.0
```

