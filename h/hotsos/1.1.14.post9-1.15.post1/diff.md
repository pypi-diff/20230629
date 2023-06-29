# Comparing `tmp/hotsos-1.1.14.post9.tar.gz` & `tmp/hotsos-1.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotsos-1.1.14.post9.tar", last modified: Wed May 24 20:03:00 2023, max compression
+gzip compressed data, was "hotsos-1.15.post1.tar", last modified: Thu Jun 29 08:56:02 2023, max compression
```

## Comparing `hotsos-1.1.14.post9.tar` & `hotsos-1.15.post1.tar`

### file list

```diff
@@ -1,403 +1,409 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.891953 hotsos-1.1.14.post9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-24 20:03:00.891953 hotsos-1.1.14.post9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.855952 hotsos-1.1.14.post9/hotsos/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 20:02:47.000000 hotsos-1.1.14.post9/hotsos/.repo-info
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13956 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15453 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.859952 hotsos-1.1.14.post9/hotsos/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.859952 hotsos-1.1.14.post9/hotsos/core/host_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/host_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35158 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/host_helpers/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/host_helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/host_helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/host_helpers/filestat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/host_helpers/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/host_helpers/packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/host_helpers/pebble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/host_helpers/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/host_helpers/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/host_helpers/systemd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/host_helpers/uptime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.859952 hotsos-1.1.14.post9/hotsos/core/issues/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/issues/issue_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/issues/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.859952 hotsos-1.1.14.post9/hotsos/core/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.859952 hotsos-1.1.14.post9/hotsos/core/plugins/juju/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/juju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/juju/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/juju/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.863952 hotsos-1.1.14.post9/hotsos/core/plugins/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/kernel/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/kernel/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.863952 hotsos-1.1.14.post9/hotsos/core/plugins/kernel/kernlog/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/kernel/kernlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/kernel/kernlog/calltrace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/kernel/kernlog/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/kernel/kernlog/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/kernel/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    20317 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/kernel/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/kernel/sysfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/kubernetes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.863952 hotsos-1.1.14.post9/hotsos/core/plugins/lxd/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/lxd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/lxd/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/maas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.863952 hotsos-1.1.14.post9/hotsos/core/plugins/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/openstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/openstack/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    63860 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/openstack/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/openstack/neutron.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/openstack/nova.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/openstack/octavia.py
--rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/openstack/openstack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.863952 hotsos-1.1.14.post9/hotsos/core/plugins/openvswitch/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/openvswitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/openvswitch/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/openvswitch/ovn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/openvswitch/ovs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/pacemaker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.863952 hotsos-1.1.14.post9/hotsos/core/plugins/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/rabbitmq/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/rabbitmq/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/sosreport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.863952 hotsos-1.1.14.post9/hotsos/core/plugins/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/storage/bcache.py
--rw-r--r--   0 runner    (1001) docker     (123)    38249 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/storage/ceph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.863952 hotsos-1.1.14.post9/hotsos/core/plugins/system/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/system/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/system/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugins/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)    13784 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/plugintools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.863952 hotsos-1.1.14.post9/hotsos/core/ycheck/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.867952 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.867952 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    22878 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/conclusions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.867952 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.867952 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/apt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/pebble.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/snap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/systemd.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/varops.py
--rw-r--r--   0 runner    (1001) docker     (123)    15357 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/core/ycheck/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.851952 hotsos-1.1.14.post9/hotsos/defs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.851952 hotsos-1.1.14.post9/hotsos/defs/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.867952 hotsos-1.1.14.post9/hotsos/defs/events/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openstack/apache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openstack/apparmor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openstack/http-requests.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.867952 hotsos-1.1.14.post9/hotsos/defs/events/openstack/neutron/
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openstack/neutron/agents.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openstack/neutron/ml2-routers.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.867952 hotsos-1.1.14.post9/hotsos/defs/events/openstack/nova/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openstack/nova/external-events.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.867952 hotsos-1.1.14.post9/hotsos/defs/events/openstack/nova/migrations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.867952 hotsos-1.1.14.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/dst-pre-live-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/src-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/src-post-live-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openstack/nova/migrations/migrations.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openstack/nova/nova-compute.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openstack/octavia.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.851952 hotsos-1.1.14.post9/hotsos/defs/events/openvswitch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.871952 hotsos-1.1.14.post9/hotsos/defs/events/openvswitch/ovn/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.871952 hotsos-1.1.14.post9/hotsos/defs/events/openvswitch/ovs/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openvswitch/ovs/bfd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openvswitch/ovs/errors-and-warnings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.851952 hotsos-1.1.14.post9/hotsos/defs/events/storage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.851952 hotsos-1.1.14.post9/hotsos/defs/events/storage/ceph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.871952 hotsos-1.1.14.post9/hotsos/defs/events/storage/ceph/mon/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/storage/ceph/mon/mon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/storage/ceph/mon/monlogs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.871952 hotsos-1.1.14.post9/hotsos/defs/events/storage/ceph/osd/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/storage/ceph/osd/osd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.855952 hotsos-1.1.14.post9/hotsos/defs/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.871952 hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.871952 hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/bugs/lp1983140.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/bugs/lp1983506.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/charm_unit_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/juju.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/jujud_machine_checks.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.871952 hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/disk_failure.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/memory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.871952 hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/network/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/network/misc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/network/tcp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/network/udp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/qla2xxx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.871952 hotsos-1.1.14.post9/hotsos/defs/scenarios/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/kubernetes/kubernetes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.871952 hotsos-1.1.14.post9/hotsos/defs/scenarios/lxd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.871952 hotsos-1.1.14.post9/hotsos/defs/scenarios/lxd/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.875952 hotsos-1.1.14.post9/hotsos/defs/scenarios/mysql/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.875952 hotsos-1.1.14.post9/hotsos/defs/scenarios/mysql/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/mysql/bugs/lp372017.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/mysql/mysql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/mysql/mysql_connections.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.875952 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.851952 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/barbican/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.875952 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/barbican/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/eol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.851952 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/keystone/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.875952 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/keystone/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.875952 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/masakari/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.875952 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.875952 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1883089.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1928031.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1929832.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1965297.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.875952 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/nova/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.875952 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/nova/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1944619.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/nova/config_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.875952 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/octavia/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.875952 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/octavia/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/openstack.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/pkgs_from_mixed_releases_found.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.879952 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.879952 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/openvswitch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.879952 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.879952 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1917475.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.879952 hotsos-1.1.14.post9/hotsos/defs/scenarios/pacemaker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.879952 hotsos-1.1.14.post9/hotsos/defs/scenarios/pacemaker/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/pacemaker/pacemaker.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.879952 hotsos-1.1.14.post9/hotsos/defs/scenarios/rabbitmq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.879952 hotsos-1.1.14.post9/hotsos/defs/scenarios/rabbitmq/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/rabbitmq/rabbitmq.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.879952 hotsos-1.1.14.post9/hotsos/defs/scenarios/sosreport/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.879952 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.879952 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/bcache/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/bcache/bcache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/bcache/bdev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/bcache/cacheset.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.855952 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.879952 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mgr/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.883952 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.883952 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.883952 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph-osd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.887952 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-rgw/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.887952 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/storage.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.887952 hotsos-1.1.14.post9/hotsos/defs/scenarios/system/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/system/system.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/defs/scenarios/system/unattended_upgrades.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.887952 hotsos-1.1.14.post9/hotsos/plugin_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.887952 hotsos-1.1.14.post9/hotsos/plugin_extensions/juju/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/juju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/juju/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.887952 hotsos-1.1.14.post9/hotsos/plugin_extensions/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/kernel/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.887952 hotsos-1.1.14.post9/hotsos/plugin_extensions/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/kubernetes/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.887952 hotsos-1.1.14.post9/hotsos/plugin_extensions/lxd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/lxd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/lxd/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.887952 hotsos-1.1.14.post9/hotsos/plugin_extensions/maas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/maas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/maas/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.887952 hotsos-1.1.14.post9/hotsos/plugin_extensions/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/mysql/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.887952 hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.887952 hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/agent/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/agent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/nova_external_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/service_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/service_network_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/vm_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.887952 hotsos-1.1.14.post9/hotsos/plugin_extensions/openvswitch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/openvswitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/openvswitch/event_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/openvswitch/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.887952 hotsos-1.1.14.post9/hotsos/plugin_extensions/pacemaker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/pacemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/pacemaker/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.887952 hotsos-1.1.14.post9/hotsos/plugin_extensions/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/rabbitmq/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.887952 hotsos-1.1.14.post9/hotsos/plugin_extensions/sosreport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/sosreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/sosreport/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.891953 hotsos-1.1.14.post9/hotsos/plugin_extensions/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/storage/bcache_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/storage/ceph_event_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/storage/ceph_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.891953 hotsos-1.1.14.post9/hotsos/plugin_extensions/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/system/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/system/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.891953 hotsos-1.1.14.post9/hotsos/plugin_extensions/vault/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/plugin_extensions/vault/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.891953 hotsos-1.1.14.post9/hotsos/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/templates/content_dict.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/templates/content_list.html
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/hotsos/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:03:00.855952 hotsos-1.1.14.post9/hotsos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-24 20:03:00.000000 hotsos-1.1.14.post9/hotsos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-05-24 20:03:00.000000 hotsos-1.1.14.post9/hotsos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:03:00.000000 hotsos-1.1.14.post9/hotsos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 20:03:00.000000 hotsos-1.1.14.post9/hotsos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-24 20:03:00.000000 hotsos-1.1.14.post9/hotsos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 20:03:00.000000 hotsos-1.1.14.post9/hotsos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:03:00.891953 hotsos-1.1.14.post9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-24 20:02:41.000000 hotsos-1.1.14.post9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.221868 hotsos-1.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 08:55:40.000000 hotsos-1.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 08:55:40.000000 hotsos-1.15.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-29 08:56:02.217868 hotsos-1.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-29 08:55:40.000000 hotsos-1.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.181868 hotsos-1.15.post1/hotsos/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 08:55:45.000000 hotsos-1.15.post1/hotsos/.repo-info
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15070 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15451 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.181868 hotsos-1.15.post1/hotsos/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.185868 hotsos-1.15.post1/hotsos/core/host_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/host_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35418 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/host_helpers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/host_helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/host_helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/host_helpers/filestat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/host_helpers/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/host_helpers/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/host_helpers/pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/host_helpers/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/host_helpers/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/host_helpers/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/host_helpers/uptime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.185868 hotsos-1.15.post1/hotsos/core/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/issues/issue_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/issues/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.185868 hotsos-1.15.post1/hotsos/core/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.185868 hotsos-1.15.post1/hotsos/core/plugins/juju/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/juju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/juju/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/juju/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.185868 hotsos-1.15.post1/hotsos/core/plugins/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/kernel/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/kernel/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.185868 hotsos-1.15.post1/hotsos/core/plugins/kernel/kernlog/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/kernel/kernlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/kernel/kernlog/calltrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/kernel/kernlog/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/kernel/kernlog/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/kernel/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20359 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/kernel/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/kernel/sysfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/kubernetes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.185868 hotsos-1.15.post1/hotsos/core/plugins/lxd/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/lxd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/lxd/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/maas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.189868 hotsos-1.15.post1/hotsos/core/plugins/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/openstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/openstack/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63860 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/openstack/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/openstack/neutron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/openstack/nova.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/openstack/octavia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/openstack/openstack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.189868 hotsos-1.15.post1/hotsos/core/plugins/openvswitch/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/openvswitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/openvswitch/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/openvswitch/ovn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/openvswitch/ovs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/pacemaker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.189868 hotsos-1.15.post1/hotsos/core/plugins/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/rabbitmq/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/rabbitmq/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/sosreport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.189868 hotsos-1.15.post1/hotsos/core/plugins/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/storage/bcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/storage/ceph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.189868 hotsos-1.15.post1/hotsos/core/plugins/system/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/system/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/system/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugins/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/plugintools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.189868 hotsos-1.15.post1/hotsos/core/ycheck/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.189868 hotsos-1.15.post1/hotsos/core/ycheck/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.189868 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/conclusions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.193868 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.193868 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/apt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/snap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/varops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/core/ycheck/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.173868 hotsos-1.15.post1/hotsos/defs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.173868 hotsos-1.15.post1/hotsos/defs/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.193868 hotsos-1.15.post1/hotsos/defs/events/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openstack/apache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openstack/apparmor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openstack/http-requests.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.193868 hotsos-1.15.post1/hotsos/defs/events/openstack/neutron/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openstack/neutron/agents.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openstack/neutron/ml2-routers.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.193868 hotsos-1.15.post1/hotsos/defs/events/openstack/nova/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openstack/nova/external-events.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.193868 hotsos-1.15.post1/hotsos/defs/events/openstack/nova/migrations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.193868 hotsos-1.15.post1/hotsos/defs/events/openstack/nova/migrations/live-migration/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openstack/nova/migrations/live-migration/dst-pre-live-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openstack/nova/migrations/live-migration/src-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openstack/nova/migrations/live-migration/src-post-live-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openstack/nova/migrations/migrations.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openstack/nova/nova-compute.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openstack/octavia.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.173868 hotsos-1.15.post1/hotsos/defs/events/openvswitch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.193868 hotsos-1.15.post1/hotsos/defs/events/openvswitch/ovn/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.193868 hotsos-1.15.post1/hotsos/defs/events/openvswitch/ovs/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openvswitch/ovs/bfd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openvswitch/ovs/errors-and-warnings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.173868 hotsos-1.15.post1/hotsos/defs/events/storage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.173868 hotsos-1.15.post1/hotsos/defs/events/storage/ceph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.193868 hotsos-1.15.post1/hotsos/defs/events/storage/ceph/mon/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/storage/ceph/mon/mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/storage/ceph/mon/monlogs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.197868 hotsos-1.15.post1/hotsos/defs/events/storage/ceph/osd/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/storage/ceph/osd/osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.177868 hotsos-1.15.post1/hotsos/defs/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.197868 hotsos-1.15.post1/hotsos/defs/scenarios/juju/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.197868 hotsos-1.15.post1/hotsos/defs/scenarios/juju/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/juju/bugs/lp1983140.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/juju/bugs/lp1983506.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/juju/charm_unit_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/juju/juju.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/juju/jujud_machine_checks.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.197868 hotsos-1.15.post1/hotsos/defs/scenarios/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/kernel/disk_failure.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/kernel/memory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.197868 hotsos-1.15.post1/hotsos/defs/scenarios/kernel/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/kernel/network/misc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/kernel/network/tcp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/kernel/network/udp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/kernel/qla2xxx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.197868 hotsos-1.15.post1/hotsos/defs/scenarios/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/kubernetes/kubernetes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.197868 hotsos-1.15.post1/hotsos/defs/scenarios/lxd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.197868 hotsos-1.15.post1/hotsos/defs/scenarios/lxd/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.197868 hotsos-1.15.post1/hotsos/defs/scenarios/mysql/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.197868 hotsos-1.15.post1/hotsos/defs/scenarios/mysql/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/mysql/bugs/lp372017.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/mysql/mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/mysql/mysql_connections.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.201868 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.173868 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/barbican/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.201868 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/barbican/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/eol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.173868 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/keystone/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.201868 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/keystone/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.201868 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/masakari/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.201868 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.201868 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1883089.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1928031.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1929832.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1965297.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.201868 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/nova/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.205868 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/nova/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1944619.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/nova/config_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.205868 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/octavia/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.205868 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/octavia/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/openstack.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/pkgs_from_mixed_releases_found.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.205868 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.205868 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/openvswitch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.205868 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.205868 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1917475.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/service_restarts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.205868 hotsos-1.15.post1/hotsos/defs/scenarios/pacemaker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.205868 hotsos-1.15.post1/hotsos/defs/scenarios/pacemaker/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/pacemaker/pacemaker.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.205868 hotsos-1.15.post1/hotsos/defs/scenarios/rabbitmq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.205868 hotsos-1.15.post1/hotsos/defs/scenarios/rabbitmq/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/rabbitmq/rabbitmq.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.205868 hotsos-1.15.post1/hotsos/defs/scenarios/sosreport/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.205868 hotsos-1.15.post1/hotsos/defs/scenarios/storage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.209868 hotsos-1.15.post1/hotsos/defs/scenarios/storage/bcache/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/bcache/bcache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/bcache/bdev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/bcache/cacheset.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.177868 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.209868 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mgr/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.209868 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.213868 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.213868 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph-osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.213868 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-rgw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.213868 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/storage/storage.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.213868 hotsos-1.15.post1/hotsos/defs/scenarios/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/system/system.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/defs/scenarios/system/unattended_upgrades.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.213868 hotsos-1.15.post1/hotsos/plugin_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.213868 hotsos-1.15.post1/hotsos/plugin_extensions/juju/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/juju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/juju/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.213868 hotsos-1.15.post1/hotsos/plugin_extensions/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/kernel/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.213868 hotsos-1.15.post1/hotsos/plugin_extensions/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/kubernetes/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.213868 hotsos-1.15.post1/hotsos/plugin_extensions/lxd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/lxd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/lxd/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.213868 hotsos-1.15.post1/hotsos/plugin_extensions/maas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/maas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/maas/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.213868 hotsos-1.15.post1/hotsos/plugin_extensions/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/mysql/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.217868 hotsos-1.15.post1/hotsos/plugin_extensions/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/openstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.217868 hotsos-1.15.post1/hotsos/plugin_extensions/openstack/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/openstack/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/openstack/agent/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/openstack/agent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/openstack/nova_external_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/openstack/service_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/openstack/service_network_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/openstack/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/openstack/vm_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.217868 hotsos-1.15.post1/hotsos/plugin_extensions/openvswitch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/openvswitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/openvswitch/event_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/openvswitch/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.217868 hotsos-1.15.post1/hotsos/plugin_extensions/pacemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/pacemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/pacemaker/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.217868 hotsos-1.15.post1/hotsos/plugin_extensions/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/rabbitmq/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.217868 hotsos-1.15.post1/hotsos/plugin_extensions/sosreport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/sosreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/sosreport/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.217868 hotsos-1.15.post1/hotsos/plugin_extensions/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/storage/bcache_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/storage/ceph_event_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/storage/ceph_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.217868 hotsos-1.15.post1/hotsos/plugin_extensions/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/system/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/system/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.217868 hotsos-1.15.post1/hotsos/plugin_extensions/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/plugin_extensions/vault/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.217868 hotsos-1.15.post1/hotsos/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/templates/content_dict.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/templates/content_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-29 08:55:40.000000 hotsos-1.15.post1/hotsos/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:02.181868 hotsos-1.15.post1/hotsos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-29 08:56:02.000000 hotsos-1.15.post1/hotsos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-06-29 08:56:02.000000 hotsos-1.15.post1/hotsos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:56:02.000000 hotsos-1.15.post1/hotsos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 08:56:02.000000 hotsos-1.15.post1/hotsos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-29 08:56:02.000000 hotsos-1.15.post1/hotsos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 08:56:02.000000 hotsos-1.15.post1/hotsos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-29 08:55:40.000000 hotsos-1.15.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:56:02.221868 hotsos-1.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-29 08:55:40.000000 hotsos-1.15.post1/setup.py
```

### Comparing `hotsos-1.1.14.post9/LICENSE` & `hotsos-1.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/cli.py` & `hotsos-1.15.post1/hotsos/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 #!/usr/bin/env python3
-import click
 import contextlib
