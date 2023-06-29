# Comparing `tmp/paracrine-0.0.8.tar.gz` & `tmp/paracrine-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paracrine-0.0.8.tar", last modified: Sun Jun  4 19:48:54 2023, max compression
+gzip compressed data, was "paracrine-0.0.9.tar", last modified: Thu Jun 29 21:24:21 2023, max compression
```

## Comparing `paracrine-0.0.8.tar` & `paracrine-0.0.9.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.506911 paracrine-0.0.8/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)    34520 2023-01-20 15:32:39.000000 paracrine-0.0.8/LICENSE
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       30 2023-01-21 23:59:01.000000 paracrine-0.0.8/MANIFEST.in
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3597 2023-06-04 19:48:54.506911 paracrine-0.0.8/PKG-INFO
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3071 2023-05-20 20:51:52.000000 paracrine-0.0.8/README.md
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.502911 paracrine-0.0.8/paracrine/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4661 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/__init__.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.502911 paracrine-0.0.8/paracrine/commands/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/commands/__init__.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      969 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/commands/login.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      409 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/commands/reboot.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      108 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/commands/setup.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2152 2023-06-04 15:34:10.000000 paracrine-0.0.8/paracrine/deps.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.502911 paracrine-0.0.8/paracrine/helpers/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/helpers/__init__.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     6180 2023-06-04 15:34:10.000000 paracrine-0.0.8/paracrine/helpers/config.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1282 2023-06-01 22:07:09.000000 paracrine-0.0.8/paracrine/helpers/cron.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3894 2023-06-02 18:09:42.000000 paracrine-0.0.8/paracrine/helpers/debian.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)    10423 2023-06-04 19:47:23.000000 paracrine-0.0.8/paracrine/helpers/fs.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      939 2023-06-03 22:12:18.000000 paracrine-0.0.8/paracrine/helpers/network.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      412 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/helpers/python.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2382 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/helpers/systemd.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1232 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/helpers/users.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4642 2023-06-04 15:34:10.000000 paracrine-0.0.8/paracrine/runner.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.502911 paracrine-0.0.8/paracrine/runners/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/runners/__init__.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      828 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/runners/aws.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3914 2023-06-04 15:34:10.000000 paracrine-0.0.8/paracrine/runners/certs.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2866 2023-06-04 15:34:10.000000 paracrine-0.0.8/paracrine/runners/core.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.506911 paracrine-0.0.8/paracrine/services/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-01-25 00:04:12.000000 paracrine-0.0.8/paracrine/services/__init__.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.506911 paracrine-0.0.8/paracrine/services/cockroachdb/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1067 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/cockroachdb/__init__.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2712 2023-06-04 15:34:10.000000 paracrine-0.0.8/paracrine/services/cockroachdb/certs.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      699 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/cockroachdb/common.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      670 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/cockroachdb/init.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2441 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/cockroachdb/node.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      172 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/ntp.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4091 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/pleroma.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1242 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/postgresql.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.506911 paracrine-0.0.8/paracrine/services/redis/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       88 2023-06-03 22:12:18.000000 paracrine-0.0.8/paracrine/services/redis/__init__.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1144 2023-06-04 19:47:23.000000 paracrine-0.0.8/paracrine/services/redis/init.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2336 2023-06-04 19:47:23.000000 paracrine-0.0.8/paracrine/services/redis/node.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.506911 paracrine-0.0.8/paracrine/services/wireguard/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       62 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/wireguard/__init__.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3493 2023-05-20 21:43:24.000000 paracrine-0.0.8/paracrine/services/wireguard/bootstrap.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      248 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/wireguard/common.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1147 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/wireguard/core.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.506911 paracrine-0.0.8/paracrine/templates/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       79 2023-01-20 15:21:51.000000 paracrine-0.0.8/paracrine/templates/certbot_requirements.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      503 2023-05-20 19:57:25.000000 paracrine-0.0.8/paracrine/templates/cockroach.service.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1799 2023-05-23 22:35:18.000000 paracrine-0.0.8/paracrine/templates/config.exs.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      121 2023-04-19 23:19:20.000000 paracrine-0.0.8/paracrine/templates/cron.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2716 2023-01-25 00:18:54.000000 paracrine-0.0.8/paracrine/templates/pleroma.nginx.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      576 2023-06-04 19:47:23.000000 paracrine-0.0.8/paracrine/templates/redis-sentinel.conf.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      438 2023-06-04 19:47:23.000000 paracrine-0.0.8/paracrine/templates/redis.conf.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       24 2023-01-25 00:18:56.000000 paracrine-0.0.8/paracrine/templates/robots.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      300 2023-01-25 00:18:53.000000 paracrine-0.0.8/paracrine/templates/setup_db.psql.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      260 2023-01-28 23:21:08.000000 paracrine-0.0.8/paracrine/templates/wg.conf.j2
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.502911 paracrine-0.0.8/paracrine.egg-info/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3597 2023-06-04 19:48:54.000000 paracrine-0.0.8/paracrine.egg-info/PKG-INFO
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1704 2023-06-04 19:48:54.000000 paracrine-0.0.8/paracrine.egg-info/SOURCES.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)        1 2023-06-04 19:48:54.000000 paracrine-0.0.8/paracrine.egg-info/dependency_links.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       46 2023-06-04 19:48:54.000000 paracrine-0.0.8/paracrine.egg-info/requires.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       10 2023-06-04 19:48:54.000000 paracrine-0.0.8/paracrine.egg-info/top_level.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      733 2023-06-04 19:47:49.000000 paracrine-0.0.8/pyproject.toml
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       38 2023-06-04 19:48:54.506911 paracrine-0.0.8/setup.cfg
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.506911 paracrine-0.0.8/tests/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      835 2023-01-28 23:21:08.000000 paracrine-0.0.8/tests/test_ssh.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-29 21:24:21.248034 paracrine-0.0.9/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)    34520 2023-01-20 15:32:39.000000 paracrine-0.0.9/LICENSE
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       30 2023-01-21 23:59:01.000000 paracrine-0.0.9/MANIFEST.in
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3597 2023-06-29 21:24:21.248034 paracrine-0.0.9/PKG-INFO
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3071 2023-05-20 20:51:52.000000 paracrine-0.0.9/README.md
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-29 21:24:21.244034 paracrine-0.0.9/paracrine/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4661 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/__init__.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-29 21:24:21.244034 paracrine-0.0.9/paracrine/commands/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/commands/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      969 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/commands/login.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      409 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/commands/reboot.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      108 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/commands/setup.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2242 2023-06-29 20:59:01.000000 paracrine-0.0.9/paracrine/deps.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-29 21:24:21.244034 paracrine-0.0.9/paracrine/helpers/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/helpers/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     6180 2023-06-04 15:34:10.000000 paracrine-0.0.9/paracrine/helpers/config.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1282 2023-06-01 22:07:09.000000 paracrine-0.0.9/paracrine/helpers/cron.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3894 2023-06-02 18:09:42.000000 paracrine-0.0.9/paracrine/helpers/debian.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)    10423 2023-06-29 19:55:30.000000 paracrine-0.0.9/paracrine/helpers/fs.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      939 2023-06-03 22:12:18.000000 paracrine-0.0.9/paracrine/helpers/network.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      412 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/helpers/python.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2382 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/helpers/systemd.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1232 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/helpers/users.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     5474 2023-06-29 20:59:23.000000 paracrine-0.0.9/paracrine/runner.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-29 21:24:21.244034 paracrine-0.0.9/paracrine/runners/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/runners/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      828 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/runners/aws.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3914 2023-06-04 15:34:10.000000 paracrine-0.0.9/paracrine/runners/certs.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2866 2023-06-04 15:34:10.000000 paracrine-0.0.9/paracrine/runners/core.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-29 21:24:21.244034 paracrine-0.0.9/paracrine/services/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-01-25 00:04:12.000000 paracrine-0.0.9/paracrine/services/__init__.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-29 21:24:21.248034 paracrine-0.0.9/paracrine/services/cockroachdb/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1067 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/services/cockroachdb/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2712 2023-06-04 15:34:10.000000 paracrine-0.0.9/paracrine/services/cockroachdb/certs.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      699 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/services/cockroachdb/common.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      659 2023-06-29 20:14:20.000000 paracrine-0.0.9/paracrine/services/cockroachdb/init.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2441 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/services/cockroachdb/node.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      172 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/services/ntp.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4111 2023-06-29 20:59:35.000000 paracrine-0.0.9/paracrine/services/pleroma.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1242 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/services/postgresql.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-29 21:24:21.248034 paracrine-0.0.9/paracrine/services/redis/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       88 2023-06-03 22:12:18.000000 paracrine-0.0.9/paracrine/services/redis/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      695 2023-06-29 20:05:05.000000 paracrine-0.0.9/paracrine/services/redis/common.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1092 2023-06-29 20:05:05.000000 paracrine-0.0.9/paracrine/services/redis/init.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2284 2023-06-29 20:05:05.000000 paracrine-0.0.9/paracrine/services/redis/node.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-29 21:24:21.248034 paracrine-0.0.9/paracrine/services/wireguard/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       62 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/services/wireguard/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3493 2023-05-20 21:43:24.000000 paracrine-0.0.9/paracrine/services/wireguard/bootstrap.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      248 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/services/wireguard/common.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1147 2023-05-20 20:51:52.000000 paracrine-0.0.9/paracrine/services/wireguard/core.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-29 21:24:21.248034 paracrine-0.0.9/paracrine/templates/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       79 2023-01-20 15:21:51.000000 paracrine-0.0.9/paracrine/templates/certbot_requirements.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      503 2023-05-20 19:57:25.000000 paracrine-0.0.9/paracrine/templates/cockroach.service.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1799 2023-06-16 20:41:14.000000 paracrine-0.0.9/paracrine/templates/config.exs.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      121 2023-04-19 23:19:20.000000 paracrine-0.0.9/paracrine/templates/cron.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2716 2023-01-25 00:18:54.000000 paracrine-0.0.9/paracrine/templates/pleroma.nginx.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      576 2023-06-04 19:47:23.000000 paracrine-0.0.9/paracrine/templates/redis-sentinel.conf.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      450 2023-06-29 19:58:47.000000 paracrine-0.0.9/paracrine/templates/redis.conf.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       24 2023-01-25 00:18:56.000000 paracrine-0.0.9/paracrine/templates/robots.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      300 2023-01-25 00:18:53.000000 paracrine-0.0.9/paracrine/templates/setup_db.psql.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      260 2023-01-28 23:21:08.000000 paracrine-0.0.9/paracrine/templates/wg.conf.j2
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-29 21:24:21.244034 paracrine-0.0.9/paracrine.egg-info/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3597 2023-06-29 21:24:21.000000 paracrine-0.0.9/paracrine.egg-info/PKG-INFO
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1766 2023-06-29 21:24:21.000000 paracrine-0.0.9/paracrine.egg-info/SOURCES.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        1 2023-06-29 21:24:21.000000 paracrine-0.0.9/paracrine.egg-info/dependency_links.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       46 2023-06-29 21:24:21.000000 paracrine-0.0.9/paracrine.egg-info/requires.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       10 2023-06-29 21:24:21.000000 paracrine-0.0.9/paracrine.egg-info/top_level.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      733 2023-06-29 21:23:48.000000 paracrine-0.0.9/pyproject.toml
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       38 2023-06-29 21:24:21.248034 paracrine-0.0.9/setup.cfg
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-29 21:24:21.248034 paracrine-0.0.9/tests/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      667 2023-06-29 20:59:00.000000 paracrine-0.0.9/tests/test_dependencies.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      835 2023-06-29 20:50:43.000000 paracrine-0.0.9/tests/test_ssh.py
```

### Comparing `paracrine-0.0.8/LICENSE` & `paracrine-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/PKG-INFO` & `paracrine-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paracrine
-Version: 0.0.8
+Version: 0.0.9
 Summary: A system deployment tool
 Author-email: Tom Parker-Shemilt <palfrey@tevp.net>
 Project-URL: Homepage, https://github.com/palfrey/paracrine
 Project-URL: Bug Tracker, https://github.com/palfrey/paracrine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `paracrine-0.0.8/README.md` & `paracrine-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/__init__.py` & `paracrine-0.0.9/paracrine/__init__.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/commands/login.py` & `paracrine-0.0.9/paracrine/commands/login.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/deps.py` & `paracrine-0.0.9/paracrine/deps.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 from types import ModuleType
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from mergedeep import merge
 
 from .helpers.config import clear_return_data, get_return_data, set_data
 
