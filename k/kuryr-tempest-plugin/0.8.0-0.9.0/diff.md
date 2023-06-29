# Comparing `tmp/kuryr-tempest-plugin-0.8.0.tar.gz` & `tmp/kuryr-tempest-plugin-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kuryr-tempest-plugin-0.8.0.tar", last modified: Mon Jan 18 16:45:22 2021, max compression
+gzip compressed data, was "dist/kuryr-tempest-plugin-0.9.0.tar", last modified: Mon Mar 29 09:06:03 2021, max compression
```

## Comparing `kuryr-tempest-plugin-0.8.0.tar` & `kuryr-tempest-plugin-0.9.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:45:22.689732 kuryr-tempest-plugin-0.8.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1853 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2021-01-18 16:45:22.000000 kuryr-tempest-plugin-0.8.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8671 2021-01-18 16:45:22.000000 kuryr-tempest-plugin-0.8.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1447 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2776 2021-01-18 16:45:22.689732 kuryr-tempest-plugin-0.8.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1532 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:45:22.661728 kuryr-tempest-plugin-0.8.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1327 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/devstack/plugin.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:45:22.661728 kuryr-tempest-plugin-0.8.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:45:22.665729 kuryr-tempest-plugin-0.8.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2675 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:45:22.665729 kuryr-tempest-plugin-0.8.0/doc/source/scenario_tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/doc/source/scenario_tests/scenario.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:45:22.665729 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5209 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1965 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:45:22.665729 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:45:22.665729 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:45:22.669729 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    58494 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25833 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/base_network_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/consts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3412 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_cross_ping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2488 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_cross_ping_multi_worker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1809 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_daemon.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8362 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_ha.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3499 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_kuryr_restart.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18213 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_namespace.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7268 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_network_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3060 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_npwg_multi_vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4139 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_ocp_route.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19154 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_port_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5716 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2263 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/test_pods.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:45:22.665729 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2776 2021-01-18 16:45:22.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2027 2021-01-18 16:45:22.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-01-18 16:45:22.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2021-01-18 16:45:22.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-01-18 16:45:22.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-01-18 16:45:22.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2021-01-18 16:45:22.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-01-18 16:45:22.000000 kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:45:22.661728 kuryr-tempest-plugin-0.8.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:45:22.673730 kuryr-tempest-plugin-0.8.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/releasenotes/notes/drop-py-2-7-059b699f12500b28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2021-01-18 16:45:22.689732 kuryr-tempest-plugin-0.8.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-01-18 16:45:22.689732 kuryr-tempest-plugin-0.8.0/test_container/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/test_container/Dockerfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4628 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/test_container/Dockerfile.builder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1918 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/test_container/README.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2917 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/test_container/curl_builder.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      508 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/test_container/mkrootfs.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)  7913700 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/test_container/rootfs.tar.xz
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2229 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/test_container/server.go
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/test_container/udp_client.go
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2021-01-18 16:44:06.000000 kuryr-tempest-plugin-0.8.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-29 09:06:03.935362 kuryr-tempest-plugin-0.9.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1889 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1137 2021-03-29 09:06:03.000000 kuryr-tempest-plugin-0.9.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9102 2021-03-29 09:06:03.000000 kuryr-tempest-plugin-0.9.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1447 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2942 2021-03-29 09:06:03.935362 kuryr-tempest-plugin-0.9.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1658 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-29 09:06:03.899362 kuryr-tempest-plugin-0.9.0/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1519 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/devstack/plugin.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-29 09:06:03.899362 kuryr-tempest-plugin-0.9.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-29 09:06:03.899362 kuryr-tempest-plugin-0.9.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2675 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-29 09:06:03.903362 kuryr-tempest-plugin-0.9.0/doc/source/scenario_tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/doc/source/scenario_tests/scenario.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-29 09:06:03.903362 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5337 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1965 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-29 09:06:03.903362 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-29 09:06:03.907362 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    60533 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25844 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/base_network_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/consts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3412 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_cross_ping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2488 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_cross_ping_multi_worker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1809 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_daemon.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8362 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_ha.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3499 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_kuryr_restart.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18213 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_namespace.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15394 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_network_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3060 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_npwg_multi_vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4139 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_ocp_route.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19154 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_port_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6447 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-29 09:06:03.903362 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2942 2021-03-29 09:06:03.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2044 2021-03-29 09:06:03.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-03-29 09:06:03.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2021-03-29 09:06:03.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-03-29 09:06:03.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-03-29 09:06:03.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2021-03-29 09:06:03.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-03-29 09:06:03.000000 kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-29 09:06:03.899362 kuryr-tempest-plugin-0.9.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-29 09:06:03.907362 kuryr-tempest-plugin-0.9.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/releasenotes/notes/drop-py-2-7-059b699f12500b28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2021-03-29 09:06:03.935362 kuryr-tempest-plugin-0.9.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-29 09:06:03.935362 kuryr-tempest-plugin-0.9.0/test_container/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/test_container/Dockerfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4642 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/test_container/Dockerfile.builder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1918 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/test_container/README.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2917 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/test_container/curl_builder.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-29 09:06:03.935362 kuryr-tempest-plugin-0.9.0/test_container/kuryr_sctp_demo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      725 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/test_container/kuryr_sctp_demo/Dockerfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1435 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/test_container/kuryr_sctp_demo/sctp_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1278 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/test_container/kuryr_sctp_demo/sctp_server.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      508 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/test_container/mkrootfs.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)  7913700 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/test_container/rootfs.tar.xz
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2229 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/test_container/server.go
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/test_container/udp_client.go
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2021-03-29 09:05:29.000000 kuryr-tempest-plugin-0.9.0/tox.ini
```

### Comparing `kuryr-tempest-plugin-0.8.0/.zuul.yaml` & `kuryr-tempest-plugin-0.9.0/.zuul.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -43,19 +43,21 @@
     nodeset: openstack-single-node-bionic
     required-projects:
     - name: openstack/diskimage-builder
       override-checkout: 2.30.0
     vars:
       devstack_localrc:
         USE_PYTHON3: True