+from importlib import metadata, resources
 import os
 import sys
 import subprocess
 import threading
 
-from importlib import metadata, resources
-from progress.spinner import Spinner
-
+import click
+import distro
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.log import setup_logging, log
 from hotsos.core.host_helpers import CLIHelper
 from hotsos.client import (
     HotSOSClient,
     OutputManager,
     PLUGIN_CATALOG,
 )
+from progress.spinner import Spinner
+
+
+def is_snap():
+    return os.environ.get('SNAP_NAME', '') == 'hotsos'
+
+
+def get_os_id():
+    return distro.id()
+
+
+def get_os_version():
+    return float(distro.version())
 
 
 def get_hotsos_root():
     return os.path.dirname(sys.argv[0])
 
 
 def get_version():
@@ -296,14 +308,26 @@
         HotSOSConfig.command_timeout = command_timeout
 
         if version:
             print(_version)
             return
 
         data_root = fix_data_root(data_root)
+
+        if is_snap() and data_root == '/':
+            print("ERROR: hotsos is installed as a snap which only "
+                  "supports running against a sosreport due to access "
+                  "restrictions.\n\n"
+                  "If you want to analyse a host you need to "
+                  "use an alternative installation method e.g. debian "
+                  "package - see "
+                  "https://hotsos.readthedocs.io/en/latest/install/index.html"
+                  " for more information.")
+            sys.exit(1)
+
         if agent_error_key_by_time:
             print("WARNING: option --agent-error-key-by-time is DEPRECATED "
                   "and longer has any effect. Use --event-tally-granularity "
                   "instead.")
 
         HotSOSConfig.set(use_all_logs=all_logs, plugin_yaml_defs=defs_path,
                          templates_path=templates_path, data_root=data_root,
@@ -364,9 +388,20 @@
                               minimal_mode=minimal_mode)
             if out:
                 sys.stdout.write("{}\n".format(out))
 
     cli(prog_name='hotsos')
 
 
+def exit_if_os_version_not_supported_in_snap():
+    if is_snap():
+        if get_os_id() != 'ubuntu':
+            print("This snap has only been verified to run on Ubuntu")
+            sys.exit(1)
+        if get_os_version() < 20.04:
+            print("This snap has only been verified to run on Focal and above")
+            sys.exit(2)
+
+
 if __name__ == '__main__':
+    exit_if_os_version_not_supported_in_snap()
     main()
```

### Comparing `hotsos-1.1.14.post9/hotsos/client.py` & `hotsos-1.15.post1/hotsos/client.py`

 * *Files identical despite different names*

```diff
@@ -7,30 +7,28 @@
 import tempfile
 
 from hotsos.core.log import log
 from hotsos.core.issues import IssuesManager
 from hotsos.core.host_helpers.cli import CLIHelper
 from hotsos.core.config import HotSOSConfig
 from hotsos.core import plugintools
-
 from hotsos.plugin_extensions.lxd.summary import LXDSummary
 from hotsos.plugin_extensions.mysql.summary import MySQLSummary
 from hotsos.plugin_extensions.juju.summary import JujuSummary
 from hotsos.plugin_extensions.openstack import (
     summary as ost_summary,
     service_features,
     service_network_checks,
     vm_info,
     nova_external_events,
 )
 from hotsos.plugin_extensions.openstack.agent import (
     events as agent_events,
     exceptions as agent_exceptions,
 )
-
 from hotsos.plugin_extensions.openvswitch import (
     summary as ovs_summary,
     event_checks,
 )
 from hotsos.plugin_extensions.system.summary import SystemSummary
 from hotsos.plugin_extensions.system.checks import SYSCtlChecks
 from hotsos.plugin_extensions.maas.summary import MAASSummary
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/analytics.py` & `hotsos-1.15.post1/hotsos/core/analytics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import statistics
-
 from datetime import datetime
+import statistics
 
 
 class EventCollection(object):
     """Used to collect events found in logfiles. Events are defined as having
     identifiable start and end points containing timestamp information such
     that we can calculate their duration.
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/config.py` & `hotsos-1.15.post1/hotsos/core/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import abc
-import copy
-
 from collections import UserDict
+import copy
 
 
 class ConfigException(Exception):
     pass
 
 
 class ConfigOpt(object):
@@ -17,15 +16,16 @@
 
 
 class ConfigOptGroupBase(UserDict):
 
     def __init__(self):
         self.opts = []
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def name(self):
         """ OptGroup name """
 
     @property
     def data(self):
         d = {}
         for opt in self.opts:
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/factory.py` & `hotsos-1.15.post1/hotsos/core/factory.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/host_helpers/__init__.py` & `hotsos-1.15.post1/hotsos/core/host_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/host_helpers/cli.py` & `hotsos-1.15.post1/hotsos/core/host_helpers/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,29 +107,29 @@
         self.reset()
         return out
 
     return reset_command_inner
 
 
 class CmdBase(object):
+    """ Base class for all command source types. """
 
     def __init__(self):
         self.hooks = {}
         self.reset()
 
     def reset(self):
         """
         Used to reset an object after it has been called. In other words, each
         time a command object is called it may alter its initial state e.g. via
         hooks but this state should not persist to the next call so this is
         used to restore state.
         """
         raise NotImplementedError
 
-    """ Base class for all command source types. """
     @classmethod
     def safe_readlines(cls, path):
         return open(path, 'r', errors="surrogateescape").readlines()
 
     def register_hook(self, name, f):
         """
         Implementations of this class can register hooks to
@@ -738,14 +738,17 @@
                 [DateBinCmd('date', singleline=True),
                  DateFileCmd('sos_commands/date/date', singleline=True),
                  # this is for legacy sosreport versions
                  DateFileCmd('sos_commands/general/date', singleline=True)],
             'df':
                 [BinCmd('df'),
                  FileCmd('df')],
+            'dmesg':
+                [BinCmd('dmesg'),
+                 FileCmd('sos_commands/kernel/dmesg')],
             'docker_images':
                 [BinCmd('docker images'),
                  FileCmd('sos_commands/docker/docker_images')],
             'docker_ps':
                 [BinCmd('docker ps'),
                  FileCmd('sos_commands/docker/docker_ps')],
             'dpkg_l':
@@ -786,15 +789,17 @@
                  FileCmd('sos_commands/lxd/lxd.buginfo')],
             'numactl':
                 [BinCmd('numactl --hardware'),
                  FileCmd('sos_commands/numa/numactl_--hardware')],
             'ns_ip_addr':
                 [BinCmd('ip netns exec {namespace} ip address show'),
                  FileCmd('sos_commands/networking/'
-                         'ip_netns_exec_{namespace}_ip_address_show')],
+                         'ip_netns_exec_{namespace}_ip_address_show'),
+                 FileCmd('sos_commands/networking/namespaces/{namespace}/'
+                         'ip_netns_exec_{namespace}_ip_-d_address_show')],
             'ovn_nbctl_show':
                 [BinCmd('ovn-nbctl show'),
                  FileCmd('sos_commands/ovn_central/ovn-nbctl_show')],
             'ovn_sbctl_show':
                 [BinCmd('ovn-sbctl show'),
                  FileCmd('sos_commands/ovn_central/ovn-sbctl_show')],
             'ovs_vsctl_get_Open_vSwitch':
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/host_helpers/common.py` & `hotsos-1.15.post1/hotsos/core/host_helpers/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import abc
 import re
 
-from searchkit.utils import MPCache
-
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.log import log
+from searchkit.utils import MPCache
 
 
 class HostHelpersBase(abc.ABC):
 
     def __init__(self, *args, **kwargs):
         self.cache = MPCache(self.cache_name,
                              'host_helpers_{}'.format(self.cache_type),
@@ -19,19 +18,21 @@
     def cache_root(self):
         """
         By default caches are global to all plugins but this can be overridden
         if we want otherwise.
         """
         return HotSOSConfig.global_tmp_dir
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def cache_name(self):
         """ Unique name for cache used by instance of this object. """
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def cache_type(self):
         """
         Unique name for the type of cache used by instance of this object.
         """
 
     @abc.abstractmethod
     def cache_load(self):
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/host_helpers/config.py` & `hotsos-1.15.post1/hotsos/core/host_helpers/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/host_helpers/filestat.py` & `hotsos-1.15.post1/hotsos/core/host_helpers/filestat.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/host_helpers/network.py` & `hotsos-1.15.post1/hotsos/core/host_helpers/network.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/host_helpers/packaging.py` & `hotsos-1.15.post1/hotsos/core/host_helpers/packaging.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,20 +340,20 @@
     def get_revision(self, snap):
         """ Return revision of package.
         """
         info = self._get_snap_info(snap)
         if info:
             return info[0]['revision']
 
-    def get_version(self, snap):
-        """ Return version of package.
+    def get_version(self, pkg):
+        """ Return version of snap package.
 
         Assumes only one snap will be matched.
         """
-        info = self._get_snap_info(snap)
+        info = self._get_snap_info(pkg)
         if info:
             return info[0]['version']
 
     def _get_snap_info(self, snap_name_expr):
         """
         Return a list of info for snaps matched using the expression.
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/host_helpers/pebble.py` & `hotsos-1.15.post1/hotsos/core/host_helpers/pebble.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,32 +37,30 @@
         return _services
 
     @cached_property
     def processes(self):  # pylint: disable=W0236
         """
         Identify running processes from ps that are associated with resolved
         pebble services.  The search pattern used to identify a service is also
-        used to match the process binary name.
+        used to match the process binary/cmd name.
+
+        Accounts for different types of process cmd path e.g.
+
+        /snap/<name>/1830/<svc>
+        /usr/bin/<svc>
+
+        and filter e.g.
+
+        /var/lib/<svc> and /var/log/<svc>
 
         Returns a dictionary of process names along with the number of each.
         """
         _proc_info = {}
         for line in CLIHelper().ps():
             for expr in self._service_exprs:
-                """
-                look for running process with this name.
-                We need to account for different types of process binary e.g.
-
-                /snap/<name>/1830/<svc>
-                /usr/bin/<svc>
-
-                and filter e.g.
-
-                /var/lib/<svc> and /var/log/<svc>
-                """
                 cmd = self.get_cmd_from_ps_line(line, expr)
                 if cmd:
                     if cmd in _proc_info:
                         _proc_info[cmd] += 1
                     else:
                         _proc_info[cmd] = 1
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/host_helpers/ssl.py` & `hotsos-1.15.post1/hotsos/core/host_helpers/ssl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import os
-
 from datetime import datetime
+import os
 
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
-
 from hotsos.core.host_helpers.cli import CLIHelper
 from hotsos.core.log import log
 from hotsos.core.factory import FactoryBase
 from hotsos.core.config import HotSOSConfig
 
 
 class SSLCertificate(object):
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/host_helpers/sysctl.py` & `hotsos-1.15.post1/hotsos/core/host_helpers/sysctl.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/host_helpers/systemd.py` & `hotsos-1.15.post1/hotsos/core/host_helpers/systemd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from datetime import datetime
-import os
 import glob
-
+import os
 import re
 
 from hotsos.core.log import log
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.factory import FactoryBase
 from hotsos.core.host_helpers import CLIHelper
 from hotsos.core.host_helpers.common import ServiceManagerBase
@@ -49,14 +48,35 @@
         """
         t = self.start_time
         if t is None:
             return 0
 
         return t.timestamp()
 
+    @property
+    def memory_current(self):
+        """ Returns service current memory usage in bytes. """
+        path = os.path.join(HotSOSConfig.data_root,
+                            'sys/fs/cgroup/memory/system.slice',
+                            "{}.service".format(self.name),
+                            'memory.usage_in_bytes')
+        if not os.path.exists(path):
+            # path changed between Ubuntu Focal and Jammy releases.
+            path = os.path.join(HotSOSConfig.data_root,
+                                'sys/fs/cgroup/system.slice',
+                                "{}.service".format(self.name),
+                                'memory.current')
+
+        if not os.path.exists(path):
+            log.warning("service memory info not found at %s", path)
+            return 0
+
+        with open(path) as fd:
+            return int(fd.read())
+
     def __repr__(self):
         return ("name={}, state={}, start_time={}, has_instances={}".
                 format(self.name, self.state, self.start_time,
                        self.has_instances))
 
 
 class SystemdHelper(ServiceManagerBase):
@@ -231,32 +251,30 @@
         return ps_filtered
 
     @cached_property
     def processes(self):  # pylint: disable=W0236
         """
         Identify running processes from ps that are associated with resolved
         systemd services. The search pattern used to identify a service is also
-        used to match the process binary name.
+        used to match the process binaryc/cmd name.
+
+        Accounts for different types of process cmd path e.g.
+
+        /snap/<name>/1830/<svc>
+        /usr/bin/<svc>
+
+        and filter e.g.
+
+        /var/lib/<svc> and /var/log/<svc>
 
         Returns a dictionary of process names along with the number of each.
         """
         _proc_info = {}
         for line in self._service_filtered_ps:
             for expr in self._service_exprs:
-                """
-                look for running process with this name.
-                We need to account for different types of process binary e.g.
-
-                /snap/<name>/1830/<svc>
-                /usr/bin/<svc>
-
-                and filter e.g.
-
-                /var/lib/<svc> and /var/log/<svc>
-                """
                 cmd = self.get_cmd_from_ps_line(line, expr)
                 if not cmd:
                     continue
 
                 if cmd in _proc_info:
                     _proc_info[cmd] += 1
                 else:
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/host_helpers/uptime.py` & `hotsos-1.15.post1/hotsos/core/host_helpers/uptime.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/issues/issue_types.py` & `hotsos-1.15.post1/hotsos/core/issues/issue_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,21 @@
 class BugTypeBase(abc.ABC, IssueTypeBase):
     ISSUE_TYPE = 'bug'
 
     def __init__(self, id, msg):
         self.id = id
         self.msg = msg
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def base_url(self):
         pass
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def url(self):
         pass
 
 
 class HotSOSScenariosWarning(IssueTypeBase):
     pass
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/issues/utils.py` & `hotsos-1.15.post1/hotsos/core/issues/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 import os
-import yaml
 
-from hotsos.core.log import log
 from hotsos.core.config import HotSOSConfig
+from hotsos.core.log import log
 from hotsos.core.utils import sorted_dict
+import yaml
 
 
 class IssueContext(object):
     def __init__(self, **kwargs):
         self.context = {}
         self.set(**kwargs)
 
@@ -27,15 +27,16 @@
         self.key = key
         self.context = context
         self.ref = ref
         self.description = description
         self.origin = "{}.{}".format(HotSOSConfig.plugin_name,
                                      HotSOSConfig.part_name)
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def content(self):
         """ The is the final representation of the object. """
 
 
 class IssueEntry(IssueEntryBase):
 
     @property
@@ -53,15 +54,16 @@
 class IssuesStoreBase(abc.ABC):
 
     def __init__(self):
         if not os.path.isdir(HotSOSConfig.plugin_tmp_dir):
             raise Exception("plugin tmp dir  '{}' not found".
                             format(HotSOSConfig.plugin_tmp_dir))
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def store_path(self):
         pass
 
     @abc.abstractmethod
     def load(self):
         pass
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/log.py` & `hotsos-1.15.post1/hotsos/core/log.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/juju/common.py` & `hotsos-1.15.post1/hotsos/core/plugins/juju/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 
-from searchkit.constraints import TimestampMatcherBase
-
 from hotsos.core import plugintools
 from hotsos.core.host_helpers import PebbleHelper, SystemdHelper
 from hotsos.core.plugins.juju.resources import JujuBase
+from searchkit.constraints import TimestampMatcherBase
 
 SVC_VALID_SUFFIX = r'[0-9a-zA-Z-_]*'
 JUJU_SVC_EXPRS = [r'mongod{}'.format(SVC_VALID_SUFFIX),
                   r'jujud{}'.format(SVC_VALID_SUFFIX),
                   # catch juju-db but filter out processes with juju-db in
                   # their args list.
                   r'(?:^|[^\s])juju-db{}'.format(SVC_VALID_SUFFIX)]
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/juju/resources.py` & `hotsos-1.15.post1/hotsos/core/plugins/juju/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import os
-
 import glob
+import os
 import re
-import yaml
 
 from hotsos.core.log import log
 from hotsos.core import utils
 from hotsos.core.config import HotSOSConfig
+import yaml
 
 
 class JujuMachine(object):
 
     def __init__(self, juju_lib_path):
         self.juju_lib_path = juju_lib_path
         self.cfg = {}
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/kernel/common.py` & `hotsos-1.15.post1/hotsos/core/plugins/kernel/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/kernel/config.py` & `hotsos-1.15.post1/hotsos/core/plugins/kernel/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/kernel/kernlog/calltrace.py` & `hotsos-1.15.post1/hotsos/core/plugins/kernel/kernlog/calltrace.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,22 +98,22 @@
 
         # Very basic, just a simple expression to identify that a call trace
         # has occurred.
         expr = r'.+Call Trace:'
         self._search_def = SearchDef(expr, tag=self.name)
         return self._search_def
 
-    def apply(self, result):
+    def apply(self, results):
         """
         Run through the results.
 
         @param results: list of search.SearchResult objects.
         """
-        log.debug("%s has %s results", self.__class__.__name__, len(result))
-        for _trace in result:
+        log.debug("%s has %s results", self.__class__.__name__, len(results))
+        for _trace in results:
             # just a save a value i.e. to make the list length represent the
             # number of call traces.
             self.generics.append(True)
 
     @property
     def heuristics(self):
         """
@@ -137,19 +137,21 @@
 
     def extract(self, part, line):
         for field in self.fields:
             ret = re.search('{}:{}'.format(field, self.expr), line)
             if ret:
                 part.add(field, ret.group(1))
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def expr(self):
         """ Search pattern template used to match a field and its value. """
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def fields(self):
         """ List of fields we want extract from a given section. """
 
 
 class MemFieldsMain(MemFieldsBase):
 
     @property
@@ -229,21 +231,21 @@
                          r' bch_journal_meta(\S+) bch_btree_set_root(\S+)'
                          r' bch_journal_replay(\S+) register_bcache(\S+)')
         end = SearchDef(r'{}.+\s+do_syscall_(\S+)'.format(KERNLOG_PREFIX))
         self._search_def = SequenceSearchDef(start, tag='bcache', body=body,
                                              end=end)
         return self._search_def
 
-    def apply(self, result):
+    def apply(self, results):
         """
         Run through the results.
         @param results: list of search.SearchResult objects.
         """
-        log.debug("%s has %s results", self.__class__.__name__, len(result))
-        if len(result) > 0:
+        log.debug("%s has %s results", self.__class__.__name__, len(results))
+        if len(results) > 0:
             # we have found at least one deadlock
             self.deadlocks.append(True)
 
     @property
     def heuristics(self):
         """
         Register any heuristics we want to run here.
@@ -277,21 +279,21 @@
         body = SearchDef(r'(\S+) schedule(\S+) fanotify_handle_event(\S+)'
                          r' fsnotify(\S+)')
         end = SearchDef(r'.+\s+do_sys_open(\S+)')
         self._search_def = SequenceSearchDef(start, tag='fanotify', body=body,
                                              end=end)
         return self._search_def
 
-    def apply(self, result):
+    def apply(self, results):
         """
         Run through the results.
         @param results: list of search.SearchResult objects.
         """
-        log.debug("%s has %s results", self.__class__.__name__, len(result))
-        if len(result) > 0:
+        log.debug("%s has %s results", self.__class__.__name__, len(results))
+        if len(results) > 0:
             # we have found at least one fanotify related hang
             self.fanotify_hangs.append(True)
 
     @property
     def heuristics(self):
         """
         Register any heuristics we want to run here.