-Modules = List[Union[ModuleType, Tuple[ModuleType, Dict]]]
+Module = Union[ModuleType, Tuple[ModuleType, Dict]]
+Modules = List[Module]
 """Type of modules handed to `paracrine.runner.run`"""
 
-TransmitModules = List[Union[str, Tuple[str, Dict]]]
+TransmitModule = Union[str, Tuple[str, Dict]]
+TransmitModules = List[TransmitModule]
 
 
 def runfunc(
     modules: Modules, name: str, arguments: Dict[str, Any] = {}, data: Dict = {}
 ) -> Dict[str, Any]:
     ret = {}
 
@@ -44,23 +46,23 @@
         if isinstance(module, ModuleType):
             run(module, {})
         else:
             run(module[0], module[1])
     return ret
 
 
-def maketransmit(modules: Modules) -> TransmitModules:
-    ret = []
-    for module in modules:
-        if isinstance(module, ModuleType):
-            ret.append(module.__name__)
-        else:
-            ret.append((module[0].__name__, module[1]))
+def maketransmit_single(module: Module) -> TransmitModule:
+    if isinstance(module, ModuleType):
+        return module.__name__
+    else:
+        return (module[0].__name__, module[1])
 
-    return ret
+
+def maketransmit(modules: Modules) -> TransmitModules:
+    return [maketransmit_single(module) for module in modules]
 
 
 def makereal(modules: TransmitModules) -> Modules:
     ret = []
     for module in modules:
         if isinstance(module, str):
             ret.append(importlib.import_module(module))