+    voting: false
 
 - job:
     name: kuryr-kubernetes-tempest-stein
     parent: kuryr-kubernetes-tempest
     override-checkout: stable/stein
     nodeset: openstack-single-node-bionic
     required-projects:
     - name: openstack/diskimage-builder
       override-checkout: 2.30.0
     vars:
       devstack_localrc:
         USE_PYTHON3: True
+    voting: false
```

### Comparing `kuryr-tempest-plugin-0.8.0/AUTHORS` & `kuryr-tempest-plugin-0.9.0/AUTHORS`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 Luis Tomas Bolivar <ltomasbo@redhat.com>
 Matthew Thode <mthode@mthode.org>
 Maysa Macedo <maysa.macedo95@gmail.com>
 Michał Dulko <mdulko@redhat.com>
 Peng Liu <pliu@redhat.com>
 Ramon Lobillo <rlobillo@redhat.com>
 Roman Dobosz <gryf73@gmail.com>
+Tabitha <fifedolapo02@gmail.com>
 Yossi Boaron <yossi.boaron.1234@gmail.com>
 gryf <gryf73@gmail.com>
 inspurericzhang <zhanglf01@inspur.com>
 melissaml <ma.lei@99cloud.net>
 naseeb panghal <Panghal.naseeb@gmail.com>
 pengyuesheng <pengyuesheng@gohighsec.com>
 scavnicka <scavnicka.sarka@gmail.com>
```

### Comparing `kuryr-tempest-plugin-0.8.0/CONTRIBUTING.rst` & `kuryr-tempest-plugin-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/ChangeLog` & `kuryr-tempest-plugin-0.9.0/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 CHANGES
 =======
 