@@ -330,17 +332,17 @@
         end = SearchDef(r'{} '
                         r'(?:Out of memory: |Memory cgroup out of memory: )?'
                         r'Killed process (\d+) .+'.format(KERNLOG_PREFIX))
         self._search_def = SequenceSearchDef(start, tag='oom', body=body,
                                              end=end)
         return self._search_def
 
-    def apply(self, result):
-        log.debug("%s has %s results", self.__class__.__name__, len(result))
-        for trace in result.values():
+    def apply(self, results):
+        log.debug("%s has %s results", self.__class__.__name__, len(results))
+        for trace in results.values():
             oom_kill = OOMCallTraceState()
             oom_kill.add('nodes', {})
             current_node = None
             for item in trace:
                 if item.tag.endswith('-start'):
                     oom_kill.add('procname', item.get(1))
                     oom_kill.add('order', item.get(2))
@@ -420,21 +422,21 @@
         start = SearchDef(r'.+ blocked for more than (\d+) seconds.')
         body = SearchDef('.+')
         end = SearchDef(r'.+\s+do_syscall_(\S+)')
         self._search_def = SequenceSearchDef(start, tag='hungtask', body=body,
                                              end=end)
         return self._search_def
 
-    def apply(self, result):
+    def apply(self, results):
         """
         Run through the results.
         @param results: list of searchtools.SearchResult objects.
         """
-        log.debug("%s has %s results", self.__class__.__name__, len(result))
-        if len(result) > 0:
+        log.debug("%s has %s results", self.__class__.__name__, len(results))
+        if len(results) > 0:
             # we have found at least one blocked task
             self.hungtasks.append(True)
 
     @property
     def heuristics(self):
         """
         Register any heuristics we want to run here.
@@ -462,20 +464,20 @@
     def run(self):
         for tracetype in self.tracetypes:
             self.searcher.add(tracetype.searchdef, self.path)
 
         self.results = self.searcher.run()
         for tracetype in self.tracetypes:
             if type(tracetype.searchdef) == SequenceSearchDef:
-                result = self.results.find_sequence_sections(
+                results = self.results.find_sequence_sections(
                                                            tracetype.searchdef)
             else:
-                result = self.results.find_by_tag(tracetype.searchdef.tag)
+                results = self.results.find_by_tag(tracetype.searchdef.tag)
 
-            tracetype.apply(result)
+            tracetype.apply(results)
 
     def __getattr__(self, name):
         """
         If one or more trace has been identified with the given type name,
         return its object.
         """
         for h in self.tracetypes:
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/kernel/kernlog/common.py` & `hotsos-1.15.post1/hotsos/core/plugins/kernel/kernlog/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import abc
 import os
 
-from searchkit.constraints import TimestampMatcherBase
-
 from hotsos.core.log import log
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.host_helpers import CLIHelper, HostNetworkingHelper
 from hotsos.core.search import FileSearcher, SearchConstraintSearchSince
+from searchkit.constraints import TimestampMatcherBase
 
 KERNLOG_TS = r'\[\s*\d+\.\d+\]'
 KERNLOG_PREFIX = (r'(?:\S+\s+\d+\s+[\d:]+\s+\S+\s+\S+:\s+)?{}'.
                   format(KERNLOG_TS))
 
 
 class KernLogTimestampMatcher(TimestampMatcherBase):
@@ -73,21 +72,23 @@
 class TraceTypeBase(abc.ABC):
     """
     This defines a common interface to trace types and should be implemented
     for any trace types we want to capture. Implementations of this object
     are typically registered with a CallTraceManager for processing.
     """
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def name(self):
         """
         Name used to identify the type of call trace e.g. "oomkiller".
         """
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def searchdef(self):
         """
         A search definition object (simple or sequence) used to identify this
         call trace.
         """
 
     @abc.abstractmethod
@@ -95,15 +96,16 @@
         """
         Take results and parse into constituent parts.
 
         @param results: a SearchResultsCollection object containing the results
         of our search.
         """
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def heuristics(self):
         """ Return a list of CallTraceHeuristic objects that can be used to
         run checks on any identified call traces. """
 
     @abc.abstractmethod
     def __len__(self):
         """ Return number of call stacks identified.  """
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/kernel/kernlog/events.py` & `hotsos-1.15.post1/hotsos/core/plugins/kernel/kernlog/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/kernel/memory.py` & `hotsos-1.15.post1/hotsos/core/plugins/kernel/memory.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/kernel/net.py` & `hotsos-1.15.post1/hotsos/core/plugins/kernel/net.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import abc
-import os
-
 from collections import OrderedDict, UserList
+import os
 
 from hotsos.core.log import log
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.host_helpers import SYSCtlFactory, CLIHelper
 from hotsos.core.search import FileSearcher, SearchDef, ResultFieldInfo
 from hotsos.core.utils import mktemp_dump
-from abc import abstractmethod, abstractproperty
 
 
 class ProcNetBase(abc.ABC):
     """
     Provides a common way to extract fields from /proc/net/snmp and netstat.
 
     Expected file format is:
@@ -80,20 +78,22 @@
     def _get_field(self, header, field):
         """Return counter value for field in section header, or
         zero if field does not exist (because older kernel versions
         do not have some fields).
         """
         return self._data.get(header, {}).get(field, 0)
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def _header(self):
         """
         """
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def _fields(self):
         """
         """
 
     def __getattr__(self, fld):
         if fld in self._fields:
             return self._get_field(self._header, fld)
@@ -403,34 +403,38 @@
 
 class STOVParserBase(UserList):
 
     def __init__(self):
         self.data = []
         self._load()
 
-    @abstractmethod
+    @abc.abstractmethod
     def _load(self):
         """ Load data from source. """
 
-    @abstractproperty
+    @property
+    @abc.abstractmethod
     def _search_field_info(self):
         """
         Returns a ResultFieldInfo object to make columns addressable by their
         name as well as mapping them to a specific type.
         """
 
-    @abstractproperty
+    @property
+    @abc.abstractmethod
     def _header_matcher(self):
         """ python.re regular expression to match each header. """
 
-    @abstractproperty
+    @property
+    @abc.abstractmethod
     def _field_matcher(self):
         """ python.re regular expression to match each row. """
 
-    @abstractproperty
+    @property
+    @abc.abstractmethod
     def fields(self):
         """
         This is a dictionary of fields exposed by this object along with their
         type. This provides an opportunity to split/translate fields into sub
         fields but can also mirror _search_field_info.
         """
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/kernel/sysfs.py` & `hotsos-1.15.post1/hotsos/core/plugins/kernel/sysfs.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/kubernetes.py` & `hotsos-1.15.post1/hotsos/core/plugins/kubernetes.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/lxd/common.py` & `hotsos-1.15.post1/hotsos/core/plugins/lxd/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/maas.py` & `hotsos-1.15.post1/hotsos/core/plugins/maas.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/mysql.py` & `hotsos-1.15.post1/hotsos/core/plugins/mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import glob
+
 from hotsos.core.host_helpers import (
     APTPackageHelper,
     PebbleHelper,
     SystemdHelper,
 )
 from hotsos.core import (
     host_helpers,
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/openstack/common.py` & `hotsos-1.15.post1/hotsos/core/plugins/openstack/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/openstack/exceptions.py` & `hotsos-1.15.post1/hotsos/core/plugins/openstack/exceptions.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/openstack/neutron.py` & `hotsos-1.15.post1/hotsos/core/plugins/openstack/neutron.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/openstack/nova.py` & `hotsos-1.15.post1/hotsos/core/plugins/storage/bcache.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,216 +1,215 @@
+import glob
 import os
 import re
 
 from hotsos.core.config import HotSOSConfig
-from hotsos.core.plugins.openstack.openstack import (
-    OSTServiceBase,
-    OpenstackConfig,
-)
 from hotsos.core.host_helpers import CLIHelper
-from hotsos.core.plugins.kernel.config import (
-    KernelConfig,
-    SystemdConfig,
-)
-from hotsos.core.plugins.system.system import (
-    NUMAInfo,
-    SystemBase,
+from hotsos.core.host_helpers.config import ConfigBase
+from hotsos.core.plugins.storage import StorageBase
+from hotsos.core.search import (
+    FileSearcher,
+    SequenceSearchDef,
+    SearchDef
 )
-from hotsos.core.utils import cached_property
+from hotsos.core.utils import cached_property, mktemp_dump
 
 
-class NovaBase(OSTServiceBase):
+class BcacheConfig(ConfigBase):
 
-    def __init__(self, *args, **kwargs):
-        super().__init__('nova', *args, **kwargs)
-        self.nova_config = self.project.config['main']
+    def get(self, key):
+        cfg = os.path.join(self.path, key)
+        if os.path.exists(cfg):
+            with open(cfg) as fd:
+                return fd.read().strip()
 
-    @cached_property
-    def instances(self):
-        instances = {}
-        for line in CLIHelper().ps():
-            ret = re.compile('.+product=OpenStack Nova.+').match(line)
-            if ret:
-                name = None
-                uuid = None
 
-                expr = r'.+uuid\s+([a-z0-9\-]+)[\s,]+.+'
-                ret = re.compile(expr).match(ret[0])
-                if ret:
-                    uuid = ret[1]
+class BDev(object):
 
-                expr = r'.+\s+-name\s+guest=(instance-\w+)[,]*.*\s+.+'
-                ret = re.compile(expr).match(ret[0])
-                if ret:
-                    name = ret[1]
+    def __init__(self, path, cache):
+        self.cache = cache
+        self.path = path
 
-                if not all([name, uuid]):
-                    continue
+    @property
+    def cfg(self):
+        return BcacheConfig(self.path)
 
-                guest = NovaInstance(uuid, name)
-                ret = re.compile(r'mac=([a-z0-9:]+)').findall(line)
-                if ret:
-                    for mac in ret:
-                        # convert libvirt to local/native
-                        mac = 'fe' + mac[2:]
-                        _port = self.nethelp.get_interface_with_hwaddr(mac)
-                        if _port:
-                            guest.add_port(_port)
+    @property
+    def dev_to_dname(self):
+        for line in CLIHelper().udevadm_info_dev(device=self.dev):
+            expr = r'.+\s+disk/by-dname/(.+)'
+            ret = re.compile(expr).match(line)
+            if ret:
+                return ret[1]
 
-                ret = re.compile(r'.+\s-m\s+(\d+)').search(line)
-                if ret:
-                    guest.memory_mbytes = int(ret.group(1))
+    @property
+    def dev(self):
+        return os.path.basename(os.path.realpath(os.path.join(self.path,
+                                                              'dev')))
 
-                instances[uuid] = guest
+    @cached_property
+    def name(self):
+        return os.path.basename(self.path)
 
-        return instances
+    def __getattr__(self, key):
+        cfg = os.path.join(self.path, key)
+        if os.path.exists(cfg):
+            with open(cfg) as fd:
+                return fd.read().strip()
 
-    def get_nova_config_port(self, cfg_key):
-        """
-        Fetch interface used by Openstack Nova config. Returns NetworkPort.
-        """
-        addr = self.nova_config.get(cfg_key)
-        if not addr:
-            return
+        raise AttributeError("{} not found in bdev config".format(key))
 
-        return self.nethelp.get_interface_with_addr(addr)
 
-    @cached_property
-    def my_ip_port(self):
-        # NOTE: my_ip can be an address or fqdn, we currently only support
-        # searching by address.
-        return self.get_nova_config_port('my_ip')
+class Cacheset(object):
 
-    @cached_property
-    def live_migration_inbound_addr_port(self):
-        return self.get_nova_config_port('live_migration_inbound_addr')
+    def __init__(self, path):
+        self.path = path
+        self.bdevs = []
 
-    @cached_property
-    def bind_interfaces(self):
-        """
-        Fetch interfaces used by Openstack Nova. Returned dict is keyed by
-        config key used to identify interface.
-        """
-        interfaces = {}
-        if self.my_ip_port:
-            interfaces['my_ip'] = self.my_ip_port
-
-        if self.live_migration_inbound_addr_port:
-            port = self.live_migration_inbound_addr_port
-            interfaces['live_migration_inbound_addr'] = port
-
-        return interfaces
-
-
-class CPUPinning(NovaBase):
-
-    def __init__(self):
-        super().__init__()
-        self.numa = NUMAInfo()
-        self.systemd = SystemdConfig()
-        self.kernel = KernelConfig()
-        self.nova_cfg = OpenstackConfig(os.path.join(HotSOSConfig.data_root,
-                                                     'etc/nova/nova.conf'))
-        self.isolcpus = set(self.kernel.get('isolcpus',
-                                            expand_to_list=True) or [])
-        self.cpuaffinity = set(self.systemd.get('CPUAffinity',
-                                                expand_to_list=True) or [])
+        self.uuid = os.path.basename(self.path)
+        for bdev in glob.glob(os.path.join(self.path, 'bdev*')):
+            self.bdevs.append(BDev(bdev, self))
 
     @cached_property
-    def cpu_dedicated_set(self):
-        key = 'cpu_dedicated_set'
-        return self.nova_cfg.get(key, expand_to_list=True) or []
+    def cfg(self):
+        return BcacheConfig(self.path)
 
-    @cached_property
-    def cpu_shared_set(self):
-        key = 'cpu_shared_set'
-        return self.nova_cfg.get(key, expand_to_list=True) or []
+    def __getattr__(self, key):
+        cfg = os.path.join(self.path, key)
+        if os.path.exists(cfg):
+            with open(cfg) as fd:
+                return fd.read().strip()
 
-    @cached_property
-    def vcpu_pin_set(self):
-        key = 'vcpu_pin_set'
-        return self.nova_cfg.get(key, expand_to_list=True) or []
+        raise AttributeError("{} not found in cacheset config".format(key))
 
-    @cached_property
-    def cpu_dedicated_set_name(self):
-        """
-        If the vcpu_pin_set option has a value, we use that option as the name.
-        """
-        if self.vcpu_pin_set:
-            return 'vcpu_pin_set'
 
-        return 'cpu_dedicated_set'
+class BcacheBase(StorageBase):
 
-    @cached_property
-    def cpu_dedicated_set_intersection_isolcpus(self):
-        if self.vcpu_pin_set:
-            pinset = set(self.vcpu_pin_set)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.cachesets = []
+        self._bcache_devs = []
+        self.cli = CLIHelper()
+
+        for entry in glob.glob(os.path.join(HotSOSConfig.data_root,
+                               'sys/fs/bcache/*')):
+            if not os.path.isdir(entry):
+                continue
+
+            if not os.path.exists(os.path.join(entry,
+                                               'cache_available_percent')):
+                continue
+
+            self.cachesets.append(Cacheset(entry))
+
+    @cached_property
+    def bcache_enabled(self):
+        """ Return True if there are any backing devices configured. """
+        if self.cachesets:
+            for cset in self.cachesets:
+                if cset.bdevs:
+                    return True
+
+        return False
+
+    @cached_property
+    def udev_bcache_devs(self):
+        """ If bcache devices exist fetch information and return as a list. """
+        if self._bcache_devs:
+            return self._bcache_devs
+
+        udevadm_info = self.cli.udevadm_info_exportdb()
+        if not udevadm_info:
+            return self._bcache_devs
+
+        s = FileSearcher()
+        sdef = SequenceSearchDef(start=SearchDef(r"^P: .+/(bcache\S+)"),
+                                 body=SearchDef(r"^S: disk/by-uuid/(\S+)"),
+                                 tag="bcacheinfo")
+        s.add(sdef, mktemp_dump('\n'.join(udevadm_info)))
+        results = s.run()
+        devs = []
+        for section in results.find_sequence_sections(sdef).values():
+            dev = {}
+            for r in section:
+                if r.tag == sdef.start_tag:
+                    dev["name"] = r.get(1)
+                else:
+                    dev["by-uuid"] = r.get(1)
+
+            devs.append(dev)
+
+        self._bcache_devs = devs
+        return self._bcache_devs
+
+    def resolve_bdev_from_dev(self, devpath):
+        """
+        Given a device path, resolve it to a corresponding bcache BDev object.
+        """
+        bcache_name = None
+        if 'bcache' in devpath:
+            bcache_name = os.path.basename(devpath)
         else:
-            pinset = set(self.cpu_dedicated_set)
+            ret = re.compile(r"/dev/mapper/crypt-(\S+)").search(devpath)
+            if ret:
+                for udev_dev in self.udev_bcache_devs:
+                    if 'name' not in udev_dev:
+                        continue
 
-        return list(pinset.intersection(self.isolcpus))
+                    _uuid = udev_dev.get("by-uuid")
+                    if not _uuid or _uuid != ret.group(1):
+                        continue
 
-    @cached_property
-    def cpu_dedicated_set_intersection_cpuaffinity(self):
-        if self.vcpu_pin_set:
-            pinset = set(self.vcpu_pin_set)
-        else:
-            pinset = set(self.cpu_dedicated_set)
+                    bcache_name = udev_dev['name']
 
-        return list(pinset.intersection(self.cpuaffinity))
+        if bcache_name:
+            for cset in self.cachesets:
+                for bdev in cset.bdevs:
+                    if bdev.dev == bcache_name:
+                        return bdev
 
-    @cached_property
-    def cpu_shared_set_intersection_isolcpus(self):
-        return list(set(self.cpu_shared_set).intersection(self.isolcpus))
+    def is_bcache_device(self, dev):
+        """
+        Returns True if the device either is or is backed by a bcache device
+        e.g. dmcrypt device using bcache dev.
+        """
+        if dev.startswith("bcache"):
+            return True
 
-    @cached_property
-    def cpuaffinity_intersection_isolcpus(self):
-        return list(self.cpuaffinity.intersection(self.isolcpus))
+        if dev.startswith("/dev/bcache"):
+            return True
 
-    @cached_property
-    def cpu_shared_set_intersection_cpu_dedicated_set(self):
-        if self.vcpu_pin_set:
-            pinset = set(self.vcpu_pin_set)
-        else:
-            pinset = set(self.cpu_dedicated_set)
+        if self.resolve_bdev_from_dev(dev):
+            return True
 
-        return list(set(self.cpu_shared_set).intersection(pinset))
+        return False
 
-    @cached_property
-    def num_unpinned_cpus(self):
-        num_cpus = SystemBase().num_cpus
-        total_isolated = len(self.isolcpus.union(self.cpuaffinity))
-        return num_cpus - total_isolated
 
-    @cached_property
-    def unpinned_cpus_pcent(self):
-        num_cpus = SystemBase().num_cpus
-        if num_cpus and self.num_unpinned_cpus:
-            return int((float(100) / num_cpus) * self.num_unpinned_cpus)
+class BDevsConfig(BcacheBase):
 
-        return 0
+    def get(self, key):
+        """
+        This currently assumes there is only one cacheset on the host.
+        """
+        if self.cachesets and self.cachesets[0].bdevs:
+            return self.cachesets[0].bdevs[0].cfg.get(key)
 
-    @cached_property
-    def nova_pinning_from_multi_numa_nodes(self):
-        if self.vcpu_pin_set:
-            pinset = set(self.vcpu_pin_set)
-        else:
-            pinset = set(self.cpu_dedicated_set)
 
-        node_count = 0
-        for node in self.numa.nodes:
-            node_cores = set(self.numa.cores(node))
-            if pinset.intersection(node_cores):
-                node_count += 1
-
-        return node_count > 1
-
-
-class NovaInstance(object):
-    def __init__(self, uuid, name):
-        self.uuid = uuid
-        self.name = name
-        self.ports = []
-        self.memory_mbytes = None
+class CachesetsConfig(BcacheBase):
+
+    def get(self, key):
+        """
+        This currently assumes there is only one cacheset on the host.
+        """
+        if self.cachesets:
+            return self.cachesets[0].cfg.get(key)
+
+
+class BcacheChecksBase(BcacheBase):
+
+    @property
+    def summary_subkey(self):
+        return 'bcache'
 
-    def add_port(self, port):
-        self.ports.append(port)
+    @property
+    def plugin_runnable(self):
+        return self.bcache_enabled
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/openstack/octavia.py` & `hotsos-1.15.post1/hotsos/core/plugins/openstack/octavia.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/openstack/openstack.py` & `hotsos-1.15.post1/hotsos/core/plugins/openstack/openstack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from datetime import datetime
 import os
 
-from searchkit.constraints import TimestampMatcherBase
-
 from hotsos.core import host_helpers
 from hotsos.core.log import log
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.plugins.openstack.exceptions import (
     EXCEPTIONS_COMMON,
     BARBICAN_EXCEPTIONS,
     CASTELLAN_EXCEPTIONS,
@@ -24,19 +22,21 @@
     NEUTRONCLIENT_EXCEPTIONS,
     OCTAVIA_EXCEPTIONS,
     OS_VIF_EXCEPTIONS,
     OVSDBAPP_EXCEPTIONS,
     MASAKARI_EXCEPTIONS,
 )
 from hotsos.core.utils import cached_property
+from searchkit.constraints import TimestampMatcherBase
 
 
 # NOTE(tpsilva): when updating this, refer to the Charmed Openstack supported
 # versions page: https://ubuntu.com/openstack/docs/supported-versions
 OST_EOL_INFO = {
+    'antelope': datetime(2026, 4, 30),
     'zed': datetime(2024, 4, 30),
     'yoga': datetime(2027, 4, 30),
     'xena': datetime(2023, 4, 30),
     'wallaby': datetime(2024, 4, 30),
     'victoria': datetime(2022, 4, 30),
     'ussuri': datetime(2030, 4, 30),
     'train': datetime(2021, 2, 28),
@@ -116,14 +116,18 @@
         'wallaby': '1:16.0.0',
         'victoria': '1:15.0.0',
         'ussuri': '1:14.0.0',
         'train': '1:13.0.0',
         'stein': '1:12.0.0',
         'rocky': '1:11.0.0',
         'queens': '1:10.0.0'},
+    'ironic-common': {
+        'antelope': '1:21.2',
+        'zed': '1:20.2.0',
+        'yoga': '1:19.0.0'},
     'keystone': {
         'antelope': '2:23.0.0',
         'zed': '2:22.0.0',
         'yoga': '2:21.0.0',
         'xena': '2:20.0.0',
         'wallaby': '2:19.0.0',
         'victoria': '2:18.0.0',
@@ -374,44 +378,45 @@
 
     def __init__(self):
         self._projects = {}
         self.add('aodh', config={'main': 'aodh.conf'},
                  systemd_masked_services=['aodh-api'],
                  systemd_extra_services=['apache2'],
                  log_path_overrides={'apache2':
-                                     ['var/log/aodh/aodh-api.log']}),
+                                     ['var/log/aodh/aodh-api.log']})
         self.add('barbican', config={'main': 'barbican.conf'},
                  systemd_masked_services=['barbican-api'],
                  systemd_extra_services=['apache2'],
                  log_path_overrides={'apache2':
-                                     ['var/log/barbican/barbican-api.log']}),
+                                     ['var/log/barbican/barbican-api.log']})
         self.add('ceilometer', config={'main': 'ceilometer.conf'},
-                 systemd_masked_services=['ceilometer-api']),
+                 systemd_masked_services=['ceilometer-api'])
         self.add('cinder', config={'main': 'cinder.conf'},
                  systemd_extra_services=['apache2'],
                  log_path_overrides={'apache2':
-                                     ['var/log/apache2/cinder_*.log']}),
+                                     ['var/log/apache2/cinder_*.log']})
         self.add('designate', config={'main': 'designate.conf'},
-                 systemd_extra_services=['apache2']),
+                 systemd_extra_services=['apache2'])
         self.add('glance', config={'main': 'glance-api.conf'},
-                 systemd_extra_services=['apache2']),
+                 systemd_extra_services=['apache2'])
         self.add('gnocchi', config={'main': 'gnocchi.conf'},
                  systemd_masked_services=['gnocchi-api'],
                  systemd_extra_services=['apache2'],
                  log_path_overrides={'apache2':
-                                     ['var/log/gnocchi/gnocchi-api.log']}),
+                                     ['var/log/gnocchi/gnocchi-api.log']})
         self.add('heat', config={'main': 'heat.conf'},
-                 systemd_extra_services=['apache2']),
+                 systemd_extra_services=['apache2'])
         self.add('horizon', apt_core_alt=['openstack-dashboard'],
-                 systemd_extra_services=['apache2']),
+                 systemd_extra_services=['apache2'])
+        self.add('ironic', config={'main': 'ironic.conf'})
         self.add('keystone', config={'main': 'keystone.conf'},
                  systemd_masked_services=['keystone'],
                  systemd_extra_services=['apache2'],
                  log_path_overrides={'apache2':
-                                     ['var/log/keystone/keystone.log']}),
+                                     ['var/log/keystone/keystone.log']})
         self.add('neutron',
                  config={'main': 'neutron.conf',
                          'openvswitch-agent':
                          'plugins/ml2/openvswitch_agent.ini',
                          'l3-agent': 'l3_agent.ini',
                          'dhcp-agent': 'dhcp_agent.ini',
                          'ovn': 'ovn.ini'},
@@ -423,40 +428,40 @@
         self.add('nova', config={'main': 'nova.conf'},
                  # See LP bug 1957760 for reason why neutron-server is added.
                  systemd_masked_services=['nova-api-os-compute',
                                           'neutron-server'],
                  systemd_extra_services=['apache2'],
                  log_path_overrides={'apache2':
                                      ['var/log/apache2/nova-*.log',
-                                      'var/log/nova/nova-api-wsgi.log']}),
+                                      'var/log/nova/nova-api-wsgi.log']})
         self.add('manila', config={'main': 'manila.conf'},
                  systemd_masked_services=['manila-api'],
                  systemd_extra_services=['apache2'],
                  log_path_overrides={'apache2':
-                                     ['var/log/manila/manila-api.log']}),
+                                     ['var/log/manila/manila-api.log']})
         self.add('masakari', config={'main': 'masakari.conf'},
                  systemd_masked_services=['masakari'],
                  systemd_extra_services=['apache2', 'masakari-engine'],
                  log_path_overrides={'apache2':
-                                     ['var/log/apache2/masakari_error.log']}),
+                                     ['var/log/apache2/masakari_error.log']})
         self.add('octavia', config={'main': 'octavia.conf',
                                     'amphora': 'amphora-agent.conf'},
                  systemd_masked_services=['octavia-api'],
                  apt_core_alt=[r'amphora-\S+'],
                  systemd_extra_services=['apache2', 'amphora-agent'],
                  log_path_overrides={'apache2':
-                                     ['var/log/octavia/octavia-api.log']}),
+                                     ['var/log/octavia/octavia-api.log']})
         self.add('placement', config={'main': 'placement.conf'},
                  systemd_masked_services=['placement'],
                  systemd_extra_services=['apache2'],
                  log_path_overrides={'apache2':
-                                     ['var/log/apache2/*error.log']}),
+                                     ['var/log/apache2/*error.log']})
         self.add('swift', config={'main': 'swift-proxy.conf',
                                   'proxy': 'swift-proxy.conf'},
-                 systemd_extra_services=['apache2']),
+                 systemd_extra_services=['apache2'])
 
     def __getitem__(self, name):
         return self._projects[name]
 
     def __getattr__(self, name):
         if name in self._projects:
             return self._projects[name]
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/openvswitch/common.py` & `hotsos-1.15.post1/hotsos/core/plugins/openvswitch/common.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from searchkit.constraints import TimestampMatcherBase
 
 from hotsos.core import plugintools
 from hotsos.core.host_helpers import (
     APTPackageHelper,
     PebbleHelper,
     SystemdHelper,
 )
 from hotsos.core.ycheck.events import YEventCheckerBase
 from hotsos.core.utils import cached_property, sorted_dict