```

### Comparing `paracrine-0.0.8/paracrine/helpers/config.py` & `paracrine-0.0.9/paracrine/helpers/config.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/helpers/cron.py` & `paracrine-0.0.9/paracrine/helpers/cron.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/helpers/debian.py` & `paracrine-0.0.9/paracrine/helpers/debian.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/helpers/fs.py` & `paracrine-0.0.9/paracrine/helpers/fs.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/helpers/network.py` & `paracrine-0.0.9/paracrine/helpers/network.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/helpers/systemd.py` & `paracrine-0.0.9/paracrine/helpers/systemd.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/helpers/users.py` & `paracrine-0.0.9/paracrine/helpers/users.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/runner.py` & `paracrine-0.0.9/paracrine/runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,22 @@
 from typing import Any, Callable, Dict
 
 from mergedeep import merge
 from mitogen.core import Error, StreamError
 from mitogen.parent import Context, Router
 from mitogen.utils import run_with_router
 
-from .deps import Modules, TransmitModules, makereal, maketransmit, runfunc
+from .deps import (
+    Modules,
+    TransmitModules,
+    makereal,
+    maketransmit,
+    maketransmit_single,
+    runfunc,
+)
 from .helpers.config import (
     create_data,
     get_config,
     other_config_file,
     path_to_config_file,
     set_config,
     set_data,
@@ -112,30 +119,59 @@
                     merge(selector_config, per_node["selector"])
                     selector_config = dict(sorted(selector_config.items()))
                     set_file_contents(
                         config_path, json.dumps(selector_config, indent=2)
                     )
 
 
-def run(inventory_path: str, modules: Modules):
-    logging.basicConfig()
-    logging.root.setLevel(logging.INFO)
-    set_config(inventory_path)
-
-    needs_dependencies = list(modules)
+def generate_dependencies(modules: Modules):
+    tree = {}
+    mapping = {}
+    checked = []
+    needs_dependencies = list(modules) + [core]
+    modules = []
     while len(needs_dependencies) > 0:
-        new_dependencies = runfunc(needs_dependencies, "dependencies")
-        needs_dependencies = []
+        check = needs_dependencies.pop()
+        checked.append(check)
+        key = str(maketransmit_single(check))
+        tree[key] = []
+        mapping[key] = check
+        new_dependencies = runfunc([check], "dependencies")
         for item in new_dependencies.values():
             for new_dependency in item[0]:
-                if new_dependency in modules:
+                tree[key].append(new_dependency)
+                if new_dependency in needs_dependencies or new_dependency in checked:
                     continue
-                modules.insert(0, new_dependency)
                 needs_dependencies.append(new_dependency)
-    modules.insert(0, core)
+
+    count = 0
+    while len(checked) > 0:
+        count += 1
+        if count == 100:
+            raise Exception((modules, checked))
+        for key, value in tree.items():
+            mapped = mapping[key]
+            if mapped in modules:
+                continue
+            for dep in value:
+                if dep not in modules:
+                    break
+            else:
+                modules.append(mapped)
+                checked.remove(mapped)
+
+    return modules
+
+
+def run(inventory_path: str, modules: Modules):
+    logging.basicConfig()
+    logging.root.setLevel(logging.INFO)
+    set_config(inventory_path)
+
+    modules = generate_dependencies(modules)
 
     print("Running:")
     for module in maketransmit(modules):
         print(f"* {module}")
     print("")
 
     run_with_router(internal_runner, modules, "local", "run", "parse_return")
```

### Comparing `paracrine-0.0.8/paracrine/runners/aws.py` & `paracrine-0.0.9/paracrine/runners/aws.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/runners/certs.py` & `paracrine-0.0.9/paracrine/runners/certs.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/runners/core.py` & `paracrine-0.0.9/paracrine/runners/core.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/services/cockroachdb/__init__.py` & `paracrine-0.0.9/paracrine/services/cockroachdb/__init__.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/services/cockroachdb/certs.py` & `paracrine-0.0.9/paracrine/services/cockroachdb/certs.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/services/cockroachdb/common.py` & `paracrine-0.0.9/paracrine/services/cockroachdb/common.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/services/cockroachdb/init.py` & `paracrine-0.0.9/paracrine/services/cockroachdb/init.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from . import certs, node
 from .common import CERTS_DIR, HOME_DIR, cockroach_binary, local_node_ip
 
 options = {}
 
 
 def dependencies():
-    return [(node, options), (certs, options)]
+    return [(node, options), certs]
 
 
 def run():
     # FIXME: Can't make node start work in docker
     if in_docker() or not use_this_host("cockroach-init"):
         return
     COCKROACH_PORT = options.get("COCKROACH_PORT", 26257)
```

### Comparing `paracrine-0.0.8/paracrine/services/cockroachdb/node.py` & `paracrine-0.0.9/paracrine/services/cockroachdb/node.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/services/pleroma.py` & `paracrine-0.0.9/paracrine/services/pleroma.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,25 @@
     ]
 
 
 def run():
     LOCAL = build_config(core_config())
     adduser("pleroma", home_dir="/opt/pleroma")
     make_directory("/opt/pleroma", owner="pleroma")