+0.9.0
+-----
+
+* Fix create\_vm\_for\_connectivity\_test
+* Adds connectivity test for SCTP service
+* Increase the timeout for controller to be ready
+* Make stable/train job non-voting
+* Updates Kuryr tempest README
+* Adds Kuryr-sctp-demo application
+* Make Stein gate non-voting
+* New test for services without selectors with NP
+* Change registry from docker.io to quay.io for test container image
+* Remove uselsess files and tests
+
 0.8.0
 -----
 
 * Create Tempest case to ensure Services without Selectors
 * Use registry at quay.io instead of docker.io
 * Split checks in test\_network\_policy\_add\_remove\_pod
 * Add stable/victoria job
```

### Comparing `kuryr-tempest-plugin-0.8.0/HACKING.rst` & `kuryr-tempest-plugin-0.9.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/LICENSE` & `kuryr-tempest-plugin-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/PKG-INFO` & `kuryr-tempest-plugin-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kuryr-tempest-plugin
-Version: 0.8.0
+Version: 0.9.0
 Summary: Kuryr Tempest Plugin
 Home-page: https://docs.openstack.org/kuryr-tempest-plugin/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache Software License
 Description: ========================
         Team and repository tags
@@ -46,25 +46,30 @@
         Clone this repository and call from the repo::
         
             $ pip install -e .
         
         Running the tests
         -----------------
         
-        To run all the tests from this plugin, call from the tempest repo::
+        To verify the functionality of Kuryr by running tests from this plugin;
+        From the tempest repo, initialize stestr::
         
-            $ tox -e all -- kuryr_tempest_plugin
+            $ stestr init
+        
+        Then, to run all the tests from this plugin, call::
+        
+            $ tempest run -r 'kuryr_tempest_plugin.*'
         
         To run a single test case, call with full path, for example::
         
-            $ tox -e all -- kuryr_tempest_plugin.tests.scenario.test_cross_ping.TestCrossPingScenario.test_vm_pod_ping
+            $ tempest run -r 'kuryr_tempest_plugin.tests.scenario.test_cross_ping.TestCrossPingScenario.test_vm_pod_ping*'
         
         To retrieve a list of all tempest tests, run::
         
-            $ testr list-tests
+            $ tempest run -l
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `kuryr-tempest-plugin-0.8.0/README.rst` & `kuryr-tempest-plugin-0.9.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -38,18 +38,23 @@
 Clone this repository and call from the repo::
 
     $ pip install -e .
 
 Running the tests
 -----------------
 
-To run all the tests from this plugin, call from the tempest repo::
+To verify the functionality of Kuryr by running tests from this plugin;
+From the tempest repo, initialize stestr::
 
-    $ tox -e all -- kuryr_tempest_plugin
+    $ stestr init
+
+Then, to run all the tests from this plugin, call::
+
+    $ tempest run -r 'kuryr_tempest_plugin.*'
 
 To run a single test case, call with full path, for example::
 
-    $ tox -e all -- kuryr_tempest_plugin.tests.scenario.test_cross_ping.TestCrossPingScenario.test_vm_pod_ping
+    $ tempest run -r 'kuryr_tempest_plugin.tests.scenario.test_cross_ping.TestCrossPingScenario.test_vm_pod_ping*'
 
 To retrieve a list of all tempest tests, run::
 
-    $ testr list-tests
+    $ tempest run -l
```

### Comparing `kuryr-tempest-plugin-0.8.0/devstack/plugin.sh` & `kuryr-tempest-plugin-0.9.0/devstack/plugin.sh`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,20 @@
     pushd "${DEST}/kuryr-tempest-plugin/test_container"
 
     # FIXME(dulek): Until https://github.com/containers/buildah/issues/1206 is
     #               resolved instead of podman we need to use buildah directly,
     #               hence this awful if clause.
     if [[ ${CONTAINER_ENGINE} == 'crio' ]]; then
         sudo buildah bud -t quay.io/kuryr/demo -f Dockerfile .
+        sudo buildah bud -t quay.io/kuryr/sctp-demo -f \
+            kuryr_sctp_demo/Dockerfile .
     else
         docker build -t quay.io/kuryr/demo . -f Dockerfile
+        docker build -t quay.io/kuryr/sctp-demo . -f \
+            kuryr_sctp_demo/Dockerfile
     fi
     popd
 }
 
 function install_kuryr_tempest_plugin {
     setup_dev_lib "kuryr-tempest-plugin"
 }