+from searchkit.constraints import TimestampMatcherBase
 
 OVS_SERVICES_EXPRS = [r'ovsdb[a-zA-Z-]*',
                       r'ovs-vswitch[a-zA-Z-]*',
                       r'ovn[a-zA-Z-]*',
                       'openvswitch-switch',
                       ]
 OVS_PKGS_CORE = ['openvswitch-switch',
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/openvswitch/ovn.py` & `hotsos-1.15.post1/hotsos/core/plugins/openvswitch/ovn.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,16 @@
 
     def __init__(self):
         contents = mktemp_dump(''.join(self.db_show))
         s = FileSearcher()
         s.add(self.resources_sd, contents)
         self.results = s.run()
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def db_show(self):
         """ e.g. ovn-sbctl show  """
 
     @cached_property
     def resources_sd(self):
         start = SearchDef([r"^(\S+)\s+(\S+)\s*.*"])
         body = SearchDef(r"^\s+(\S+)\s+(.+)")
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/openvswitch/ovs.py` & `hotsos-1.15.post1/hotsos/core/plugins/openvswitch/ovs.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/pacemaker.py` & `hotsos-1.15.post1/hotsos/core/plugins/pacemaker.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/rabbitmq/common.py` & `hotsos-1.15.post1/hotsos/core/plugins/rabbitmq/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/rabbitmq/report.py` & `hotsos-1.15.post1/hotsos/core/plugins/rabbitmq/report.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/sosreport.py` & `hotsos-1.15.post1/hotsos/core/plugins/sosreport.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/storage/ceph.py` & `hotsos-1.15.post1/hotsos/core/plugins/storage/ceph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,12 @@
+from datetime import datetime
 import os
 import re
-import sys
 import subprocess
-
-from datetime import datetime
-
-from searchkit.constraints import TimestampMatcherBase
+import sys
 
 from hotsos.core.factory import FactoryBase
 from hotsos.core.log import log
 from hotsos.core.utils import (
     cached_property,
     mktemp_dump,
     sorted_dict,
@@ -31,14 +28,15 @@
 from hotsos.core.plugins.storage.bcache import BcacheBase
 from hotsos.core.search import (
     FileSearcher,
     SequenceSearchDef,
     SearchDef
 )
 from hotsos.core.plugins.kernel.net import Lsof
+from searchkit.constraints import TimestampMatcherBase
 
 CEPH_SERVICES_EXPRS = [r"ceph-[a-z0-9-]+",
                        r"rados[a-z0-9-:]+"]
 CEPH_PKGS_CORE = [r"ceph",
                   r"rados",
                   r"rbd",
                   ]
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/system/system.py` & `hotsos-1.15.post1/hotsos/core/plugins/system/system.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugins/vault.py` & `hotsos-1.15.post1/hotsos/core/plugins/vault.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/plugintools.py` & `hotsos-1.15.post1/hotsos/core/plugintools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
-import yaml
-
-from jinja2 import FileSystemLoader, Environment
 
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.log import log
 from hotsos.core.issues import IssuesManager
 from hotsos.core.ycheck.scenarios import YScenarioChecker
+from jinja2 import FileSystemLoader, Environment
+import yaml
 
 
 def summary_entry_offset(offset):
     def _inner(f):
         def _inner2(*args, **kwargs):
             out = f(*args, **kwargs)
             if out is not None:
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/search.py` & `hotsos-1.15.post1/hotsos/core/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     ResultFieldInfo,
     SearchDef,
     SequenceSearchDef,
 )
 from searchkit.constraints import (
     SearchConstraintSearchSince as _SearchConstraintSearchSince
 )
-
 from hotsos.core.log import log
 from hotsos.core.host_helpers.cli import CLIHelper
 from hotsos.core.config import HotSOSConfig
 
 
 class FileSearcher(_FileSearcher):
     def __init__(self, *args, **kwargs):
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/utils.py` & `hotsos-1.15.post1/hotsos/core/utils.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/common.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/common.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
-import yaml
 
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.log import log
+import yaml
 
 
 class YDefsLoader(object):
     """ Load yaml definitions. """
 
     def __init__(self, ytype):
         """
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/checks.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/checks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,42 @@
-from hotsos.core.config import HotSOSConfig
 from hotsos.core.log import log
-from hotsos.core.search import (
-    FileSearcher,
-    SearchConstraintSearchSince,
-)
 from hotsos.core.ycheck.engine.properties.common import (
     cached_yproperty_attr,
     YPropertyOverrideBase,
     YPropertyMappedOverrideBase,
     YDefsSection,
     add_to_property_catalog,
     YDefsContext,
 )
 from hotsos.core.ycheck.engine.properties.requires.requires import (
     YPropertyRequires
 )
 from hotsos.core.ycheck.engine.properties.search import (
     YPropertySearch,
-    CommonTimestampMatcher,
 )
 from hotsos.core.ycheck.engine.properties.input import YPropertyInput
 
-MAX_CACHED_SEARCH_RESULTS = 100
-
 
 @add_to_property_catalog
 class YPropertyCheck(YPropertyMappedOverrideBase):
 
     @property
-    def first_search_result(self):
-        return self.cache.first_search_result
-
-    @property
     def _search_results(self):
         """
         Retrieve the global searchkit.SearchResultsCollection from this
         property's context. We filter results using our tag and apply any
         search constraints requested.
         """
         global_results = self.context.search_results
         if global_results is not None:
             tag = self.search.unique_search_tag
             _results = global_results.find_by_tag(tag)
             log.debug("check %s has %s search results with tag %s",
                       self.check_name, len(_results), tag)
-            ret = self.search.apply_constraints(_results)
-            if ret:
-                self.cache.set('first_search_result', ret[0])
-
-            return ret
+            return self.search.apply_constraints(_results)
 
         raise Exception("no search results provided to check '{}'".
                         format(self.check_name))
 
     @classmethod
     def _override_keys(cls):
         return ['check']
@@ -64,52 +48,36 @@
     @property
     def name(self):
         if hasattr(self, 'check_name'):
             return getattr(self, 'check_name')
 
     def _set_search_cache_info(self, results):
         """
-        Set information in the local property cache that can be retrieved
-        using PropertyCacheRefResolver. This information is typically used
+        Set information in check cache so that it can be retrieved using
+        PropertyCacheRefResolver. This information is typically used
         when creating messages as part of raising issues.
 
+        IMPORTANT: do not cache search results themselves as this can consume a
+                   lot of memory.
+
         @param results: search results for query in search property found in
                         this check.
         """
+        # this is so that the information can be accessed like:
+        # @checks.<checkname>.search.<setting>
+        self.cache.set('search', self.search.cache)
         self.search.cache.set('num_results', len(results))
         if not results:
             return
 
-        # The following aggregates results by group/index and stores in
-        # the property cache to make them accessible via
-        # PropertyCacheRefResolver.
-        # NOTE: we cap at MAX_CACHED_SEARCH_RESULTS results to save memory
-        results_by_idx = {}
-        for i, result in enumerate(results):
-            if i > MAX_CACHED_SEARCH_RESULTS:
-                break
-
-            for idx, value in enumerate(result):
-                if idx not in results_by_idx:
-                    results_by_idx[idx] = set()
-
-                results_by_idx[idx].add(value)
-
-        for idx in results_by_idx:
-            self.search.cache.set('results_group_{}'.format(idx),
-                                  list(results_by_idx[idx]))
-
         # Saves a list of files that contained search results.
         sources = set([r.source_id for r in results])
         files = [self.context.search_obj.resolve_source_id(s) for s in sources]
         self.search.cache.set('files', files)
 
-        # make it available from this property
-        self.cache.set('search', self.search.cache)
-
     def _result(self):
         if self.search:
             _results = self._search_results
             self._set_search_cache_info(_results)
             if not _results:
                 log.debug("check %s search has no matches so result=False",
                           self.name)
@@ -141,54 +109,50 @@
 @add_to_property_catalog
 class YPropertyChecks(YPropertyOverrideBase):
 
     @classmethod
     def _override_keys(cls):
         return ['checks']
 
-    def initialise(self, vars, input):
+    def initialise(self, vars, input, searcher, scenario):
         """
         Perform initialisation tasks for this set of checks.
 
         * create context containing vars for each check
         * pre-load searches from all/any checks and get results. This needs to
           be done before check results are consumed.
+
+        @param vars: YPropertyVars object containing all variables defined in
+                     the context of these checks and that we wil pass on to all
+                     check def and properties.
+        @param input: YPropertyInput object
+        @param searcher: FileSearcher object
         """
         self.check_context = YDefsContext({'vars': vars})
 
-        log.debug("loading checks searchdefs into filesearcher")
-
-        if HotSOSConfig.use_all_logs:
-            hours = 24 * HotSOSConfig.max_logrotate_depth
-        else:
-            hours = 24
-
-        c = SearchConstraintSearchSince(ts_matcher_cls=CommonTimestampMatcher,
-                                        hours=hours)
-        s = FileSearcher(constraint=c)
+        log.debug("pre-loading scenario '%s' checks searches into "
+                  "filesearcher", scenario.name)
         # first load all the search definitions into the searcher
         for c in self._checks:
             if c.search:
                 # local takes precedence over global
                 _input = c.input or input
                 if _input.command:
                     # don't apply constraints to command outputs
                     allow_constraints = False
                 else:
                     allow_constraints = True
 
                 for path in _input.paths:
                     log.debug("loading searches for check %s", c.check_name)
-                    c.search.load_searcher(s, path,
+                    c.search.load_searcher(searcher, path,
                                            allow_constraints=allow_constraints)
 
         # provide results to each check object using global context
-        log.debug("executing check searches")
-        self.check_context.search_obj = s
-        self.check_context.search_results = s.run()
+        self.check_context.search_obj = searcher
 
     @cached_yproperty_attr
     def _checks(self):
         log.debug("parsing checks section")
         if not hasattr(self, 'check_context'):
             raise Exception("checks not yet initialised")
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/common.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import abc
 import builtins
 import inspect
 import importlib
 
+from hotsos.core.log import log
 from propertree import (
     PTreeOverrideBase,
     PTreeMappedOverrideBase,
     PTreeSection,
 )
 
-from hotsos.core.log import log
-
 YPropertiesCatalog = []
 
 
 class ImportPathIsNotAClass(Exception):
     def __init__(self, msg):
         self.msg = msg
         super().__init__()
@@ -74,15 +73,18 @@
         """
         @param initial_state: optional dict to use as initial state.
         """
         self._ydefs_context = initial_state or {}
 
     def __setattr__(self, key, value):
         if key != '_ydefs_context':
-            log.debug("%s setting %s=%s", self.__class__.__name__, key, value)
+            # don't print values as they can be very large and e.g. search
+            # results will be expanded re-duplicated.
+            log.debug("%s setting %s with value of type '%s'",
+                      self.__class__.__name__, key, type(value))
             self._ydefs_context[key] = value
             return
 
         super().__setattr__(key, value)
 
     def __getattr__(self, key):
         return self._ydefs_context.get(key)
@@ -185,44 +187,89 @@
         if self.reftype == 'checks':
             _key = self._ref_body.partition('.')[2]
         else:
             _key = self._ref_body
 
         return _key.partition(':')[2]
 
-    def apply_renderer_function(self, value):
+    @staticmethod
+    def apply_renderer(value, func):
         """
-        The last section of a ref string can be a colon followed by a function
-        name which itself can be one of two things; any method supported by
-        builtins or "comma_join".
-        """
-        func = self.property_cache_value_renderer_function
-        if func:
-            if func == "comma_join":
-                # needless to say this will only work with lists, dicts etc.
-                return ', '.join(value)
-
-            return getattr(builtins, func)(value)
+        A cache reference or import path can be suffixed with :<function>
+        where <function> can be one of two things; either a builtins function
+        or one of the extras defined here. Obviously not all builtins can be
+        used and their use depends on the type() of value.
+
+        @param value: value to apply renderer function to
+        @param func: function to apply to value
+        """
+        extras = {'comma_join': {
+                    'requirements': [lambda value: isinstance(value, list),
+                                     lambda value: isinstance(value, dict)],
+                    'action': lambda value: ', '.join(value)},
+                  'unique_comma_join': {
+                    'requirements': [lambda value: isinstance(value, list),
+                                     lambda value: isinstance(value, dict)],
+                    'action': lambda value: ', '.join(sorted(set(value)))},
+                  'first': {
+                    'requirements': [lambda value: isinstance(value, list)],
+                    'action': lambda value: value[0]}}
+
+        if func in extras:
+            if not any([req(value) for req in extras[func]['requirements']]):
+                log.warning("attempted to apply '%s' to value of "
+                            "type %s", func, type(value))
+                return value
+
+            return extras[func]['action'](value)
+
+        return getattr(builtins, func)(value)
+
+    def _get_search_result_group(self, cache_key):
+        """
+        Extract values at the given group index from all search results.
+        """
+        val = []
+        group = int(cache_key.partition('results_group_')[2])
+        for result in self.checks[self.check_name]._search_results:
+            if len(result) >= group:
+                val.append(result.get(group))
 
-        return value
+        return sorted(val)
 
     def resolve(self):
+        """
+        Resolve value associated with a check property result or variable.
+
+        Values are then run through an optional renderer function.
+        """
         if self.reftype == 'checks':
-            check_cache = self.checks[self.check_name].cache
-            property_cache = getattr(check_cache, self.property_name)
-            val = getattr(property_cache, self.property_cache_key)
+            cache_key = self.property_cache_key
+            # This provides an interface to extract the values of specific
+            # search result groups.
+            if cache_key.startswith('results_group_'):
+                val = self._get_search_result_group(cache_key)
+            else:
+                check_cache = self.checks[self.check_name].cache
+                property_cache = getattr(check_cache, self.property_name)
+                val = getattr(property_cache, cache_key)
         else:
             varname = self.refstr.partition("$")[2]
             varname = varname.partition(':')[0]
             val = self.vars.resolve(varname)
 
         if val is None:
             return
 
-        return self.apply_renderer_function(val)
+        func = self.property_cache_value_renderer_function
+        if not func:
+            # noop
+            return val
+
+        return self.apply_renderer(val, func)
 
 
 class PropertyCache(object):
 
     def __init__(self):
         self._property_cache_data = {}
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/conclusions.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/conclusions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import builtins
-
 from hotsos.core.exceptions import ScenarioException
 from hotsos.core.issues import IssueContext
 from hotsos.core.log import log
 from hotsos.core.ycheck.engine.properties.common import (
     cached_yproperty_attr,
     YPropertyOverrideBase,
     PropertyCacheRefResolver,
@@ -40,15 +38,15 @@
         return self.content.get('bug-id')
 
     @property
     def message(self):
         """ optional setting. do this to allow querying. """
         return self.content.get('message')
 
-    def message_with_format_dict_applied(self, checks=None):
+    def message_formatted(self, checks=None):
         """
         If a format-dict is provided this will resolve any cache references
         then format the message. Returns formatted message.
 
         @params checks: optional dict of YPropertyChecks objects.
         """
         fdict = self.format_dict
@@ -66,74 +64,44 @@
 
         message = self.message
         if message is not None:
             message = str(message).format(**fdict)
 
         return message
 
-    def message_with_format_list_applied(self, searchresult):
-        """
-        If format-groups have been provided this will extract their
-        corresponding values from searchresult and use them to format the
-        message. Returns formatted message.
-
-        @param searchresult: a search.SearchResult object.
-        """
-        if not self.format_groups:
-            return self.message
-
-        format_list = []
-        for idx in self.format_groups:
-            format_list.append(searchresult.get(idx))
-
-        message = self.message
-        if message is not None:
-            message = str(message).format(*format_list)
-
-        return message
-
-    def apply_renderer_function(self, value, func):
-        if not func:
-            return value
-
-        if func == "comma_join":
-            # needless to say this will only work with lists, dicts etc.
-            return ', '.join(value)
-
-        return getattr(builtins, func)(value)
-
     @cached_yproperty_attr
     def format_dict(self):
         """
         Optional dict of key/val pairs used to format the message string.
 
-        Keys that start with @ are used as references to properties allowing
-        us to extract cached values.
+        Keys that start with @ are used as references to yaml properties
+        allowing us to extract cached values. Alternatively an import path
+        can be specified in which case the value is imported immediately and
+        optional rendering function applied.
         """
         _format_dict = self.content.get('format-dict')
         if not _format_dict:
             return {}
 
         fdict = {}
         for k, v in _format_dict.items():
             if PropertyCacheRefResolver.is_valid_cache_ref(v):
-                # save string for later parsing/extraction
+                # save for later parsing/extraction
                 fdict[k] = v
-            else:
-                func = v.partition(':')[2]
-                v = v.partition(':')[0]
-                fdict[k] = self.apply_renderer_function(self.get_import(v),
-                                                        func)
+                continue
 
-        return fdict
+            # process now since there is no cache to resolve
+            path, _, func = v.partition(':')
+            value = self.get_import(path)
+            if func:
+                value = PropertyCacheRefResolver.apply_renderer(value, func)
 
-    @cached_yproperty_attr
-    def format_groups(self):
-        """ optional setting. do this to allow querying. """
-        return self.content.get('search-result-format-groups')
+            fdict[k] = value
+
+        return fdict
 
     @cached_yproperty_attr
     def type(self):
         """ Name of core.issues.IssueTypeBase object and will be used to raise
         an issue or bug using message as argument. """
         _type = "hotsos.core.issues.{}".format(self.content['type'])
         return self.get_cls(_type)
@@ -212,50 +180,24 @@
         self.decision.add_checks_instances(checks)
         log.debug("decision:start")
         result = self.decision.run_collection()
         log.debug("decision:end")
         if not result:
             return False
 
-        first_search_result = None
-        for check in checks.values():
-            if check.search and check.first_search_result:
-                first_search_result = check.first_search_result
-
-            # FIXME: disabling for now because if the cache contains
-            # data that cant be saved at yaml this will lead to errors.
-            """
-            if check.requires:
-                # Dump the requires cache into the context. We improve this
-                # later by adding more info.
-                self.issue_context.set(**check.requires.cache.data)
-            """
-
-        if self.raises.format_groups:
-            if first_search_result:
-                # we only use the first result
-                message = self.raises.message_with_format_list_applied(
-                                                           first_search_result)
-            else:
-                message = self.raises.message
-                log.warning("no search results found so not applying format "
-                            "groups")
-        else:
-            message = self.raises.message_with_format_dict_applied(
-                                                                 checks=checks)
-
         bug_id = self.raises.bug_id
         bug_type = self.raises.type.ISSUE_TYPE
         is_bug_type = bug_type == 'bug'
         if ((is_bug_type and bug_id is None) or
                 (bug_id is not None and not is_bug_type)):
             msg = ("both bug-id (current={}) and bug type (current={}) "
                    "required in order to raise a bug".format(bug_id, bug_type))
             raise ScenarioException(msg)
 
+        message = self.raises.message_formatted(checks=checks)
         if self.raises.type.ISSUE_TYPE == 'bug':
             self.issue = self.raises.type(self.raises.bug_id, message)
         else:
             self.issue = self.raises.type(message)
 
         return result
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/input.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/input.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/common.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
 class PackageCheckItemsBase(CheckItemsBase):
 
     @cached_property
     def packages_to_check(self):
         return [item[0] for item in self]
 
+    @property
     @abc.abstractmethod
     def packaging_helper(self):
         """
         Returns and implementation of host_helpers.packaging.PackageHelperBase
         e.g. APTPackagehelper or SnapPackageHelper.
         """
 
@@ -160,15 +161,16 @@
                                    force_expected=force_expected)
 
         return input
 
 
 class YRequirementTypeBase(YPropertyOverrideBase, OpsUtils):
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def _result(self):
         """ Assert whether the requirement is met.
 
         Returns True if met otherwise False.
         """
 
     def __call__(self):
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/requires.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/requires.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/apt.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/apt.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,18 @@
     YRequirementTypeBase,
     PackageCheckItemsBase,
 )
 
 
 class APTCheckItems(PackageCheckItemsBase):
 