-    # Taken from https://git.pleroma.social/pleroma/pleroma/-/pipelines?page=1&scope=branches&ref=stable
+    # Taken from https://git.pleroma.social/pleroma/pleroma/-/pipelines?page=1&scope=branches&ref=stable using amd64:archive
     res = download_and_unpack(
-        "https://git.pleroma.social/pleroma/pleroma/-/jobs/220705/artifacts/download?file_type=archive",
-        "8b4e2ab17362c7b0ed3ca685e19d578ad842ac00cde2db7d8c54dfd5a4e05891",
-        "pleroma-2.4.4.zip",
-        "/opt/pleroma-2.4.4",
+        "https://git.pleroma.social/pleroma/pleroma/-/jobs/234433/artifacts/download?file_type=archive",
+        "8ef0bea62671d39e60f9e08d13109a4c332c552a1f855184063353987d46c84a",
+        "pleroma-2.5.2.zip",
+        "/opt/pleroma-2.5.2",
     )
     release_changed = res["changed"]
 
     if release_changed:
-        run_command("cp -R /opt/pleroma-2.4.4/release/* /opt/pleroma")
+        run_command("cp -R /opt/pleroma-2.5.2/release/* /opt/pleroma")
         run_command("chown -R pleroma /opt/pleroma")
 
     make_directory("/var/lib/pleroma/uploads", owner="pleroma")
     make_directory("/var/lib/pleroma/static", owner="pleroma")
     set_file_contents_from_template("/var/lib/pleroma/static/robots.txt", "robots.txt")
     make_directory("/etc/pleroma", owner="pleroma")
     config_changes = set_file_contents_from_template(
```

### Comparing `paracrine-0.0.8/paracrine/services/postgresql.py` & `paracrine-0.0.9/paracrine/services/postgresql.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/services/redis/node.py` & `paracrine-0.0.9/paracrine/services/redis/node.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
     insert_or_replace,
     render_template,
     set_file_contents,
     set_file_contents_from_template,
 )
 from ...helpers.network import wireguard_ip
 from ...helpers.systemd import systemd_set