```

### Comparing `kuryr-tempest-plugin-0.8.0/doc/source/conf.py` & `kuryr-tempest-plugin-0.9.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/config.py` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,16 @@
     cfg.BoolOpt("ap_ha", default=False,
                 help='Whether or not A/P HA of kuryr-controller is enabled'),
     cfg.StrOpt("controller_deployment_name", default="kuryr-controller",
                help="Name of Kubernetes Deployment running kuryr-controller "
                     "Pods"),
     cfg.BoolOpt("test_udp_services", default=False,
                 help="Whether or not service UDP tests will be running"),
+    cfg.BoolOpt("test_sctp_services", default=False,
+                help="Whether or not service SCTP tests will be running"),
     cfg.BoolOpt("multi_worker_setup", default=False, help="Whether or not we "
                 "have a multi-worker setup"),
     cfg.BoolOpt("cloud_provider", default=False, help="Whether or not a "
                 "cloud provider is set"),
     cfg.BoolOpt("validate_crd", default=False, help="Whether or not kuryr "
                 "CRDs should be validated"),
     cfg.BoolOpt("kuryrloadbalancers", default=False, help="Whether or not "
```

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/plugin.py` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/base.py` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import json
 import six
 import socket
 import time
 
 from oslo_log import log as logging
 
+import netaddr
 import requests
 
 import kubernetes
 from kubernetes import client as k8s_client
 from kubernetes import config as k8s_config
 from kubernetes.stream import stream
 from kuryr_tempest_plugin.tests.scenario import consts
@@ -628,16 +629,21 @@
                                       protocol="TCP", port=80,
                                       target_port=8080, label=None,
                                       namespace="default", get_ip=True,
                                       service_name=None, cleanup=True):
 
         label = label or data_utils.rand_name('kuryr-app')
         for i in range(pod_num):