+    # NOTE: the following pylint disable can be removed when we move to newer
+    #       pylint.
     @cached_property
-    def packaging_helper(self):
+    def packaging_helper(self):  # pylint: disable=W0236
         return APTPackageHelper(self.packages_to_check)
 
     @cached_property
     def installed_versions(self):
         _versions = []
         for p in self.installed:
             _versions.append(self.packaging_helper.get_version(p))
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/config.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/path.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/path.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/pebble.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/pebble.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/property.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/property.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/snap.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/snap.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,18 @@
     YRequirementTypeBase,
     PackageCheckItemsBase,
 )
 
 
 class SnapCheckItems(PackageCheckItemsBase):
 
+    # NOTE: the following pylint disable can be removed when we move to newer
+    #       pylint.
     @cached_property
-    def packaging_helper(self):
+    def packaging_helper(self):  # pylint: disable=W0236
         return SnapPackageHelper(core_snaps=self.packages_to_check)
 
     @cached_property
     def installed_revisions(self):
         _revisions = []
         for p in self.installed:
             _revisions.append(self.packaging_helper.get_revision(p))
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/systemd.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/systemd.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/requires/types/varops.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/requires/types/varops.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/search.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,48 @@
-from searchkit.constraints import TimestampMatcherBase
-
 from datetime import (
     datetime,
     timedelta,
 )
+import re
+
 from hotsos.core.host_helpers import UptimeHelper, CLIHelper
 from hotsos.core.log import log
+from hotsos.core.utils import cached_property
 from hotsos.core.search import (
     SearchDef,
     SequenceSearchDef,
     SearchConstraintSearchSince,
 )
 from hotsos.core.ycheck.engine.properties.common import (
     cached_yproperty_attr,
     YPropertyOverrideBase,
     YPropertyMappedOverrideBase,
     add_to_property_catalog,
 )
+from searchkit.constraints import TimestampMatcherBase
 
 
 class CommonTimestampMatcher(TimestampMatcherBase):
     MONTH_MAP = {'jan': 1, 'feb': 2, 'mar': 3, 'apr': 4, 'may': 5,
                  'jun': 6, 'jul': 7, 'aug': 8, 'sep': 9, 'oct': 10,
                  'nov': 11, 'dec': 12}
 
+    @cached_property
+    def _current_year(self):
+        return CLIHelper().date(format='+%Y')
+
     @property
     def year(self):
         """ Needed for kernlog which has no year group. """
-        if 'year' in self.result.groups():
+        try:
             return self.result.group('year')
+        except IndexError:
+            pass
 
-        return CLIHelper().date(format='+%Y')
+        return self._current_year
 
     @property
     def month(self):
         """ Needed for kernlog which has a string month. """
         try:
             return int(self.result.group('month'))
         except ValueError:
@@ -75,14 +83,19 @@
 
 class YPropertySearchConstraints(YPropertyOverrideBase):
 
     @classmethod
     def _override_keys(cls):
         return ['constraints']
 
+    @property
+    def valid_attributes(self):
+        return ['search-period-hours', 'search-result-age-hours',
+                'min-hours-since-last-boot', 'min-results']
+
     @cached_yproperty_attr
     def search_period_hours(self):
         """
         If min is provided this is used to determine the period within which
         min applies. If period is unset, the period is infinite i.e. across all
         available data.
 
@@ -117,14 +130,25 @@
 
     @cached_yproperty_attr
     def filesearch_constraints_obj(self):
         """
         Create a search constraints object representing the paramaters in
         this property.
         """
+        invalid = []
+        for attr in self.content:
+            if attr not in self.valid_attributes:
+                invalid.append(attr)
+
+        if invalid:
+            raise Exception("Invalid search constraints attributes found: {}. "
+                            "Valid options are: {}".
+                            format(', '.join(invalid),
+                                   ', '.join(self.valid_attributes)))
+
         has_result_hours = 'search-result-age-hours' in self.content
         has_boot_hours = 'min-hours-since-last-boot' in self.content
         if not any([has_result_hours, has_boot_hours]):
             return
 
         uptime_etime_hours = UptimeHelper().hours
         hours = self.search_result_age_hours
@@ -180,34 +204,27 @@
         to do so it will return None. The normal expectation is that two search
         result groups be available at index 1 and 2 but if only 1 is valid it
         will be used a fallback.
         """
         ts = result.get(1)
         if result.get(2):
             ts = "{} {}".format(ts, result.get(2))
+        else:
+            ts = "{} 00:00:00".format(ts)
 
-        ts_formats = ["%Y-%m-%d %H:%M:%S.%f", "%Y-%m-%d %H:%M:%S", "%Y-%m-%d"]
-        for format in ts_formats:
-            try:
-                return datetime.strptime(ts, format)
-            except ValueError:
-                continue
-
-        ts = result.get(1)
-        for format in ts_formats:
-            try:
-                return datetime.strptime(ts, format)
-            except ValueError:
-                continue
+        ts_matcher = CommonTimestampMatcher(ts)
+        if ts_matcher.matched:
+            return ts_matcher.strptime
 
-        log.warning("failed to parse timestamp string 1='%s' 2='%s' - "
-                    "returning None", result.get(1), result.get(2))
+        log.warning("failed to parse timestamp string '%s' (num_group=%s) - "
+                    "returning None", ts, len(result))
 
     @classmethod
     def filter_by_age(cls, results, result_age_hours):