-from ...runners.core import wireguard_ip_for_machine_for
 from .. import wireguard
+from .common import get_master_ip
 
 options = {}
 
 
 def dependencies():
     return [wireguard]
 
 
 def run():
-    LOCAL = build_config(core_config())
     apt_install(["redis-sentinel", "redis-server"])
-    master_ip = wireguard_ip_for_machine_for("redis-master")
+    LOCAL = build_config(core_config())
     local_ip = wireguard_ip()
+    master_ip = get_master_ip()
     server_changes = set_file_contents_from_template(
         "/etc/redis/redis.conf",
         "redis.conf.j2",
         WIREGUARD_IP=local_ip,
         IS_MASTER=local_ip == master_ip,
         MASTER_IP=master_ip,
         REDIS_PASSWORD=LOCAL["REDIS_PASSWORD"],
```

### Comparing `paracrine-0.0.8/paracrine/services/wireguard/bootstrap.py` & `paracrine-0.0.9/paracrine/services/wireguard/bootstrap.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/services/wireguard/core.py` & `paracrine-0.0.9/paracrine/services/wireguard/core.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/templates/config.exs.j2` & `paracrine-0.0.9/paracrine/templates/config.exs.j2`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/templates/pleroma.nginx.j2` & `paracrine-0.0.9/paracrine/templates/pleroma.nginx.j2`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine/templates/redis-sentinel.conf.j2` & `paracrine-0.0.9/paracrine/templates/redis-sentinel.conf.j2`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.8/paracrine.egg-info/PKG-INFO` & `paracrine-0.0.9/paracrine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paracrine
-Version: 0.0.8
+Version: 0.0.9
 Summary: A system deployment tool
 Author-email: Tom Parker-Shemilt <palfrey@tevp.net>
 Project-URL: Homepage, https://github.com/palfrey/paracrine
 Project-URL: Bug Tracker, https://github.com/palfrey/paracrine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `paracrine-0.0.8/paracrine.egg-info/SOURCES.txt` & `paracrine-0.0.9/paracrine.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 paracrine/services/postgresql.py
 paracrine/services/cockroachdb/__init__.py
 paracrine/services/cockroachdb/certs.py
 paracrine/services/cockroachdb/common.py
 paracrine/services/cockroachdb/init.py
 paracrine/services/cockroachdb/node.py
 paracrine/services/redis/__init__.py
+paracrine/services/redis/common.py
 paracrine/services/redis/init.py
 paracrine/services/redis/node.py
 paracrine/services/wireguard/__init__.py
 paracrine/services/wireguard/bootstrap.py
 paracrine/services/wireguard/common.py
 paracrine/services/wireguard/core.py
 paracrine/templates/certbot_requirements.txt
@@ -49,8 +50,9 @@
 paracrine/templates/cron.j2
 paracrine/templates/pleroma.nginx.j2
 paracrine/templates/redis-sentinel.conf.j2
 paracrine/templates/redis.conf.j2
 paracrine/templates/robots.txt
 paracrine/templates/setup_db.psql.j2
 paracrine/templates/wg.conf.j2
+tests/test_dependencies.py
 tests/test_ssh.py
```

### Comparing `paracrine-0.0.8/pyproject.toml` & `paracrine-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "paracrine"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Tom Parker-Shemilt", email="palfrey@tevp.net" },
 ]
 description = "A system deployment tool"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `paracrine-0.0.8/tests/test_ssh.py` & `paracrine-0.0.9/tests/test_ssh.py`

 * *Files identical despite different names*