-            pod_name, pod = cls.create_pod(
-                labels={"app": label}, namespace=namespace)
+            if protocol == "SCTP":
+                pod_name, pod = cls.create_pod(
+                    labels={"app": label}, image='quay.io/kuryr/sctp-demo',
+                    namespace=namespace)
+            else:
+                pod_name, pod = cls.create_pod(
+                    labels={"app": label}, namespace=namespace)
             if cleanup:
                 cls.addClassResourceCleanup(cls.delete_pod, pod_name,
                                             namespace=namespace)
         cls.pod_num = pod_num
         service_name, service_obj = cls.create_service(
             pod_label=pod.metadata.labels, spec_type=spec_type,
             protocol=protocol, port=port, target_port=target_port,
@@ -720,20 +726,22 @@
                 return True
             except kubernetes.client.rest.ApiException:
                 pass
 
         return False
 
     @classmethod
-    def create_namespace(cls, name=None, wait_for_crd=True,
+    def create_namespace(cls, name=None, labels=None,
+                         wait_for_crd=True,
                          timeout_period=consts.NS_TIMEOUT):
         if not name:
             name = data_utils.rand_name(prefix='kuryr-namespace')
         namespace = cls.k8s_client.V1Namespace()
-        namespace.metadata = cls.k8s_client.V1ObjectMeta(name=name)
+        namespace.metadata = cls.k8s_client.V1ObjectMeta(name=name,
+                                                         labels=labels)
         namespace_obj = cls.k8s_client.CoreV1Api().create_namespace(
             body=namespace)
 
         if not wait_for_crd or not CONF.kuryr_kubernetes.subnet_per_namespace:
             # You cannot create pods until default ServiceAccount for the
             # namespace is created, let's wait for it.
             if not cls.wait_for_ns_serviceaccount(name):
@@ -949,14 +957,28 @@
             if stderr:
                 LOG.error('Failed to reach service at {}:{} '
                           'Err: {}'.format(server_ip, server_port, stderr))
                 time.sleep(10)
                 return
             return stdout
 
+        def req_sctp():
+            cmd = "python3 sctp_client.py {} {}".format(
+                server_ip, server_port)
+            pod_cmd = ["/bin/sh", "-c", cmd]
+            stdout, stderr = self.exec_command_in_pod(pod, pod_cmd,
+                                                      namespace=namespace_name,
+                                                      stderr=True)
+            if stderr:
+                LOG.error('Failed to reach service at {}:{} '
+                          'Err: {}'.format(server_ip, server_port, stderr))
+                time.sleep(10)
+                return
+            return stdout
+
         def pred(tester, responses):
             if protocol == 'TCP':
                 unique_resps = set(resp for resp in responses if resp)
             else:
                 unique_resps = set(resp for resp in responses if resp
                                    != '')
             tester.assertEqual(amount, len(unique_resps),
@@ -965,14 +987,18 @@
 
         if protocol == 'TCP':
             req = req_tcp
         elif protocol == "UDP":
             self.assertIsNotNone(server_port, "server_port must be "
                                               "provided for UDP protocol")
             req = req_udp
+        elif protocol == "SCTP":
+            self.assertIsNotNone(server_port, "server_port must be "
+                                              "provided for SCTP protocol")
+            req = req_sctp
         else:
             LOG.info("Unsupported protocol %s, returning", protocol)
             return
         self._run_and_assert(req, pred)
 
     def _run_and_assert(self, fn, predicate, retry_repetitions=100):
         resps = [fn() for _ in range(retry_repetitions)]
@@ -1060,15 +1086,21 @@
         if not annotation_success:
             msg = "Timed out waiting for %s in ep=%s annotation to appear" % (
                     ann_string, ep_name)
             raise lib_exc.TimeoutException(msg)
 
     def create_vm_for_connectivity_test(self):
         keypair = self.create_keypair()
-        sec_grp = self._create_security_group()
+        # NOTE(maysams): we need to support older versions of Tempest.
+        # So, let's try calling the non-private method and if fails
+        # we default to the private one.
+        try:
+            sec_grp = self._create_security_group()
+        except AttributeError:
+            sec_grp = self.create_security_group()
         security_groups = [
             {'name': sec_grp['name']}
         ]
         server = self.create_server(name=data_utils.rand_name(prefix='kuryr'),
                                     key_name=keypair['name'],
                                     security_groups=security_groups)
         fip = self.create_floating_ip(server)
@@ -1253,15 +1285,15 @@
                 namespace=system_namespace,
                 pod_status='Running',
                 retries=120)
 
             # Wait until kuryr-controller pools are reloaded, i.e.,
             # kuryr-controller is ready
             res = test_utils.call_until_true(
-                self.get_pod_readiness, 30, 1, kuryr_pod_name,
+                self.get_pod_readiness, 60, 1, kuryr_pod_name,
                 namespace=system_namespace, container_name='controller')
             self.assertTrue(res, 'Timed out waiting for '
                                  'kuryr-controller to reload pools.')
 
     def update_config_map_ini_section_and_restart(
             self, name, conf_to_update, section,
             namespace=CONF.kuryr_kubernetes.kube_system_namespace, **kwargs):
@@ -1315,19 +1347,34 @@
         # check service status as there are some issues with the FIPs
         # and OVN gates
         clusterip_svc_ip = self.get_service_ip(self.service_name,
                                                spec_type='ClusterIP',
                                                namespace=namespace)
         pod_num = pod_num or self.pod_num
         if not pod_name:
-            pod_name, _ = self.create_pod(namespace=namespace, labels=labels)
+            if protocol == "SCTP":
+                pod_name, _ = self.create_pod(
+                    labels=labels, image='quay.io/kuryr/sctp-demo',
+                    namespace=namespace)
+            else:
+                pod_name, _ = self.create_pod(
+                    namespace=namespace, labels=labels)
             if cleanup:
                 self.addClassResourceCleanup(self.delete_pod, pod_name,
                                              namespace=namespace)
         self.assert_backend_amount_from_pod(
             clusterip_svc_ip,
             pod_num,
             pod_name,
             service_port,
             protocol,
             namespace_name=namespace)
         return pod_name
+
+    def get_curl_template(self, ip_or_cidr, extra_args='', port=False):
+        ipn = netaddr.IPNetwork(ip_or_cidr)
+
+        curl_tmpl = "curl " + extra_args if extra_args else "curl"
+        curl_tmpl = (curl_tmpl + " [{}]"
+                     if ipn.version == 6 else curl_tmpl + " {}")
+
+        return curl_tmpl + "{}" if port else curl_tmpl
```

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/base_network_policy.py` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/base_network_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,28 +142,29 @@
         self.assertTrue(ingress_block_found)
         self.assertTrue(egress_block_found)
 
     @decorators.idempotent_id('a9db5bc5-e921-4819-8301-5431437c76f8')
     def test_ipblock_network_policy_allow_except(self):
         namespace_name, namespace = self.create_namespace()
         self.addCleanup(self.delete_namespace, namespace_name)
+
         if CONF.kuryr_kubernetes.kuryrnetworks:
             cidr = self.get_kuryr_network_crds(
                 namespace_name)['status']['subnetCIDR']
         else:
             crd_name = 'ns-' + namespace_name
             cidr = self.get_kuryr_net_crds(
                 crd_name)['spec']['subnetCIDR']
 
         ipn = netaddr.IPNetwork(cidr)
         max_prefixlen = "/32"
-        curl_tmpl = "curl {}{}"
         if ipn.version == 6:
             max_prefixlen = "/128"
-            curl_tmpl = "curl [{}]{}"
+
+        curl_tmpl = self.get_curl_template(cidr, extra_args='-m 5', port=True)
 
         allow_all_cidr = cidr
         pod_ip_list = []
         pod_name_list = []
         cmd_list = []
 
         for i in range(4):
```

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/consts.py` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/consts.py`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_cross_ping.py` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_cross_ping.py`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_cross_ping_multi_worker.py` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_cross_ping_multi_worker.py`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_daemon.py` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_daemon.py`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_ha.py` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_ha.py`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_kuryr_restart.py` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_kuryr_restart.py`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_namespace.py` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_namespace.py`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_npwg_multi_vif.py` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_npwg_multi_vif.py`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_ocp_route.py` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_ocp_route.py`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_port_pool.py` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_port_pool.py`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin/tests/scenario/test_service.py` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin/tests/scenario/test_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -132,7 +132,26 @@
     def test_service_without_selector(self):
         # Create a service without selector
         ns_name, ns_obj = self.create_namespace()
         self.addCleanup(self.delete_namespace, ns_name)
         self.service_without_selector_base(namespace=ns_name)
 
         self.check_service_internal_connectivity(namespace=ns_name)
+
+
+class TestSCTPServiceScenario(base.BaseKuryrScenarioTest):
+
+    @classmethod
+    def skip_checks(cls):
+        super(TestSCTPServiceScenario, cls).skip_checks()
+        if not CONF.kuryr_kubernetes.service_tests_enabled:
+            raise cls.skipException("Service tests are not enabled")
+        if not CONF.kuryr_kubernetes.test_sctp_services:
+            raise cls.skipException("Service SCTP tests are not enabled")
+
+    @decorators.idempotent_id('bb8cc977-c867-4766-b623-137d8395cb60')
+    def test_service_sctp_ping(self):
+        self.create_setup_for_service_test(
+            protocol="SCTP", port=90, target_port=9090)
+
+        self.check_service_internal_connectivity(
+            service_port='90', protocol='SCTP')
```

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin.egg-info/PKG-INFO` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kuryr-tempest-plugin
-Version: 0.8.0
+Version: 0.9.0
 Summary: Kuryr Tempest Plugin
 Home-page: https://docs.openstack.org/kuryr-tempest-plugin/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache Software License
 Description: ========================
         Team and repository tags
@@ -46,25 +46,30 @@
         Clone this repository and call from the repo::
         
             $ pip install -e .
         
         Running the tests
         -----------------
         
-        To run all the tests from this plugin, call from the tempest repo::
+        To verify the functionality of Kuryr by running tests from this plugin;
+        From the tempest repo, initialize stestr::
         
-            $ tox -e all -- kuryr_tempest_plugin
+            $ stestr init
+        
+        Then, to run all the tests from this plugin, call::
+        
+            $ tempest run -r 'kuryr_tempest_plugin.*'
         
         To run a single test case, call with full path, for example::
         
-            $ tox -e all -- kuryr_tempest_plugin.tests.scenario.test_cross_ping.TestCrossPingScenario.test_vm_pod_ping
+            $ tempest run -r 'kuryr_tempest_plugin.tests.scenario.test_cross_ping.TestCrossPingScenario.test_vm_pod_ping*'
         
         To retrieve a list of all tempest tests, run::
         
-            $ testr list-tests
+            $ tempest run -l
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `kuryr-tempest-plugin-0.8.0/kuryr_tempest_plugin.egg-info/SOURCES.txt` & `kuryr-tempest-plugin-0.9.0/kuryr_tempest_plugin.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -23,18 +23,15 @@
 kuryr_tempest_plugin.egg-info/SOURCES.txt
 kuryr_tempest_plugin.egg-info/dependency_links.txt
 kuryr_tempest_plugin.egg-info/entry_points.txt
 kuryr_tempest_plugin.egg-info/not-zip-safe
 kuryr_tempest_plugin.egg-info/pbr.json
 kuryr_tempest_plugin.egg-info/requires.txt
 kuryr_tempest_plugin.egg-info/top_level.txt
-kuryr_tempest_plugin/services/__init__.py
 kuryr_tempest_plugin/tests/__init__.py
-kuryr_tempest_plugin/tests/base.py
-kuryr_tempest_plugin/tests/test_pods.py
 kuryr_tempest_plugin/tests/scenario/README.rst
 kuryr_tempest_plugin/tests/scenario/__init__.py
 kuryr_tempest_plugin/tests/scenario/base.py
 kuryr_tempest_plugin/tests/scenario/base_network_policy.py
 kuryr_tempest_plugin/tests/scenario/consts.py
 kuryr_tempest_plugin/tests/scenario/test_cross_ping.py
 kuryr_tempest_plugin/tests/scenario/test_cross_ping_multi_worker.py
@@ -51,8 +48,11 @@
 test_container/Dockerfile
 test_container/Dockerfile.builder
 test_container/README.rst
 test_container/curl_builder.sh
 test_container/mkrootfs.sh
 test_container/rootfs.tar.xz
 test_container/server.go
-test_container/udp_client.go
+test_container/udp_client.go
+test_container/kuryr_sctp_demo/Dockerfile
+test_container/kuryr_sctp_demo/sctp_client.py
+test_container/kuryr_sctp_demo/sctp_server.py
```

### Comparing `kuryr-tempest-plugin-0.8.0/setup.cfg` & `kuryr-tempest-plugin-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/setup.py` & `kuryr-tempest-plugin-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/test_container/Dockerfile.builder` & `kuryr-tempest-plugin-0.9.0/test_container/Dockerfile.builder`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM alpine:3.12
+FROM quay.io/kuryr/alpine:3.12
 
 RUN apk add --no-cache \
 		bash \
 		bzip2 \
 		coreutils \
 		curl \
 		gcc \
```

### Comparing `kuryr-tempest-plugin-0.8.0/test_container/README.rst` & `kuryr-tempest-plugin-0.9.0/test_container/README.rst`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/test_container/curl_builder.sh` & `kuryr-tempest-plugin-0.9.0/test_container/curl_builder.sh`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/test_container/rootfs.tar.xz` & `kuryr-tempest-plugin-0.9.0/test_container/rootfs.tar.xz`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/test_container/server.go` & `kuryr-tempest-plugin-0.9.0/test_container/server.go`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/test_container/udp_client.go` & `kuryr-tempest-plugin-0.9.0/test_container/udp_client.go`

 * *Files identical despite different names*

### Comparing `kuryr-tempest-plugin-0.8.0/tox.ini` & `kuryr-tempest-plugin-0.9.0/tox.ini`

 * *Files identical despite different names*