+        """ Return results from the last result_age_hours. """
         if not result_age_hours:
             log.debug("result age filter not specified - skipping")
             return results
 
         current = CLIHelper().date(format='+%Y-%m-%d %H:%M:%S')
         if not current:
             log.warning("date() returned unexpected value '%s' - skipping "
@@ -225,47 +242,50 @@
                 _results.append(r)
 
         log.debug("%s results remain after applying filter", len(_results))
         return _results
 
     @classmethod
     def filter_by_period(cls, results, period_hours):
+        """ Return the most recent period_hours worth of results. """
         if not period_hours:
             log.debug("period filter not specified - skipping")
             return results
 
         log.debug("applying search filter (period_hours=%s)", period_hours)
 
         _results = []
         for r in results:
             ts = cls.get_datetime_from_result(r)
             if ts:
                 _results.append((ts, r))
 
         results = []
         last = None
-        prev = None
 
         for r in sorted(_results, key=lambda i: i[0], reverse=True):
             if last is None:
                 last = r[0]
             elif r[0] < last - timedelta(hours=period_hours):
-                last = prev
-                prev = None
-                # pop first element since it is now invalidated
-                results = results[1:]
-            elif prev is None:
-                prev = r[0]
+                break
 
             results.append(r)
 
         log.debug("%s results remain after applying filter", len(results))
         return [r[1] for r in results]
 
     def apply_constraints(self, results):
+        """
+        NOTE: this is mostly unneeded now that we apply constraints in the
+              searches themselves but for occasions where timestamp cannot be
+              extracted form the start of a line, the searcher will assume the
+              line is valid and therefore we still need to post-process these
+              lines. The number of lines this applies to should always be very
+              small.
+        """
         if not self.constraints:
             log.debug("no search constraints to apply")
             return results
 
         log.debug("applying search constraints")
         count = len(results)
         result_age_hours = self.constraints.search_result_age_hours
@@ -312,14 +332,23 @@
     @property
     def search_pattern(self):
         if self.expr:
             return self._resolve_exprs(self.expr.expr)
 
         # can be supplied as a single string or list of strings
         patterns = self._resolve_exprs(list(self.content.keys()))
+        if len(patterns) == 0:
+            raise Exception("no search pattern (expr) defined")
+
+        for pattern in patterns:
+            if not re.search(r"[^\\]\(", pattern):
+                log.info("pattern '%s' does not contain a subgroup. this "
+                         "is inefficient and can result in unnecessary "
+                         "memory consumption", pattern)
+
         if len(patterns) == 1:
             return patterns[0]
 
         return patterns
 
     @property
     def is_sequence_search(self):
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/engine/properties/vars.py` & `hotsos-1.15.post1/hotsos/core/ycheck/engine/properties/vars.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/events.py` & `hotsos-1.15.post1/hotsos/core/ycheck/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,26 @@
                     if not set([None, None, None]).intersection([r.get(1),
                                                                  r.get(2),
                                                                  r.get(3)]):
                         results.append({'date': r.get(1), 'time': r.get(2),
                                         'key': r.get(3)})
                     else:
                         _fail_count += 1
+                elif len(r) < 1:
+                    msg = ("result (tag={}) does not have enough groups "
+                           "(min 1) to be categorised - aborting".
+                           format(r.tag))
+                    raise Exception(msg)
                 else:
+                    if len(r) < 2:
+                        # results with just a date will have None for the key
+                        log.debug("result (tag=%s) has just one group which "
+                                  "is assumed to be a date and using key=None",
+                                  r.tag)
+
                     results.append({'date': r.get(1), 'key': r.get(2)})
 
             if _fail_count:
                 log.info("event '%s' has %s results with insufficient fields",
                          event.name, _fail_count)
 
         for r in results:
```

### Comparing `hotsos-1.1.14.post9/hotsos/core/ycheck/scenarios.py` & `hotsos-1.15.post1/hotsos/core/ycheck/scenarios.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.issues import IssuesManager, HotSOSScenariosWarning
 from hotsos.core.log import log
+from hotsos.core.search import (
+    FileSearcher,
+    SearchConstraintSearchSince,
+)
 from hotsos.core.ycheck.engine import (
     YDefsLoader,
     YDefsSection,
     YHandlerBase,
 )
+from hotsos.core.ycheck.engine.properties.search import (
+    CommonTimestampMatcher,
+)
 
 
 class Scenario(object):
     def __init__(self, name, checks, conclusions):
         log.debug("scenario: %s", name)
         self.name = name
         self._checks = checks
@@ -43,31 +50,48 @@
             return
 
         log.debug("sections=%s, scenarios=%s",
                   len(yscenarios.branch_sections),
                   len(yscenarios.leaf_sections))
 
         to_skip = set()
+
+        if HotSOSConfig.use_all_logs:
+            hours = 24 * HotSOSConfig.max_logrotate_depth
+        else:
+            hours = 24
+
+        c = SearchConstraintSearchSince(ts_matcher_cls=CommonTimestampMatcher,
+                                        hours=hours)
+        searcher = FileSearcher(constraint=c)
+        checks = []
         for scenario in yscenarios.leaf_sections:
             # Only register scenarios if requirements are satisfied.
             group_name = scenario.parent.name
             if (not HotSOSConfig.force_mode and
                     (group_name in to_skip or
                         (scenario.requires and not scenario.requires.passes))):
                 log.debug("%s requirements not met - skipping scenario %s",
                           group_name, scenario.name)
                 to_skip.add(group_name)
                 continue
 
-            scenario.checks.initialise(scenario.vars, scenario.input)
+            checks.append(scenario.checks)
+            scenario.checks.initialise(scenario.vars, scenario.input, searcher,
+                                       scenario)
             scenario.conclusions.initialise(scenario.vars)
             self._scenarios.append(Scenario(scenario.name,
                                             scenario.checks,
                                             scenario.conclusions))
 
+        log.debug("executing check searches")
+        results = searcher.run()
+        for check in checks:
+            check.check_context.search_results = results
+
     @property
     def scenarios(self):
         return self._scenarios
 
     def _run_scenario_conclusion(self, scenario, issue_mgr):
         """ Determine the conclusion of this scenario. """
         results = {}
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/events/openstack/neutron/agents.yaml` & `hotsos-1.15.post1/hotsos/defs/events/openstack/neutron/agents.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,44 @@
+# NOTE: for efficiency, do not capture time as subgroup unless actually necessary.
 neutron-ovs-agent:
   input:
     path: 'var/log/neutron/neutron-openvswitch-agent.log'
     options:
       # Disabling all-logs for now since running against a long
       # history of logs can generate a very large amount of data that can
       # consume too much memory.
       disable-all-logs: True
   # identify rpc_loop iterations and get stats and longest running loops.
   rpc-loop:
     start:
-      expr: '^([0-9\-]+) (\S+) .+ Agent rpc_loop - iteration:([0-9]+) started.*'
+      expr: '([\d-]+) ([\d:]+\.\d{3}) .+ Agent rpc_loop - iteration:([0-9]+) started.*'
       hint: 'Agent rpc_loop'
     end:
-      expr: '^([0-9\-]+) (\S+) .+ Agent rpc_loop - iteration:([0-9]+) completed..+'
+      expr: '([\d-]+) ([\d:]+\.\d{3}) .+ Agent rpc_loop - iteration:([0-9]+) completed..+'
       hint: 'Agent rpc_loop'
     # we want to analyse these with core.analytics.LogEventStats so don't treat as sequence.
     passthrough-results: True      
 neutron-l3-agent:
   input:
     path: 'var/log/neutron/neutron-l3-agent.log'
   # identify router updates that took the longest to complete and report the longest updates.
   router-updates:
     start:
-      expr: '^([0-9-]+) (\S+) .+ Starting router update for (\S+), .+ update_id (\S+). .+'
+      expr: '([\d-]+) ([\d:]+\.\d{3}) .+ Starting router update for (\S+), .+ update_id (\S+). .+'
       hint: 'router update'
     end:
-      expr: '^([0-9-]+) (\S+) .+ Finished a router update for (\S+), update_id (\S+). .+'
+      expr: '([\d-]+) ([\d:]+\.\d{3}) .+ Finished a router update for (\S+), update_id (\S+). .+'
       hint: 'router update'
     # we want to analyse these with core.analytics.LogEventStats so don't treat as sequence.
     passthrough-results: True
   # identify HA router keepalived spawn events that took the longest to complete and report the longest updates.
   router-spawn-events:
     # router state_change_monitor + keepalived spawn
     # NOTE: there are no logs that depict a router create so we use the state change monitor spawn as a start point.
     start:
-      expr: '^([0-9-]+) (\S+) .+ Router (\S+) .+ spawn_state_change_monitor'
+      expr: '([\d-]+) ([\d:]+\.\d{3}) .+ Router (\S+) .+ spawn_state_change_monitor'
       hint: 'spawn_state_change'
     end:
-      expr: '^([0-9-]+) (\S+) .+ neutron.agent.linux.utils .+neutron-rootwrap.+''keepalived'',.+''/var/lib/neutron/ha_confs/([0-9a-z-]+)/keepalived.conf''.+ create_process'
+      expr: '([\d-]+) ([\d:]+\.\d{3}) .+ neutron.agent.linux.utils .+neutron-rootwrap.+''keepalived'',.+''/var/lib/neutron/ha_confs/([0-9a-z-]+)/keepalived.conf''.+ create_process'
       hint: 'Keepalived'
     # we want to analyse these with core.analytics.LogEventStats so don't treat as sequence.
     passthrough-results: True
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/events/openstack/nova/external-events.yaml` & `hotsos-1.15.post1/hotsos/defs/events/openstack/nova/external-events.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+# NOTE: for efficiency, do not capture time as subgroup unless actually necessary.
 input:
   path: 'var/log/nova/nova-compute.log'
   options:
     # Searching all logs can yield too many results and we don't yet have a
     # way to override MAX_LOGROTATE_DEPTH so disabling for now.
     disable-all-logs: True
 # Supported events - https://docs.openstack.org/api-ref/compute/?expanded=run-events-detail#create-external-events-os-server-external-events  # noqa E501
 events:
   network-changed:
-    expr: '.+\[instance: (\S+)\].+Received event (network-changed)-(\S+)\s+'
+    expr: '[\d-]+ [\d:]+\.\d{3} .+\[instance: (\S+)\].+Received event (network-changed)-(\S+)\s+'
   network-vif-plugged:
-    expr: '.+\[instance: (\S+)\].+Preparing to wait for external event (network-vif-plugged)-(\S+)\s+'
+    expr: '[\d-]+ [\d:]+\.\d{3} .+\[instance: (\S+)\].+Preparing to wait for external event (network-vif-plugged)-(\S+)\s+'
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml` & `hotsos-1.15.post1/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+# NOTE: for efficiency, do not capture time as subgroup unless actually necessary.
 ovsdb-server-sb:
   input:
     path: 'var/log/ovn/ovsdb-server-sb.log'
   hint: '(ERR|WARN|EMER)'
-  expr: '([0-9-]+)T[0-9:\.]+Z.+\|(ERR|ERROR|WARN|EMER)\|.+'
+  expr: '([\d-]+)T[\d:]+\.\d+Z.+\|(ERR|ERROR|WARN|EMER)\|.+'
 ovsdb-server-nb:
   input:
     path: 'var/log/ovn/ovsdb-server-nb.log'
   hint: '(ERR|WARN|EMER)'
-  expr: '([0-9-]+)T[0-9:\.]+Z.+\|(ERR|ERROR|WARN|EMER)\|.+'
+  expr: '([\d-]+)T[\d:]+\.\d+Z.+\|(ERR|ERROR|WARN|EMER)\|.+'
 ovn-northd:
   input:
     path: 'var/log/ovn/ovn-northd.log'
   hint: '(ERR|WARN|EMER)'
-  expr: '([0-9-]+)T[0-9:\.]+Z.+\|(ERR|ERROR|WARN|EMER)\|.+'
+  expr: '([\d-]+)T[\d:]+\.\d+Z.+\|(ERR|ERROR|WARN|EMER)\|.+'
 ovn-controller:
   input:
     path: 'var/log/ovn/ovn-controller.log'
   hint: '(ERR|WARN|EMER)'
-  expr: '([0-9-]+)T[0-9:\.]+Z.+\|(ERR|ERROR|WARN|EMER)\|.+'
+  expr: '([\d-]+)T[\d:]+\.\d+Z.+\|(ERR|ERROR|WARN|EMER)\|.+'
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml` & `hotsos-1.15.post1/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,32 @@
+# NOTE: for efficiency, do not capture time as subgroup unless actually necessary.
 ovsdb-server-sb:
   input:
     path: 'var/log/ovn/ovsdb-server-sb.log'
   inactivity-probe:
-    expr: '([0-9-]+)T[0-9:\.]+Z.+\|reconnect\|ERR\|ssl:(\S+):\d+: no response to inactivity probe'
+    expr: '([\d-]+)T[\d:]+\.\d+Z.+\|reconnect\|ERR\|ssl:(\S+):\d+: no response to inactivity probe'
   unreasonably-long-poll-interval:
-    expr: '([0-9-]+)T[0-9:\.]+Z.+\|timeval(?:\([a-zA-Z]+\d+\))?\|WARN\|Unreasonably long \d+ms poll interval'
+    expr: '([\d-]+)T[\d:]+\.\d+Z.+\|timeval(?:\([a-zA-Z]+\d+\))?\|WARN\|Unreasonably long \d+ms poll interval'
   leadership-transfers:
     expr:
-      - '([0-9-]+)T[0-9:\.]+Z.+\|raft\|INFO\|received leadership transfer from '
-      - '([0-9-]+)T[0-9:\.]+Z.+\|raft\|INFO\|Transferring leadership to write a snapshot.'
+      - '([\d-]+)T[\d:]+\.\d+Z.+\|raft\|INFO\|received leadership transfer from '
+      - '([\d-]+)T[\d:]+\.\d+Z.+\|raft\|INFO\|Transferring leadership to write a snapshot.'
   compactions:
-    expr: '([0-9-]+)T[0-9:\.]+Z.+\|ovsdb\|INFO\|OVN_Southbound: Database compaction'
+    expr: '([\d-]+)T[\d:]+\.\d+Z.+\|ovsdb\|INFO\|OVN_Southbound: Database compaction'
 ovsdb-server-nb:
   input:
     path: 'var/log/ovn/ovsdb-server-nb.log'
   inactivity-probe:
-    expr: '([0-9-]+)T[0-9:\.]+Z.+\|reconnect\|ERR\|ssl:(\S+):\d+: no response to inactivity probe'
+    expr: '([\d-]+)T[\d:]+\.\d+Z.+\|reconnect\|ERR\|ssl:(\S+):\d+: no response to inactivity probe'
   unreasonably-long-poll-interval:
-    expr: '([0-9-]+)T[0-9:\.]+Z.+\|timeval(?:\([a-zA-Z]+\d+\))?\|WARN\|Unreasonably long \d+ms poll interval'
+    expr: '([\d-]+)T[\d:]+\.\d+Z.+\|timeval(?:\([a-zA-Z]+\d+\))?\|WARN\|Unreasonably long \d+ms poll interval'
   leadership-transfers:
     expr:
-      - '([0-9-]+)T[0-9:\.]+Z.+\|raft\|INFO\|received leadership transfer from '
-      - '([0-9-]+)T[0-9:\.]+Z.+\|raft\|INFO\|Transferring leadership to write a snapshot.'
+      - '([\d-]+)T[\d:]+\.\d+Z.+\|raft\|INFO\|received leadership transfer from '
+      - '([\d-]+)T[\d:]+\.\d+Z.+\|raft\|INFO\|Transferring leadership to write a snapshot.'
   compactions:
-    expr: '([0-9-]+)T[0-9:\.]+Z.+\|ovsdb\|INFO\|OVN_Northbound: Database compaction'
+    expr: '([\d-]+)T[\d:]+\.\d+Z.+\|ovsdb\|INFO\|OVN_Northbound: Database compaction'
 northd:
   input:
     path: 'var/log/ovn/ovn-northd.log'
   inactivity-probe:
-    expr: '([0-9-]+)T[0-9:\.]+Z.+\|reconnect\|ERR\|ssl:(\S+):\d+: no response to inactivity probe'
+    expr: '([\d-]+)T[\d:]+\.\d+Z.+\|reconnect\|ERR\|ssl:(\S+):\d+: no response to inactivity probe'
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 checks:
   has_lp1852502:
     input:
       command: journalctl
       options:
         kwargs:
           unit: juju-db
-    expr: '.* CappedPositionLost: CollectionScan died due to position in capped collection being deleted'
+    expr: '(\S+) .+ CappedPositionLost: CollectionScan died due to position in capped collection being deleted'
 conclusions:
   lp1852502:
     decision: has_lp1852502
     raises:
       type: LaunchpadBug
       bug-id: 1852502
       message: >-
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 checks:
   has_unknown_relation_errors:
     input:
       path: 'var/log/juju/unit-*.log'
-    expr: '(\S+) (\S+) ERROR juju.worker.uniter agent.go:\d+ resolver loop error: unknown relation: \d+'
+    expr: '([\d-]+) ([\d:]+) ERROR juju.worker.uniter agent.go:\d+ resolver loop error: unknown relation: (\d+)'
     constraints:
       # within 7 days
       search-result-age-hours: 168
 conclusions:
   lp1895040:
     decision: has_unknown_relation_errors
     raises:
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 checks:
   has_lp1910958:
     input:
       path: 'var/log/juju/unit-*.log'
-    expr: '.* manifold worker .+ error: failed to initialize uniter for "(\S+)": cannot create relation state tracker: cannot remove persisted state, relation (\d+) has members'
+    expr: '[\d-]+ [\d:]+ ERROR juju.worker.dependency engine.go:\d+ "uniter" manifold worker .+ error: failed to initialize uniter for "(\S+)": cannot create relation state tracker: cannot remove persisted state, relation (\d+) has members'
     hint: 'manifold worker returned unexpected error'
 conclusions:
   lp1910958:
     decision: has_lp1910958
     raises:
       type: LaunchpadBug
       bug-id: 1910958
       message: >-
-        Unit {} failed to start due to members in relation {} that cannot be
+        Unit {unit} failed to start due to members in relation {rel} that cannot be
         removed.
-      search-result-format-groups: [1, 2]
+      format-dict:
+        unit: '@checks.has_lp1910958.search.results_group_1:unique_comma_join'
+        rel: '@checks.has_lp1910958.search.results_group_2:unique_comma_join'
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 checks:
   has_lp1996230:
     input:
       path: 'var/log/juju/machine-*.log'
-    expr: '.* manifold worker .+ error: could not retrieve action (\S+): action no longer available'
-    hint: 'manifold worker returned unexpected error'
+    expr: '[\d-]+ [\d:]+ ERROR juju.worker.dependency engine.go:\d+ "\S+" manifold worker .+ error: could not retrieve action (\S+): action no longer available'
 conclusions:
   lp1996230:
     decision: has_lp1996230
     raises:
       type: LaunchpadBug
       bug-id: 1996230
       message: >-
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/juju/charm_unit_checks.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/juju/charm_unit_checks.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 input:
   # default path that can be overriden
   path: 'var/log/juju/unit-*.log'
 checks:
   units_have_leadership_errors:
     search:
-      expr: '^(\S+) (\S+) .+ERROR cannot write leadership settings: cannot write settings: failed to merge leadership settings: application "(\S+)"'
+      expr: '(\S+) (\S+) .+ERROR cannot write leadership settings: cannot write settings: failed to merge leadership settings: application "(\S+)"'
       constraints:
         search-result-age-hours: 168  # 7 days
   units_have_tracebacks:
     search:
       expr:
         - Traceback \('
-        - '^(\S+) (\S+) (?:ERROR|WARNING) unit\.([^\.]+)\.\S+ .+ Traceback \('
+        - '(\S+) (\S+) (?:ERROR|WARNING) unit\.([^\.]+)\.\S+ .+ Traceback \('
       constraints:
         search-result-age-hours: 48
 conclusions:
   units-have-leadership-errors:
     decision: units_have_leadership_errors
     raises:
       type: JujuWarning
       message: >-
         Juju unit(s) '{units}' are showing leadership errors in their logs from
         the last 7 days. Please investigate.
       format-dict:
-        units: '@checks.units_have_leadership_errors.search.results_group_2:comma_join'
+        units: '@checks.units_have_leadership_errors.search.results_group_3:unique_comma_join'
   units-have-tracebacks:
     decision: units_have_tracebacks
     raises:
       type: JujuWarning
       message: >-
         Juju logs for unit(s) '{units}' contain {num_tracebacks} Traceback(s) from
         the last 48 hours - please check.
       format-dict:
-        units: '@checks.units_have_tracebacks.search.results_group_2:comma_join'
-        num_tracebacks: '@checks.units_have_tracebacks.search.results_group_2:len'
+        units: '@checks.units_have_tracebacks.search.results_group_3:unique_comma_join'
+        num_tracebacks: '@checks.units_have_tracebacks.search.num_results'
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/memory.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/kernel/memory.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -33,12 +33,12 @@
       - low_free_high_order_mem_blocks
       - high_compaction_failures
     raises:
       type: MemoryWarning
       message: >-
         Memory compaction failures are at {pcent}% of successes. This can suggest that
         there are insufficient high-order memory blocks available and the kernel is
-        unable form larger blocks on request which can slow things down. See vmstat
+        unable to form larger blocks on request which can slow things down. See vmstat
         output for more detail.
       format-dict:
         pcent: $compaction_failures_percent
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/network/misc.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/kernel/network/misc.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/network/tcp.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/kernel/network/tcp.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/network/udp.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/kernel/network/udp.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/kernel/qla2xxx.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/kernel/qla2xxx.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -5,11 +5,12 @@
     expr: '.+ qla2xxx (\S+): skipping scsi_scan_host\(\) for non-initiator port'
 conclusions:
   qla2xxx_skipped_scsi_scan_host:
     decision: qla2xxx_skipping_scsi_scan_host
     raises:
       type: KernelWarning
       message: >-
-        The qla2xxx driver did not perform SCSI scan on host/port {}.
+        The qla2xxx driver did not perform SCSI scan on host/port {port}.
         Some SCSI disks/paths might not be present. (Module option
         'qla2xxx.qlini_mode')
-      search-result-format-groups: [1]
+      format-dict:
+        port: '@checks.qla2xxx_skipping_scsi_scan_host.search.results_group_1:first'
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/mysql/mysql_connections.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/mysql/mysql_connections.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/eol.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 checks:
   has_1960319_log:
     input: var/log/neutron/neutron-server.log
-    expr: '(\S+\s+[\d:]+).\S+ .+ ovsdbapp.event FileNotFoundError: \[Errno 2\] No such file or directory: ''ovsdb-client'''
+    expr: '([\d-]+) ([\d:]+)\.\d{3} .+ ovsdbapp.event FileNotFoundError: \[Errno 2\] No such file or directory: ''ovsdb-client'''
     constraints:
       search-result-age-hours: 168  # 7 days
   has_1960319_package:
     apt: openvswitch-common
 conclusions:
   lp_1960319:
     decision:
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 checks:
   has_1979089:
     input:
       path: 'var/log/neutron/neutron-l3-agent.log'
     search:
-      expr: '(\S+\s+[\d:]+).\S+ .+ Cannot open network namespace "qrouter-\S+": No such file or directory'
+      expr: '([\d-]+) ([\d:]+)\.\d{3} .+ Cannot open network namespace "qrouter-\S+": No such file or directory'
       hint: 'ERROR neutron.agent.linux.utils'
       constraints:
         # if we hit this bug there will be a large number in a small space of time
         min-results: 10
         search-period-hours: 1
         search-result-age-hours: 48
 conclusions:
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,21 @@
   is_neutron_ovn_metadata_agent:
     apt: neutron-ovn-metadata-agent
   has_1829109_neutron_log:
     input:
       - var/log/neutron/neutron-server.log
       - var/log/neutron/neutron-ovn-metadata-agent.log
     # note: neutron-server and neutron-ovn-metadata-agent use different ports to speak to the southbound db (16642/6642)
-    expr: '(\S+\s+[\d:]+).\S+ .+ ovsdbapp.backend.ovs_idl.vlog \[-\] ssl:\S+:1?6642: clustered database server has stale data; trying another server'
+    expr: '([\d-]+) ([\d:]+)\.\d{3} .+ ovsdbapp.backend.ovs_idl.vlog \[-\] ssl:\S+:1?6642: clustered database server has stale data; trying another server'
     constraints:
       min-results: 10
       search-result-age-hours: 6
   has_1829109_ovn_controller_log:
     input: var/log/ovn/ovn-controller.log
-    expr: '([0-9-]+)T([0-9:\.]+)Z.+\|ovsdb_idl\|WARN\|tcp:\S+:6642: clustered database server has stale data; trying another server'
+    expr: '([\d-]+)T([\d:]+)\.\d+Z.+\|ovsdb_idl\|WARN\|tcp:\S+:6642: clustered database server has stale data; trying another server'
     constraints:
       min-results: 10
       search-result-age-hours: 6
 conclusions:
   has_1960319_neutron_server:
     decision:
       - is_neutron_server
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 checks:
   has_1860743:
     input:
       path: 'var/log/nova/nova-compute.log'
-    expr: '.+Live Migration failure: operation failed: Failed to connect to remote libvirt URI .+Cannot recv data: Host key verification failed\.: Connection reset by peer: libvirtError: operation failed: Failed to connect to remote libvirt URI.+Cannot recv data: Host key verification failed\.: Connection reset by peer'
+    expr: '([\d-]+) [\d:]+\.\d{3} .+Live Migration failure: operation failed: Failed to connect to remote libvirt URI .+Cannot recv data: Host key verification failed\.: Connection reset by peer: libvirtError: operation failed: Failed to connect to remote libvirt URI.+Cannot recv data: Host key verification failed\.: Connection reset by peer'
     hint: 'libvirtError'
 conclusions:
   lp1860743:
     decision: has_1860743
     raises:
       type: LaunchpadBug
       bug-id: 1860743
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 checks:
   has_1888395_pt1:
     input:
       path: 'var/log/nova/nova-compute.log'
-    expr: '.+NotImplementedError: Cannot load ''vifs'' in the base class'
+    expr: '([\d-]+) [\d:]+\.\d{3} .+NotImplementedError: Cannot load ''vifs'' in the base class'
     hint: 'NotImplementedError'
   has_1888395_pt2:
     apt:
       nova-common:
         # train
         - min: 2:20.0.0
           max: 2:20.6.0-0ubuntu0
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 checks:
   logs:
     input:
       path: 'var/log/nova/nova-compute.log'
     search:
-      expr: '^([\d-]+\s+[\d:]+)\S+ .+ libvirt.libvirtError: Cannot access storage file ''\S+'' \(as uid:\d+, gid:\d+\): Permission denied'
+      expr: '([\d-]+) ([\d:]+)\.\d{3} .+ libvirt.libvirtError: Cannot access storage file ''\S+'' \(as uid:\d+, gid:\d+\): Permission denied'
       hint: ERROR
       constraints:
         search-result-age-hours: 168  # 7 days
   pkg:
     apt:
       nova-common:
         # every version up to kinetic/zed initial release has the bug
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/nova/config_checks.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/nova/config_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
           max: 6.2.0-0ubuntu1~cloud0~1
         # victoria
         - min: 7.0.0
           max: 7.1.0-0ubuntu1~cloud0~1
   has_2008099_logs:
     input:
       path: 'var/log/octavia/octavia-worker.log'
-    expr: '.+octavia.amphorae.drivers.haproxy.exceptions .+ Removing incomplete section ''peers'
+    expr: '([\d-]+) [\d:]+\.\d{3} \d+ ERROR octavia.amphorae.drivers.haproxy.exceptions .+ Removing incomplete section ''peers'
     hint: octavia.amphorae.drivers.haproxy.exceptions
 conclusions:
   2008099:
     decision:
       - has_2008099_pkg_versions
       - has_2008099_logs
     raises:
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 input:
   command: ovs_appctl_dpctl_dump_conntrack
   options:
     kwargs:
       datapath: 'system@ovs-system'
 checks:
+  # NOTE: we don't extract any info from the following searches so they define the smallest group possible so as to minimise saved data.
   ovs_using_geneve:
     input:
       command: ovs_appctl_ofproto_list_tunnels
-    search: '.+ \(geneve:'
+    search: '.+ \((g)eneve:'
   ovs_using_vxlan:
     input:
       command: ovs_appctl_ofproto_list_tunnels
-    search: '.+ \(vxlan:'
+    search: '.+ \((v)xlan:'
   geneve_is_tracked:
-    search: '^udp,.+,sport=6081,'
+    search: '^(u)dp,.+,sport=6081,'
   vxlan_is_tracked:
-    search: '^udp,.+,sport=4789,'
+    search: '^(u)dp,.+,sport=4789,'
 conclusions:
   ovs_ct_tunnels:
     decision:
       or:
         - and:
            - ovs_using_geneve
            - geneve_is_tracked
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     lost packets is increasing and (b) check the ovs-vswitchd logs for more context
     and check the path between nic and ovs.
 checks:
   dp_has_lost_packets:
     varops: [[$num_lost_packets], [gt, 5]]  # allow a very small number
   dpif_netlink_lost_packet_on_handler:
     search:
-      expr: '([0-9-]+)T[0-9:\.]+Z.+\|system@ovs-system: lost packet on port channel.+'
+      expr: '([\d-]+)T([\d:]+)\.\d+Z.+\|system@ovs-system: lost packet on port channel.+'
       constraints:
         min-results: 10  # allow a very small number
         search-period-hours: 24
         search-result-age-hours: 168  # 7 days
 conclusions:
   has_lost_packets_cause_unknown:
     priority: 1
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # default input
 input:
   path: var/log/openvswitch/ovs-vswitchd.log
 checks:
   dpif_resubmit_limit_reached:
     search:
-      expr: '([0-9-]+)T[0-9:\.]+Z.+\|WARN\|over (\d+) resubmit actions on bridge (\S+) while processing'
+      expr: '([\d-]+)T([\d:]+)\.\d+Z.+\|WARN\|over (\d+) resubmit actions on bridge (\S+) while processing'
       constraints:
         min-results: 5
-        search-result-period: 24
+        search-period-hours: 24
         search-result-age-hours: 336  # 14 days
 conclusions:
   has_resubmit_limit_reached:
     decision: dpif_resubmit_limit_reached
     raises:
       type: OpenvSwitchWarning
       message: >-
         OpenvSwitch (vswitchd) is reporting flows hitting action resubmit
-        limit ({}) which suggests that packets are being silently
+        limit ({value}) which suggests that packets are being silently
         dropped. One cause of this is when you have too many flows and an
         example is when you have an excess of ovn logical flows. Look for
         "resubmit actions on bridge" in /var/log/openvswitch/ovs-vswitchd.log
         for more info and see what type of flow is resulting in this limit
         being hit.
-      search-result-format-groups: [2]
+      format-dict:
+        value: '@checks.dpif_resubmit_limit_reached.search.results_group_3:first'
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 checks:
   vswitchd_to_ovn_controller_inactivity_timeouts:
     input:
       path: var/log/openvswitch/ovs-vswitchd.log
     search:
-      expr: '([0-9-]+)T([0-9:\.]+)Z.+\|reconnect\|ERR\|ssl:(\S+):\d+: no response to inactivity probe'
+      expr: '([\d-]+)T([\d:]+)\.\d+Z.+\|reconnect\|ERR\|ssl:(\S+):\d+: no response to inactivity probe'
       constraints:
         # trigger if we at least this many in 1 hour period and look at last 24 hours only.
         min-results: 10
         search-period-hours: 1
         search-result-age-hours: 24
   bfd_state_changes:
     input:
       path: var/log/openvswitch/ovs-vswitchd.log
     search:
-      expr: '([0-9-]+)T([0-9:\.])+Z.+\|bfd\(\S+\)\|INFO\|[a-z0-9-]+: BFD state change'
+      expr: '([\d-]+)T([\d:]+)\.\d+Z.+\|bfd\(\S+\)\|INFO\|[a-z0-9-]+: BFD state change'
       constraints:
         # trigger if we at least this many in 1 hour period and look at last 24 hours only.
         min-results: 10
         search-period-hours: 1
         search-result-age-hours: 24
   chassis_gw_port_reassignments:
     input:
       path: var/log/ovn/ovn-controller.log
     search:
-      expr: '([0-9-]+)T([0-9:\.]+)Z.+\|binding\|INFO\|(Claiming|Releasing) lport cr-lrp-\S+ for this chassis.'
+      expr: '([\d-]+)T([\d:]+)\.\d+Z.+\|binding\|INFO\|(Claiming|Releasing) lport cr-lrp-\S+ for this chassis.'
       constraints:
         # trigger if we see at least this many in last 24 hours.
         min-results: 20
         search-result-age-hours: 24
 conclusions:
   chassis_gw_port_reassignments_no_bfd:
     priority: 1
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 checks:
-  has_1865127:
-    input:
-      path: 'var/log/ovn/ovn-controller.log'
-    expr: '.+ERR\|bridge not found for localnet port \S+ with network name'
-  1865127_broken_package:
+  1865127_logs:
+    input: 'var/log/ovn/ovn-controller.log'
+    search:
+      expr: '([\d-]+)T([\d:]+)\.\d+Z.+ERR\|bridge not found for localnet port \S+ with network name'
+      constraints:
+        search-result-age-hours: 24
+  1865127_apt_broken_package:
     apt:
       ovn-common:
         - min: 0
           max: 20.12.0~1
 conclusions:
   lp1865127:
     decision:
-      - has_1865127
-      - 1865127_broken_package
+      - 1865127_logs
+      - 1865127_apt_broken_package
     raises:
       type: LaunchpadBug
       bug-id: 1865127
       message: >-
         The version of ovn on this node is affected by a known bug where the
         ovn-controller logs are being spammed with error messages containing
         "No bridge for localnet port ..." when that is in fact not an error.
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 vars:
   host_cert_mtime: '@hotsos.core.host_helpers.filestat.FileFactory.mtime:etc/ovn/cert_host'
   ovn_central_cert_mtime: '@hotsos.core.host_helpers.filestat.FileFactory.mtime:etc/ovn/ovn-central.crt'
   northd_start_time: '@hotsos.core.host_helpers.systemd.ServiceFactory.start_time_secs:ovn-northd'
   ovsdb_nb_start_time: '@hotsos.core.host_helpers.systemd.ServiceFactory.start_time_secs:ovn-ovsdb-server-nb'
   ovsdb_sb_start_time: '@hotsos.core.host_helpers.systemd.ServiceFactory.start_time_secs:ovn-ovsdb-server-sb'
-  cert_expired_expr: '([0-9-]+)T[0-9:\.]+Z\|\S+\|stream_ssl\|WARN\|SSL_accept: error:\S+:SSL routines:ssl3_read_bytes:sslv3 alert certificate expired'
-  cert_invalid_expr: '([0-9-]+)T[0-9:\.]+Z\|\S+\|stream_ssl\|WARN\|SSL_accept: error:\S+:SSL routines:tls_process_client_certificate:certificate verify failed'
+  cert_expired_expr: '([\d-]+)T([\d:]+)\.\d+Z\|\S+\|stream_ssl\|WARN\|SSL_accept: error:\S+:SSL routines:ssl3_read_bytes:sslv3 alert certificate expired'
+  cert_invalid_expr: '([\d-]+)T([\d:]+)\.\d+Z\|\S+\|stream_ssl\|WARN\|SSL_accept: error:\S+:SSL routines:tls_process_client_certificate:certificate verify failed'
 checks:
   services_not_restarted_after_cert_update:
     - systemd: [ovn-northd, ovn-ovsdb-server-nb, ovn-ovsdb-server-sb]
     - or:
         - varops: [[$host_cert_mtime], [gt, $northd_start_time]]
         - varops: [[$host_cert_mtime], [gt, $ovsdb_nb_start_time]]
         - varops: [[$host_cert_mtime], [gt, $ovsdb_sb_start_time]]
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 vars:
   host_cert_mtime: '@hotsos.core.host_helpers.filestat.FileFactory.mtime:etc/ovn/cert_host'
   ovn_chassis_cert_mtime: '@hotsos.core.host_helpers.filestat.FileFactory.mtime:etc/ovn/ovn-chassis.crt'
   ovn_controller_start_time: '@hotsos.core.host_helpers.systemd.ServiceFactory.start_time_secs:ovn-controller'
-  cert_expired_expr: '([0-9-]+)T[0-9:\.]+Z\|\S+\|stream_ssl\|WARN\|SSL_accept: error:\S+:SSL routines:ssl3_read_bytes:sslv3 alert certificate expired'
-  cert_invalid_expr: '([0-9-]+)T[0-9:\.]+Z\|\S+\|stream_ssl\|WARN\|SSL_accept: error:\S+:SSL routines:tls_process_client_certificate:certificate verify failed'
+  cert_expired_expr: '([\d-]+)T([\d:]+)\.\d+Z\|\S+\|stream_ssl\|WARN\|SSL_accept: error:\S+:SSL routines:ssl3_read_bytes:sslv3 alert certificate expired'
+  cert_invalid_expr: '([\d-]+)T([\d:]+)\.\d+Z\|\S+\|stream_ssl\|WARN\|SSL_accept: error:\S+:SSL routines:tls_process_client_certificate:certificate verify failed'
 checks:
   services_not_restarted_after_cert_update:
     - systemd: ovn-controller
     - varops: [[$host_cert_mtime], [gt, $ovn_controller_start_time]]
     - varops: [[$ovn_chassis_cert_mtime], [gt, $ovn_controller_start_time]]
   certs_expired_logs:
     input: var/log/ovn/ovn-controller.log
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   ovn_controller_not_fixed:
     apt:
       ovn-host:
         - min: 0
           max: 20.03.2-0ubuntu0.20.04.3
   has_northd_version_mismatch:
     input: var/log/ovn/ovn-controller.log
-    expr: '([0-9-]+)T[0-9:\.]+Z\|\S+\|main\|WARN\|controller version - (\S+) mismatch with northd version - (\S+)'
+    expr: '([\d-]+)T([\d:]+)\.\d+Z\|\S+\|main\|WARN\|controller version - (\S+) mismatch with northd version - (\S+)'
     constraints:
-      search-results-age-hours: 336  # 14 days
+      search-result-age-hours: 336  # 14 days
 conclusions:
   has_northd_version_mismatch:
     decision:
       - is_ovn_controller
       - ovn_controller_not_fixed
       - has_northd_version_mismatch
     raises:
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 checks:
   sb_ovn_elections:
     input:
-      path:
-        - var/log/ovn/ovsdb-server-sb.log
+      path: var/log/ovn/ovsdb-server-sb.log
     search:
-      expr: '([0-9-]+)T([0-9:\.]+)Z.+\|raft\|INFO\|term ([0-9]+):\s(([0-9]+) ms timeout expired, )?starting election$'
+      expr: '([\d-]+)T([\d:]+)\.\d+Z.+\|raft\|INFO\|term ([0-9]+):\s(([0-9]+) ms timeout expired, )?starting election$'
       constraints:
         min-results: 5
         search-period-hours: 1
         search-result-age-hours: 48
   nb_ovn_elections:
     input:
-      path:
-        - var/log/ovn/ovsdb-server-nb.log
+      path: var/log/ovn/ovsdb-server-nb.log
     search:
-      expr: '([0-9-]+)T([0-9:\.]+)Z.+\|raft\|INFO\|term ([0-9]+):\s(([0-9]+) ms timeout expired, )?starting election$'
+      expr: '([\d-]+)T([\d:]+)\.\d+Z.+\|raft\|INFO\|term ([0-9]+):\s(([0-9]+) ms timeout expired, )?starting election$'
       constraints:
         min-results: 5
         search-period-hours: 1
         search-result-age-hours: 48
 conclusions:
   ovn_frequent_elections_sb:
     priority: 1
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 checks:
   has_ovsdb_reconnection_errors:
     input:
       - var/log/neutron/neutron-server.log
       - var/log/neutron/neutron-ovn-metadata-agent.log
-    expr: '.+ ovsdbapp.backend.ovs_idl.connection ValueError: non-zero flags not allowed in calls to send\(\) on <class ''eventlet.green.ssl.GreenSSLSocket''>'
+    expr: '([\d-]+) [\d:]+\.\d{3} .+ ovsdbapp.backend.ovs_idl.connection ValueError: non-zero flags not allowed in calls to send\(\) on <class ''eventlet.green.ssl.GreenSSLSocket''>'
     hint: ERROR
   has_pyovs_with_reconnection_bug:
     apt:
       python3-openvswitch:
         - min: 2.17.0
           max: 2.17.1
 conclusions:
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 input:
   path: 'var/log/rabbitmq/rabbit@*.log'
 checks:
   cluster_partitions:
     expr: '.+ \S+_partitioned_network'
     hint: 'partition'
   no_sync:
-    expr: 'Mirrored queue ''.+'' in vhost ''.+'': Stopping'
+    expr: '.+ Mirrored queue ''.+'' in vhost ''.+'': Stopping'
     hint: 'synchronised'
   discard:
-    expr: 'Discarding message.+old incarnation'
+    expr: '.+ Discarding message.+old incarnation'
     hint: 'Discarding'
 conclusions:
   cluster-has-had-partions:
     decision: cluster_partitions
     raises:
       type: RabbitMQWarning
       message: >-
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/bcache/bdev.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/bcache/bdev.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/bcache/cacheset.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/bcache/cacheset.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,14 @@
   db_too_large:
     decision:
       - mon_large_db
       - health_warning
     raises:
       type: CephMonWarning
       message: >-
-        Ceph is reporting that for mon {}, the leveldb database used to
+        Ceph is reporting that for mon {mon_id}, the leveldb database used to
         store cluster metadata is using a lot of disk space which may
         cause slow queries and delayed response to clients.
         Recommendation is to run compaction on the mon db. Please see
         docs.ceph.com/en/quincy/rados/operations/health-checks/#mon-disk-big
-      search-result-format-groups: [1]
-
+      format-dict:
+        mon_id: '@checks.mon_large_db.search.results_group_1:first'
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 checks:
   ceph_log_has_election_calls:
     input:
       path: var/log/ceph/ceph*.log
     search:
-      expr: '^([0-9-]+)\S* (\S+) .+ mon.\S+ calling monitor election'
+      expr: '^([\d-]+)[T ]([\d:]+)\S+ (\S+) .+ mon.\S+ calling monitor election'
       constraints:
         # i.e. must occur 5 times within same 24 hour period
         min-results: 5
         search-period-hours: 24
         search-result-age-hours: 48
         min-hours-since-last-boot: 1
   ceph_interfaces_have_errors:
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 checks:
   # NOTE: the following check can be run on a mon or osd node since the same
   # logs should be available on both.
   osd_flapping:
     input:
       path: var/log/ceph/ceph*.log
-    expr: '^([\d-]+)[T ]([\d:]+\.\d)\S+ .+ wrongly marked me down at .+'
+    expr: '([\d-])+[T ][\d:]+\S+ .+ wrongly marked me down at .+'
   ceph_interfaces_have_errors:
     property: hotsos.core.plugins.storage.ceph.CephChecksBase.has_interface_errors
 conclusions:
   cause-unknown:
     priority: 1
     decision: osd_flapping
     raises:
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 checks:
   osd_slow_heartbeats:
     input:
       path: var/log/ceph/ceph*.log
     search:
-      expr: '^([\d-]+)T([\d:]+\.\d)\S+ .+ Slow OSD heartbeats on .+'
+      expr: '^([\d-]+)[T ]([\d:]+)\S+ .+ Slow OSD heartbeats on .+'
       constraints:
         # i.e. must occur 10 times within an hour
         min-results: 10
         search-period-hours: 1
 conclusions:
   osd-slow-heartbeats:
     decision: osd_slow_heartbeats
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 checks:
   # NOTE: the following check can be run on a mon or osd node since the same
   # logs should be available on both.
   osd_slow_ops:
     input:
       path: var/log/ceph/ceph*.log
     search:
-      expr: '^([\d-]+)[T ]([\d:]+\.\d)\S+ .+ slow ops, oldest one blocked .+'
+      expr: '^([\d-]+)[T ]([\d:]+)\S+ .+ slow ops, oldest one blocked .+'
       constraints:
         # i.e. must occur 5 times within same 24 hour period
         min-results: 5
         search-period-hours: 1
         search-result-age-hours: 24
   ceph_interfaces_have_errors:
     property: hotsos.core.plugins.storage.ceph.CephChecksBase.has_interface_errors
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 vars:
   bluestore_volume_selection_policy: '@hotsos.core.plugins.storage.ceph.CephDaemonAllOSDsFactory.bluestore_volume_selection_policy:CephDaemonConfigShow'
   bluestore_cache_onode: '@hotsos.core.plugins.storage.ceph.CephDaemonAllOSDsFactory.bluestore_cache_onode:CephDaemonDumpMemPools'
 checks:
   has_1996010_osd_log:
     # NOTE: this needs quite a high debug level to appear - debug_bluestore=30/30
     input: var/log/ceph/ceph-osd.*.log
-    expr: '^([\d-]+)[T ]([\d:]+\.\d)\S+ .+ bluestore\.MempoolThread\(\S+\) _resize_shards max_shard_onodes: 0 '
+    expr: '([\d-]+)[T ][\d:]+\S+ .+ bluestore\.MempoolThread\(\S+\) _resize_shards max_shard_onodes: 0 '
   has_1996010_mempools:
     # this is a hack to check if a value less than 10 exists in the list
     or:
       - varops: [[$bluestore_cache_onode], [contains, 0]]
       - varops: [[$bluestore_cache_onode], [contains, 1]]
       - varops: [[$bluestore_cache_onode], [contains, 2]]
       - varops: [[$bluestore_cache_onode], [contains, 3]]
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 checks:
   # NOTE: the following check can be run on a mon or osd node since the same
   # logs should be available on both.
   osd_flapping:
     input:
       path: var/log/ceph/ceph*.log
-    expr: '^([\d-]+)[T ]([\d:]+\.\d)\S+ .+ wrongly marked me down at .+'
+    expr: '([\d-])+[T ][\d:]+\S+ .+ wrongly marked me down at .+'
   ceph_interfaces_have_errors:
     property: hotsos.core.plugins.storage.ceph.CephChecksBase.has_interface_errors
 conclusions:
   cause-unknown:
     priority: 1
     decision: osd_flapping
     raises:
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 checks:
   osd_disk_latency:
     input:
       path: var/log/ceph/ceph*.log
     search:
-      expr: '^([\d-]+)[T ]([\d:]+\.\d)\S+ .+ slow operation observed .+'
+      expr: '^([\d-]+)[T ]([\d:]+)\S+ .+ slow operation observed .+'
       constraints:
         # Expect several in a row; anything that's temporary wouldn't result in
         # slow ops and likely to be a result of momentary extreme load.
         min-results: 5
         search-period-hours: 1
         search-result-age-hours: 168  # 7 days
 conclusions:
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 checks:
   # NOTE: the following check can be run on a mon or osd node since the same
   # logs should be available on both.
   osd_slow_ops:
     input:
       path: var/log/ceph/ceph*.log
     search:
-      expr: '^([\d-]+)[T ]([\d:]+\.\d)\S+ .+ slow ops, oldest one blocked .+'
+      expr: '^([\d-]+)[T ]([\d:]+)\S+ .+ slow ops, oldest one blocked .+'
       constraints:
         # i.e. must occur 5 times within same 24 hour period
         min-results: 5
         search-period-hours: 1
         search-result-age-hours: 24
   ceph_interfaces_have_errors:
     property: hotsos.core.plugins.storage.ceph.CephChecksBase.has_interface_errors
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -3,23 +3,26 @@
     property:
       path: hotsos.core.plugins.storage.ceph.CephCluster.health_status
       ops: [[ne, HEALTH_OK]]
   ceph_osd_withhold_creation:
     input:
       path: [var/log/ceph/ceph-osd*.log, var/log/ceph/ceph.log]
     search:
-      expr: '.+ (osd.+) .+ maybe_wait_for_max_pg withhold creation of pg .+: (.+) >= (.+)'
+      expr: '[\d-]+[T ][\d:]+\S+ .+ (osd.+) .+ maybe_wait_for_max_pg withhold creation of pg .+: (.+) >= (.+)'
 conclusions:
   pending_creating_pgs:
     decision:
       - health_warning
       - ceph_osd_withhold_creation
     raises:
       type: CephOSDWarning
       message: >-
-        ceph is trying to create {} PGs on {} but the hard limit is {}.
+        ceph is trying to create {num_pgs} PGs on {osd} but the hard limit is {limit}.
         The mon_max_pg_per_osd or osd_max_pg_per_osd_hard_ratio may be
         increased as a workaround. Please see
         www.ceph.com/community/new-luminous-pg-overdose-protection
         Note if the pending PGs are more than double the hard limit,
         it needs further investigation before applying the workaround.
-      search-result-format-groups: [2,1,3]
+      format-dict:
+        osd: '@checks.ceph_osd_withhold_creation.search.results_group_1:first'
+        num_pgs: '@checks.ceph_osd_withhold_creation.search.results_group_2:first'
+        limit: '@checks.ceph_osd_withhold_creation.search.results_group_3:first'
```

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml` & `hotsos-1.15.post1/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/juju/summary.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/juju/summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+from datetime import datetime, timedelta
 import os
 import re
 
-from datetime import datetime, timedelta
-
 from hotsos.core.log import log
 from hotsos.core.host_helpers import CLIHelper
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.plugins.juju.common import (
     JujuChecksBase,
     JujuTimestampMatcher,
 )
```

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/kernel/summary.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/kernel/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/kubernetes/summary.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/kubernetes/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/lxd/summary.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/lxd/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/agent/events.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/openstack/agent/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import datetime
-import yaml
 
 from hotsos.core.plugintools import summary_entry_offset as idx
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.analytics import LogEventStats, SearchResultIndices
 from hotsos.core.host_helpers import CLIHelper
 from hotsos.core.ycheck.events import CallbackHelper
 from hotsos.core.issues import (
@@ -21,14 +20,15 @@
 from hotsos.core.plugins.openstack.common import (
     OpenstackChecksBase,
     OpenstackEventChecksBase,
 )
 from hotsos.core.plugins.openstack.openstack import OpenstackTimestampMatcher
 from hotsos.core.plugins.openstack.neutron import NeutronHAInfo
 from hotsos.core.utils import sorted_dict
+import yaml
 
 EVENTCALLBACKS = CallbackHelper()
 VRRP_TRANSITION_WARN_THRESHOLD = 8
 
 
 class ApacheEventChecks(OpenstackEventChecksBase):
 
@@ -91,16 +91,15 @@
         super().__init__(EVENTCALLBACKS, *args,
                          yaml_defs_group='http-requests', **kwargs)
 
     @EVENTCALLBACKS.callback(event_group='http-requests',
                              event_names=['neutron'])
     def http_requests(self, event):
         results = [{'date': r.get(1),
-                    'time': r.get(2),
-                    'key': r.get(3)} for r in event.results]
+                    'key': r.get(2)} for r in event.results]
         ret = self.categorise_events(event, results=results)
         if ret:
             return ret
 
     def __summary_http_requests(self):
         out = self.final_event_results
         if out:
@@ -164,20 +163,20 @@
 
     @EVENTCALLBACKS.callback(event_group='octavia',
                              event_names=['lb-failover-auto',
                                           'lb-failover-manual'])
     def lb_failovers(self, event):
         results = []
         for e in event.results:
-            payload = yaml.safe_load(e.get(2))
+            payload = yaml.safe_load(e.get(3))
             lb_id = payload.get('load_balancer_id')
             if lb_id is None:
                 continue
 
-            results.append({'date': e.get(1), 'key': lb_id})
+            results.append({'date': e.get(1), 'time': e.get(2), 'key': lb_id})
 
         ret = self.categorise_events(event, results=results, key_by_date=False)
         if ret:
             failover_type = event.name.rpartition('-')[2]
             return {failover_type: ret}, 'lb-failovers'
 
     @EVENTCALLBACKS.callback(event_group='octavia')
@@ -278,20 +277,21 @@
 
         return args, kwargs
 
     @EVENTCALLBACKS.callback(event_group='neutron.ml2-routers')
     def vrrp_transitions(self, event):
         results = []
         for r in event.results:
-            router = self.ha_info.find_router_with_vr_id(r.get(2))
+            router = self.ha_info.find_router_with_vr_id(r.get(3))
             if not router:
-                log.debug("could not find router with vr_id %s", r.get(2))
+                log.debug("could not find router with vr_id %s", r.get(3))
                 continue
 
-            results.append({'date': r.get(1), 'key': router.uuid})
+            results.append({'date': r.get(1), 'time': r.get(2),
+                            'key': router.uuid})
 
         transitions = self.categorise_events(event, results=results,
                                              key_by_date=False)
         if transitions:
             # run checks
             self.check_vrrp_transitions(transitions)
             # add info to summary
```

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/agent/exceptions.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/openstack/agent/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+from collections import UserDict
 import os
 import re
 
-from collections import UserDict
-
 from hotsos.core.log import log
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.plugins.openstack.common import OpenstackChecksBase
 from hotsos.core.plugins.openstack.openstack import OpenstackTimestampMatcher
 from hotsos.core.search import (
     FileSearcher,
     SearchDef,
```

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/nova_external_events.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/openstack/nova_external_events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/service_features.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/openstack/service_features.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/service_network_checks.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/openstack/service_network_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/summary.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/openstack/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/openstack/vm_info.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/openstack/vm_info.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,147 +1,43 @@
-import os
-import re
-
 from datetime import datetime
 
-from hotsos.core.config import HotSOSConfig
 from hotsos.core.ycheck.events import CallbackHelper
 from hotsos.core.analytics import LogEventStats
+from hotsos.core.plugins.openstack.openstack import (
+    OpenstackTimestampMatcher,
+)
 from hotsos.core.search import (
     FileSearcher,
-    SearchDef,
-    SequenceSearchDef,
     SearchConstraintSearchSince,
 )
-from hotsos.core.plugins.openstack.openstack import (
-    OpenstackConfig,
-    OpenstackTimestampMatcher,
-)
 from hotsos.core.plugins.openstack.common import (
     OpenstackChecksBase,
     OpenstackEventChecksBase,
 )
-from hotsos.core.plugins.system.system import SystemBase
-from hotsos.core.plugins.kernel.sysfs import CPU
+from hotsos.core.plugins.openstack.nova import NovaLibvirt
 from hotsos.core import utils
 
 EVENTCALLBACKS = CallbackHelper()
 
 
 class OpenstackInstanceChecks(OpenstackChecksBase):
 
-    def _get_cpu_models(self, etc_libvirt_qemu):
-        """ Get CPU models used by instances. """
-        cpu_models = {}
-        if not self.nova.instances:
-            return cpu_models
-
-        guests = []
-        seqs = {}
-        s = FileSearcher()
-        for i in self.nova.instances.values():
-            guests.append(i.name)
-            start = SearchDef(r"\s+<cpu .+>")
-            body = SearchDef(r".+")
-            end = SearchDef(r"\s+</cpu>")
-            tag = "{}.cpu".format(i.name)
-            seqs[i.name] = SequenceSearchDef(start=start, body=body,
-                                             end=end, tag=tag)
-            path = os.path.join(etc_libvirt_qemu, "{}.xml".format(i.name))
-            s.add(seqs[i.name], path)
-
-        results = s.run()
-        for guest in guests:
-            sections = results.find_sequence_sections(seqs[guest]).values()
-            for section in sections:
-                for r in section:
-                    if 'body' in r.tag:
-                        if '<model' in r.get(0):
-                            ret = re.search(r'.+>(\S+)<.+', r.get(0))
-                            if ret:
-                                model = ret.group(1)
-                                if model in cpu_models:
-                                    cpu_models[model] += 1
-                                else:
-                                    cpu_models[model] = 1
-
-        return cpu_models
-
-    def _get_vcpu_info(self, etc_libvirt_qemu):
-        vcpu_info = {}
-        if not self.nova.instances:
-            return vcpu_info
-
-        guests = []
-        s = FileSearcher()
-        for i in self.nova.instances.values():
-            guests.append(i.name)
-            tag = "{}.vcpus".format(i.name)
-            path = os.path.join(etc_libvirt_qemu, "{}.xml".format(i.name))
-            s.add(SearchDef(".+vcpus>([0-9]+)<.+", tag=tag), path)
-
-        total_vcpus = 0
-        results = s.run()
-        for guest in guests:
-            for r in results.find_by_tag("{}.vcpus".format(guest)):
-                vcpus = r.get(1)
-                total_vcpus += int(vcpus)
-
-        vcpu_info["used"] = total_vcpus
-
-        sysinfo = SystemBase()
-        if sysinfo.num_cpus is None:
-            return vcpu_info
-
-        total_cores = sysinfo.num_cpus
-        vcpu_info["system-cores"] = total_cores
-
-        nova_config = OpenstackConfig(os.path.join(HotSOSConfig.data_root,
-                                                   "etc/nova/nova.conf"))
-        pinset = nova_config.get("vcpu_pin_set",
-                                 expand_to_list=True) or []
-        pinset += nova_config.get("cpu_dedicated_set",
-                                  expand_to_list=True) or []
-        pinset += nova_config.get("cpu_shared_set",
-                                  expand_to_list=True) or []
-        if pinset:
-            # if pinning is used, reduce total num of cores available
-            # to those included in nova cpu sets.
-            available_cores = len(set(pinset))
-        else:
-            available_cores = total_cores
-
-        vcpu_info["available-cores"] = available_cores
-
-        cpu = CPU()
-        # put this here so that available cores value has
-        # context
-        if cpu.smt is not None:
-            vcpu_info["smt"] = cpu.smt
-
-        factor = float(total_vcpus) / available_cores
-        vcpu_info["overcommit-factor"] = round(factor, 2)
-
-        return vcpu_info
-
     def __summary_vm_info(self):
         _info = {}
 
         instances = self.nova.instances.values()
         if instances:
             _info['running'] = [i.uuid for i in instances]
 
-        etc_libvirt_qemu = os.path.join(HotSOSConfig.data_root,
-                                        'etc/libvirt/qemu')
-
-        cpu_models = self._get_cpu_models(etc_libvirt_qemu)
+        novalibvirt = NovaLibvirt()
+        cpu_models = novalibvirt.cpu_models
         if cpu_models:
             _info["cpu-models"] = cpu_models
 
-        vm_vcpu_info = self._get_vcpu_info(etc_libvirt_qemu)
+        vm_vcpu_info = novalibvirt.vcpu_info
         if vm_vcpu_info:
             _info["vcpu-info"] = vm_vcpu_info
 
         if _info:
             return _info
 
 
@@ -273,18 +169,16 @@
         top5 = stats.get_top_n_events_sorted(5)
         if not top5:
             return
 
         results = {"top": top5}
         # There can be a very large number of incomplete migrations so need to
         # find a useful way to represent this
-        """
-        if stats.data.incomplete_events:
-            results['incomplete-migrations'] = stats.data.incomplete_events
-        """
+        # if stats.data.incomplete_events:
+        #     results['incomplete-migrations'] = stats.data.incomplete_events
 
         return results
 
     @EVENTCALLBACKS.callback(event_group='nova.migrations')
     def src_post_live_migration(self, event):
         # section name expected to be live-migration
         return self.migration_stats_info(event), event.section
```

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/openvswitch/event_checks.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/openvswitch/event_checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
     @EVENTCALLBACKS.callback(event_group='ovs',
                              event_names=[
                                     'ovsdb-server', 'ovs-vswitchd',
                                     'receive-tunnel-port-not-found',
                                     'rx-packet-on-unassociated-datapath-port',
                                     'dpif-netlink-lost-packet-on-handler',
+                                    'assertion-failures',
                                     'unreasonably-long-poll-interval'])
     def process_log_events(self, event):
         key_by_date = True
         if event.name in ['ovs-vswitchd', 'ovsdb-server']:
             key_by_date = False
 
         ret = self.categorise_events(event, key_by_date=key_by_date,
```

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/openvswitch/summary.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/openvswitch/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/pacemaker/summary.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/pacemaker/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/rabbitmq/summary.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/rabbitmq/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/sosreport/summary.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/sosreport/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/storage/bcache_summary.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/storage/bcache_summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/storage/ceph_event_checks.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/storage/ceph_event_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/storage/ceph_summary.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/storage/ceph_summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/system/checks.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/system/checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/plugin_extensions/system/summary.py` & `hotsos-1.15.post1/hotsos/plugin_extensions/system/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos/templates/header.html` & `hotsos-1.15.post1/hotsos/templates/header.html`

 * *Files identical despite different names*

### Comparing `hotsos-1.1.14.post9/hotsos.egg-info/SOURCES.txt` & `hotsos-1.15.post1/hotsos.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -173,36 +173,42 @@
 hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml
 hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml
 hotsos/defs/scenarios/openstack/neutron/bugs/lp1928031.yaml
 hotsos/defs/scenarios/openstack/neutron/bugs/lp1929832.yaml
 hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml
 hotsos/defs/scenarios/openstack/neutron/bugs/lp1965297.yaml
 hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml
+hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml
+hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml
 hotsos/defs/scenarios/openstack/nova/config_checks.yaml
 hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
+hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml
 hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml
 hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml
 hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml
 hotsos/defs/scenarios/openstack/nova/bugs/lp1944619.yaml
 hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml
+hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml
 hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
 hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml
 hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
 hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
 hotsos/defs/scenarios/openvswitch/openvswitch.yaml
+hotsos/defs/scenarios/openvswitch/service_restarts.yaml
 hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml
 hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml
 hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml
 hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml
 hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml
 hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml
 hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml
 hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml
 hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml
 hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml
+hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml
 hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml
 hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1917475.yaml
 hotsos/defs/scenarios/pacemaker/pacemaker.yaml
 hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml
 hotsos/defs/scenarios/rabbitmq/cluster_config.yaml
 hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml
 hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml
```

### Comparing `hotsos-1.1.14.post9/pyproject.toml` & `hotsos-1.15.post1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 
 [project]
 name = "hotsos"
 description = "Software analysis toolkit. Define checks in high-level language and leverage library to perform analysis of common Cloud applications."
 readme = "README.md"
 requires-python = ">=3.8"
 dynamic = ["version"]
+# NOTE: updates to this section must also be relected in requirements.txt
 dependencies = [
     'importlib-metadata; python_version >= "3.8"',
     'click',
+    'cryptography',
+    'distro',
+    'jinja2',
     'progress',
+    'propertree',
     'pyyaml',
-    'simplejson',
-    'jinja2',
-    'cryptography',
-    'searchkit >= 0.2.3',
-    'propertree'
+    'searchkit >= 0.2.7',
+    'simplejson'
 ]
 
 [project.scripts]
 hotsos = "hotsos.cli:main"
```

