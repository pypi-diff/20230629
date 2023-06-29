# Comparing `tmp/e2e_cli-0.9.9.8.tar.gz` & `tmp/e2e_cli-0.9.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2e_cli-0.9.9.8.tar", last modified: Wed Apr 19 10:42:06 2023, max compression
+gzip compressed data, was "e2e_cli-0.9.9.9.tar", last modified: Wed Jun 28 12:56:58 2023, max compression
```

## Comparing `e2e_cli-0.9.9.8.tar` & `e2e_cli-0.9.9.9.tar`

### file list

```diff
@@ -1,105 +1,120 @@
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.011713 e2e_cli-0.9.9.8/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/LICENSE
--rw-r--r--   0 aman       (501) staff       (20)       31 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/MANIFEST.in
--rw-r--r--   0 aman       (501) staff       (20)     2570 2023-04-19 10:42:06.011517 e2e_cli-0.9.9.8/PKG-INFO
--rw-r--r--   0 aman       (501) staff       (20)     6237 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/README.md
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:05.996072 e2e_cli-0.9.9.8/e2e_cli/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/__init__.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:05.998082 e2e_cli-0.9.9.8/e2e_cli/auto_scaling/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/auto_scaling/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     4068 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/auto_scaling/auto_scaling.py
--rw-r--r--   0 aman       (501) staff       (20)     2315 2023-04-19 08:31:18.000000 e2e_cli-0.9.9.8/e2e_cli/auto_scaling/autoscaling_routing.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:05.998475 e2e_cli-0.9.9.8/e2e_cli/bucket_store/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/bucket_store/__init__.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:05.998904 e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_actions/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_actions/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     8272 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_actions/bucket_actions.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:05.999486 e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_crud/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_crud/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     4074 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_crud/bucket_storage.py
--rw-r--r--   0 aman       (501) staff       (20)     5074 2023-04-19 08:32:45.000000 e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_routing.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:05.999962 e2e_cli-0.9.9.8/e2e_cli/cdn/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/cdn/__init__.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.000383 e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_actions/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_actions/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     3135 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_actions/cdn_action.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.000791 e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_crud/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_crud/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     3698 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_crud/cdn.py
--rw-r--r--   0 aman       (501) staff       (20)     3748 2023-04-19 08:32:53.000000 e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_routing.py
--rw-r--r--   0 aman       (501) staff       (20)     6481 2023-04-19 08:39:16.000000 e2e_cli-0.9.9.8/e2e_cli/commands_routing.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.001624 e2e_cli-0.9.9.8/e2e_cli/config/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/config/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     6580 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/config/config.py
--rw-r--r--   0 aman       (501) staff       (20)     3208 2023-04-19 08:35:40.000000 e2e_cli-0.9.9.8/e2e_cli/config/config_routing.py
--rw-r--r--   0 aman       (501) staff       (20)      372 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/config/config_service.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.003341 e2e_cli-0.9.9.8/e2e_cli/core/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/core/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     2249 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/core/alias_service.py
--rw-r--r--   0 aman       (501) staff       (20)     1978 2023-04-19 07:52:48.000000 e2e_cli-0.9.9.8/e2e_cli/core/constants.py
--rw-r--r--   0 aman       (501) staff       (20)     3639 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/core/error_logs_service.py
--rw-r--r--   0 aman       (501) staff       (20)     1797 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/core/help_messages.py
--rw-r--r--   0 aman       (501) staff       (20)     3263 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/core/helper_service.py
--rw-r--r--   0 aman       (501) staff       (20)      657 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/core/py_manager.py
--rw-r--r--   0 aman       (501) staff       (20)      455 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/core/request_service.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.003734 e2e_cli-0.9.9.8/e2e_cli/dbaas/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/dbaas/__init__.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.004159 e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_actions/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_actions/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     8272 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_actions/dbaas_action.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.004779 e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_crud/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_crud/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     5221 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_crud/dbaas.py
--rw-r--r--   0 aman       (501) staff       (20)     8922 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_crud/dbaas_services.py
--rw-r--r--   0 aman       (501) staff       (20)     5658 2023-04-19 08:33:02.000000 e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_routing.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.005194 e2e_cli-0.9.9.8/e2e_cli/docs/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/docs/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     7055 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/docs/e2e_cli.1
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.005577 e2e_cli-0.9.9.8/e2e_cli/image/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/image/__init__.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.005961 e2e_cli-0.9.9.8/e2e_cli/image/image_crud/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/image/image_crud/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     3345 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/image/image_crud/image.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.006389 e2e_cli-0.9.9.8/e2e_cli/image/image_listing/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/image/image_listing/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     1365 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/image/image_listing/image_list.py
--rw-r--r--   0 aman       (501) staff       (20)     2989 2023-04-19 08:31:18.000000 e2e_cli-0.9.9.8/e2e_cli/image/image_routing.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.007405 e2e_cli-0.9.9.8/e2e_cli/loadbalancer/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/loadbalancer/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     4406 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/loadbalancer/lb.py
--rw-r--r--   0 aman       (501) staff       (20)     1745 2023-04-19 08:31:18.000000 e2e_cli-0.9.9.8/e2e_cli/loadbalancer/lb_routing.py
--rw-r--r--   0 aman       (501) staff       (20)    42484 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/loadbalancer/lb_services.py
--rw-r--r--   0 aman       (501) staff       (20)    15202 2023-04-19 08:59:40.000000 e2e_cli-0.9.9.8/e2e_cli/main.py
--rw-r--r--   0 aman       (501) staff       (20)      459 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/man_display.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.007947 e2e_cli-0.9.9.8/e2e_cli/node/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/node/__init__.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.008369 e2e_cli-0.9.9.8/e2e_cli/node/node_actions/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/node/node_actions/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     8128 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/node/node_actions/node_action.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.009005 e2e_cli-0.9.9.8/e2e_cli/node/node_crud/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/node/node_crud/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     6680 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/node/node_crud/node.py
--rw-r--r--   0 aman       (501) staff       (20)     3666 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/node/node_crud/node_listing_service.py
--rw-r--r--   0 aman       (501) staff       (20)     5809 2023-04-19 08:32:06.000000 e2e_cli-0.9.9.8/e2e_cli/node/node_routing.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.009441 e2e_cli-0.9.9.8/e2e_cli/volumes/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/volumes/__init__.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.009865 e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_actions/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_actions/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     1839 2023-04-18 10:34:31.000000 e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_actions/volumes_action.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.010458 e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_crud/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_crud/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     3930 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_crud/volumes.py
--rw-r--r--   0 aman       (501) staff       (20)     3406 2023-04-19 08:32:17.000000 e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_routing.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:06.011155 e2e_cli-0.9.9.8/e2e_cli/vpc/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/vpc/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     3510 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.8/e2e_cli/vpc/vpc.py
--rw-r--r--   0 aman       (501) staff       (20)     2722 2023-04-19 08:32:26.000000 e2e_cli-0.9.9.8/e2e_cli/vpc/vpc_routing.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-04-19 10:42:05.997356 e2e_cli-0.9.9.8/e2e_cli.egg-info/
--rw-r--r--   0 aman       (501) staff       (20)     2570 2023-04-19 10:42:05.000000 e2e_cli-0.9.9.8/e2e_cli.egg-info/PKG-INFO
--rw-r--r--   0 aman       (501) staff       (20)     2435 2023-04-19 10:42:05.000000 e2e_cli-0.9.9.8/e2e_cli.egg-info/SOURCES.txt
--rw-r--r--   0 aman       (501) staff       (20)        1 2023-04-19 10:42:05.000000 e2e_cli-0.9.9.8/e2e_cli.egg-info/dependency_links.txt
--rw-r--r--   0 aman       (501) staff       (20)       57 2023-04-19 10:42:05.000000 e2e_cli-0.9.9.8/e2e_cli.egg-info/entry_points.txt
--rw-r--r--   0 aman       (501) staff       (20)       40 2023-04-19 10:42:05.000000 e2e_cli-0.9.9.8/e2e_cli.egg-info/requires.txt
--rw-r--r--   0 aman       (501) staff       (20)        8 2023-04-19 10:42:05.000000 e2e_cli-0.9.9.8/e2e_cli.egg-info/top_level.txt
--rw-r--r--   0 aman       (501) staff       (20)       38 2023-04-19 10:42:06.011794 e2e_cli-0.9.9.8/setup.cfg
--rw-r--r--   0 aman       (501) staff       (20)      950 2023-04-19 10:41:10.000000 e2e_cli-0.9.9.8/setup.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.550171 e2e_cli-0.9.9.9/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/LICENSE
+-rw-r--r--   0 aman       (501) staff       (20)       31 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/MANIFEST.in
+-rw-r--r--   0 aman       (501) staff       (20)     2570 2023-06-28 12:56:58.549981 e2e_cli-0.9.9.9/PKG-INFO
+-rw-r--r--   0 aman       (501) staff       (20)     6237 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/README.md
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.522411 e2e_cli-0.9.9.9/e2e_cli/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/__init__.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.524627 e2e_cli-0.9.9.9/e2e_cli/add_on_services/
+-rw-r--r--   0 aman       (501) staff       (20)        1 2023-06-28 12:11:15.000000 e2e_cli-0.9.9.9/e2e_cli/add_on_services/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     1105 2023-06-28 12:45:57.000000 e2e_cli-0.9.9.9/e2e_cli/add_on_services/view_security_groups.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.526057 e2e_cli-0.9.9.9/e2e_cli/auto_scaling/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/auto_scaling/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     4334 2023-06-28 07:11:34.000000 e2e_cli-0.9.9.9/e2e_cli/auto_scaling/auto_scaling.py
+-rw-r--r--   0 aman       (501) staff       (20)     1637 2023-06-28 06:51:40.000000 e2e_cli-0.9.9.9/e2e_cli/auto_scaling/autoscaling_routing.py
+-rw-r--r--   0 aman       (501) staff       (20)     1122 2023-06-28 07:15:28.000000 e2e_cli-0.9.9.9/e2e_cli/auto_scaling/helpers.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.526699 e2e_cli-0.9.9.9/e2e_cli/bucket_store/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/bucket_store/__init__.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.527660 e2e_cli-0.9.9.9/e2e_cli/bucket_store/bucket_actions/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/bucket_store/bucket_actions/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     8106 2023-06-28 06:12:27.000000 e2e_cli-0.9.9.9/e2e_cli/bucket_store/bucket_actions/bucket_actions.py
+-rw-r--r--   0 aman       (501) staff       (20)     1883 2023-06-28 06:27:19.000000 e2e_cli-0.9.9.9/e2e_cli/bucket_store/bucket_actions/helpers.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.528691 e2e_cli-0.9.9.9/e2e_cli/bucket_store/bucket_crud/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/bucket_store/bucket_crud/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     3980 2023-06-28 06:07:49.000000 e2e_cli-0.9.9.9/e2e_cli/bucket_store/bucket_crud/bucket_storage.py
+-rw-r--r--   0 aman       (501) staff       (20)     1092 2023-06-28 06:26:15.000000 e2e_cli-0.9.9.9/e2e_cli/bucket_store/bucket_crud/helpers.py
+-rw-r--r--   0 aman       (501) staff       (20)     2483 2023-06-27 12:10:42.000000 e2e_cli-0.9.9.9/e2e_cli/bucket_store/bucket_routing.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.529298 e2e_cli-0.9.9.9/e2e_cli/cdn/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/cdn/__init__.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.530243 e2e_cli-0.9.9.9/e2e_cli/cdn/cdn_actions/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/cdn/cdn_actions/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     3466 2023-06-28 10:56:40.000000 e2e_cli-0.9.9.9/e2e_cli/cdn/cdn_actions/cdn_action.py
+-rw-r--r--   0 aman       (501) staff       (20)     1044 2023-06-28 10:57:22.000000 e2e_cli-0.9.9.9/e2e_cli/cdn/cdn_actions/helpers.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.531328 e2e_cli-0.9.9.9/e2e_cli/cdn/cdn_crud/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/cdn/cdn_crud/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     3905 2023-06-28 10:54:58.000000 e2e_cli-0.9.9.9/e2e_cli/cdn/cdn_crud/cdn.py
+-rw-r--r--   0 aman       (501) staff       (20)      552 2023-06-28 10:55:53.000000 e2e_cli-0.9.9.9/e2e_cli/cdn/cdn_crud/helpers.py
+-rw-r--r--   0 aman       (501) staff       (20)     2406 2023-06-28 10:27:40.000000 e2e_cli-0.9.9.9/e2e_cli/cdn/cdn_routing.py
+-rw-r--r--   0 aman       (501) staff       (20)     7056 2023-06-28 12:31:08.000000 e2e_cli-0.9.9.9/e2e_cli/commands_routing.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.532682 e2e_cli-0.9.9.9/e2e_cli/config/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/config/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     6580 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/config/config.py
+-rw-r--r--   0 aman       (501) staff       (20)     3208 2023-04-19 08:35:40.000000 e2e_cli-0.9.9.9/e2e_cli/config/config_routing.py
+-rw-r--r--   0 aman       (501) staff       (20)      319 2023-06-28 08:34:25.000000 e2e_cli-0.9.9.9/e2e_cli/config/config_service.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.535287 e2e_cli-0.9.9.9/e2e_cli/core/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/core/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     2249 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/core/alias_service.py
+-rw-r--r--   0 aman       (501) staff       (20)     2084 2023-06-28 07:20:29.000000 e2e_cli-0.9.9.9/e2e_cli/core/constants.py
+-rw-r--r--   0 aman       (501) staff       (20)     3639 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/core/error_logs_service.py
+-rw-r--r--   0 aman       (501) staff       (20)     1795 2023-06-28 07:20:12.000000 e2e_cli-0.9.9.9/e2e_cli/core/help_messages.py
+-rw-r--r--   0 aman       (501) staff       (20)     4481 2023-06-28 06:00:56.000000 e2e_cli-0.9.9.9/e2e_cli/core/helper_service.py
+-rw-r--r--   0 aman       (501) staff       (20)      657 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/core/py_manager.py
+-rw-r--r--   0 aman       (501) staff       (20)      541 2023-06-28 12:43:38.000000 e2e_cli-0.9.9.9/e2e_cli/core/request_service.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.535872 e2e_cli-0.9.9.9/e2e_cli/dbaas/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/dbaas/__init__.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.536795 e2e_cli-0.9.9.9/e2e_cli/dbaas/dbaas_actions/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/dbaas/dbaas_actions/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     7580 2023-06-28 09:46:57.000000 e2e_cli-0.9.9.9/e2e_cli/dbaas/dbaas_actions/dbaas_action.py
+-rw-r--r--   0 aman       (501) staff       (20)     1494 2023-06-28 10:03:39.000000 e2e_cli-0.9.9.9/e2e_cli/dbaas/dbaas_actions/helpers.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.537754 e2e_cli-0.9.9.9/e2e_cli/dbaas/dbaas_crud/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/dbaas/dbaas_crud/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     5220 2023-06-23 18:37:21.000000 e2e_cli-0.9.9.9/e2e_cli/dbaas/dbaas_crud/dbaas.py
+-rw-r--r--   0 aman       (501) staff       (20)     8877 2023-06-28 09:51:05.000000 e2e_cli-0.9.9.9/e2e_cli/dbaas/dbaas_crud/dbaas_services.py
+-rw-r--r--   0 aman       (501) staff       (20)     2871 2023-06-28 08:54:50.000000 e2e_cli-0.9.9.9/e2e_cli/dbaas/dbaas_routing.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.538370 e2e_cli-0.9.9.9/e2e_cli/docs/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/docs/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     7055 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/docs/e2e_cli.1
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.538938 e2e_cli-0.9.9.9/e2e_cli/image/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/image/__init__.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.539829 e2e_cli-0.9.9.9/e2e_cli/image/image_crud/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/image/image_crud/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)      976 2023-06-28 07:51:45.000000 e2e_cli-0.9.9.9/e2e_cli/image/image_crud/helpers.py
+-rw-r--r--   0 aman       (501) staff       (20)     3159 2023-06-28 07:52:47.000000 e2e_cli-0.9.9.9/e2e_cli/image/image_crud/image.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.540423 e2e_cli-0.9.9.9/e2e_cli/image/image_listing/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/image/image_listing/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     1365 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/image/image_listing/image_list.py
+-rw-r--r--   0 aman       (501) staff       (20)     1833 2023-06-28 08:04:15.000000 e2e_cli-0.9.9.9/e2e_cli/image/image_routing.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.541829 e2e_cli-0.9.9.9/e2e_cli/loadbalancer/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/loadbalancer/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     4687 2023-06-28 11:03:59.000000 e2e_cli-0.9.9.9/e2e_cli/loadbalancer/lb.py
+-rw-r--r--   0 aman       (501) staff       (20)     1019 2023-06-28 11:06:42.000000 e2e_cli-0.9.9.9/e2e_cli/loadbalancer/lb_routing.py
+-rw-r--r--   0 aman       (501) staff       (20)    42484 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/loadbalancer/lb_services.py
+-rw-r--r--   0 aman       (501) staff       (20)    15321 2023-06-28 12:28:43.000000 e2e_cli-0.9.9.9/e2e_cli/main.py
+-rw-r--r--   0 aman       (501) staff       (20)      459 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/man_display.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.542823 e2e_cli-0.9.9.9/e2e_cli/node/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/node/__init__.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.544232 e2e_cli-0.9.9.9/e2e_cli/node/node_actions/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/node/node_actions/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)      473 2023-06-27 10:10:09.000000 e2e_cli-0.9.9.9/e2e_cli/node/node_actions/helpers.py
+-rw-r--r--   0 aman       (501) staff       (20)     7419 2023-06-27 11:29:31.000000 e2e_cli-0.9.9.9/e2e_cli/node/node_actions/node_action.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.545795 e2e_cli-0.9.9.9/e2e_cli/node/node_crud/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/node/node_crud/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     2275 2023-06-27 09:33:52.000000 e2e_cli-0.9.9.9/e2e_cli/node/node_crud/helpers.py
+-rw-r--r--   0 aman       (501) staff       (20)     5895 2023-06-28 12:10:26.000000 e2e_cli-0.9.9.9/e2e_cli/node/node_crud/node.py
+-rw-r--r--   0 aman       (501) staff       (20)     3604 2023-06-27 06:29:19.000000 e2e_cli-0.9.9.9/e2e_cli/node/node_crud/node_listing_service.py
+-rw-r--r--   0 aman       (501) staff       (20)     2175 2023-06-28 11:57:11.000000 e2e_cli-0.9.9.9/e2e_cli/node/node_routing.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.546314 e2e_cli-0.9.9.9/e2e_cli/volumes/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/volumes/__init__.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.546844 e2e_cli-0.9.9.9/e2e_cli/volumes/volumes_actions/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/volumes/volumes_actions/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     1839 2023-04-18 10:34:31.000000 e2e_cli-0.9.9.9/e2e_cli/volumes/volumes_actions/volumes_action.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.548286 e2e_cli-0.9.9.9/e2e_cli/volumes/volumes_crud/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/volumes/volumes_crud/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)      148 2023-06-28 11:27:49.000000 e2e_cli-0.9.9.9/e2e_cli/volumes/volumes_crud/constants.py
+-rw-r--r--   0 aman       (501) staff       (20)     1095 2023-06-28 11:34:14.000000 e2e_cli-0.9.9.9/e2e_cli/volumes/volumes_crud/helpers.py
+-rw-r--r--   0 aman       (501) staff       (20)     4042 2023-06-28 11:39:52.000000 e2e_cli-0.9.9.9/e2e_cli/volumes/volumes_crud/volumes.py
+-rw-r--r--   0 aman       (501) staff       (20)     2878 2023-06-28 11:37:11.000000 e2e_cli-0.9.9.9/e2e_cli/volumes/volumes_routing.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.549532 e2e_cli-0.9.9.9/e2e_cli/vpc/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-04-10 10:10:01.000000 e2e_cli-0.9.9.9/e2e_cli/vpc/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)      758 2023-06-28 08:05:54.000000 e2e_cli-0.9.9.9/e2e_cli/vpc/helpers.py
+-rw-r--r--   0 aman       (501) staff       (20)     3755 2023-06-28 12:41:24.000000 e2e_cli-0.9.9.9/e2e_cli/vpc/vpc.py
+-rw-r--r--   0 aman       (501) staff       (20)     1795 2023-06-28 08:05:03.000000 e2e_cli-0.9.9.9/e2e_cli/vpc/vpc_routing.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2023-06-28 12:56:58.524030 e2e_cli-0.9.9.9/e2e_cli.egg-info/
+-rw-r--r--   0 aman       (501) staff       (20)     2570 2023-06-28 12:56:58.000000 e2e_cli-0.9.9.9/e2e_cli.egg-info/PKG-INFO
+-rw-r--r--   0 aman       (501) staff       (20)     2960 2023-06-28 12:56:58.000000 e2e_cli-0.9.9.9/e2e_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 aman       (501) staff       (20)        1 2023-06-28 12:56:58.000000 e2e_cli-0.9.9.9/e2e_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 aman       (501) staff       (20)       57 2023-06-28 12:56:58.000000 e2e_cli-0.9.9.9/e2e_cli.egg-info/entry_points.txt
+-rw-r--r--   0 aman       (501) staff       (20)       40 2023-06-28 12:56:58.000000 e2e_cli-0.9.9.9/e2e_cli.egg-info/requires.txt
+-rw-r--r--   0 aman       (501) staff       (20)        8 2023-06-28 12:56:58.000000 e2e_cli-0.9.9.9/e2e_cli.egg-info/top_level.txt
+-rw-r--r--   0 aman       (501) staff       (20)       38 2023-06-28 12:56:58.550254 e2e_cli-0.9.9.9/setup.cfg
+-rw-r--r--   0 aman       (501) staff       (20)      950 2023-06-28 12:56:31.000000 e2e_cli-0.9.9.9/setup.py
```

### Comparing `e2e_cli-0.9.9.8/PKG-INFO` & `e2e_cli-0.9.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2e_cli
-Version: 0.9.9.8
+Version: 0.9.9.9
 Summary: This a E2E CLI tool for myAccount
 Home-page: UNKNOWN
 Author: Sajal&Aman@E2E_Networks_Ltd
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `e2e_cli-0.9.9.8/README.md` & `e2e_cli-0.9.9.9/README.md`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.8/e2e_cli/auto_scaling/auto_scaling.py` & `e2e_cli-0.9.9.9/e2e_cli/auto_scaling/auto_scaling.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,94 +1,100 @@
 from prettytable import PrettyTable
 
 from e2e_cli.core.py_manager import Py_version_manager
 from e2e_cli.core.request_service import Request
 from e2e_cli.core.alias_service import get_user_cred
 from e2e_cli.core.helper_service import Checks
-from e2e_cli.core.constants import BASE_URL
+from e2e_cli.auto_scaling.helpers import autoscaling_crud_helper
 
 
-class autoscaling_Crud:
+class AutoscalingCrud:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
-        if(get_user_cred(kwargs['alias'])):
-            self.API_key=get_user_cred(kwargs['alias'])[1]
-            self.Auth_Token=get_user_cred(kwargs['alias'])[0]
-            self.possible=True
+        if (get_user_cred(kwargs['alias'])):
+            self.API_key = get_user_cred(kwargs['alias'])[1]
+            self.Auth_Token = get_user_cred(kwargs['alias'])[0]
+            self.possible = True
         else:
-            self.possible=False
-        
+            self.possible = False
+
+    def caller(self, method):
+        function_set = {"create": self.create_autoscaling,
+                        "delete": self.delete_autoscaling,
+                        "list": self.list_autoscaling
+                        }
+        return function_set.get(method)
+
 
     def create_autoscaling(self):
         Py_version_manager.py_print("Currently not integrated")
-        # my_payload= {}  
+        # my_payload= {}
         # autoscaling_name=Py_version_manager.py_input("input name of your new autoscaling : ")
         # while(Checks.autoscaling_name_validity(autoscaling_name)):
         #         autoscaling_name=Py_version_manager.py_input("Only following chars are supported: lowercase letters (a-z) or numbers(0-9)  Re-enter : ")
 
         # API_key=self.API_key
         # Auth_Token=self.Auth_Token
-        # url =  BASE_URL+"myaccount/api/v1/storage/autoscalings/"+ autoscaling_name +"/?apikey="+API_key+"&location=Delhi"
+        # url =  "myaccount/api/v1/storage/autoscalings/"+ autoscaling_name +"/?apikey="+API_key+"&location=Delhi"
         # req="POST"
         # status=Request(url, Auth_Token, my_payload, req).response.json()
-               
+
         # if Checks.status_result(status, req):
         #     try:
         #         x = PrettyTable()
         #         x.field_names = ["ID", "Name", "Created at"]
         #         x.add_row([status['data']['id'], status['data']['name'], status['data']['created_at']])
         #         Py_version_manager.py_print(x)
         #     except Exception as e:
         #               Checks.show_json(status, e)
         #               return
-                  
-        # Checks.show_json(status)    
+
+        # Checks.show_json(status)
 
 
     def delete_autoscaling(self):
-        my_payload={}
-        autoscaling_id=Checks.take_input(self.kwargs["inputs"], "autoscaling_id")
-        while(not Checks.is_int(autoscaling_id)):
-                autoscaling_id=Py_version_manager.py_input("Only integers allowed ")
-        
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/scaler/scalegroups/"+ autoscaling_id +"?apikey="+API_key
-        req="DELETE"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
-
-        if Checks.status_result(status,req):
-                        Py_version_manager.py_print("autoscaling Successfully deleted")
-                        Py_version_manager.py_print("use following command -> e2e_cli <alias> autoscaling list to check if autoscaling has been deleted")
-        
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        autoscaling_crud_helper(self.kwargs["inputs"])
+        my_payload = {}
+        autoscaling_id = self.kwargs["inputs"]["autoscaling_id"]
+        url = "myaccount/api/v1/scaler/scalegroups/" + \
+            str(autoscaling_id) + "?apikey="+API_key
+        req = "DELETE"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
+
+        Checks.show_json(status)
+        Py_version_manager.py_print(
+            "use following command -> e2e_cli <alias> autoscaling list to check if autoscaling has been deleted")
+        # if Checks.status_result(status,req):
+        #                 Py_version_manager.py_print("autoscaling Successfully deleted")
+        #                 Py_version_manager.py_print("use following command -> e2e_cli <alias> autoscaling list to check if autoscaling has been deleted")
         # if('json' in self.kwargs["inputs"]):
         #     Checks.show_json(status)
-        Checks.show_json(status) 
 
 
     def list_autoscaling(self):
-        my_payload={}
-        API_key= self.API_key  
-        Auth_Token= self.Auth_Token 
-        url =  BASE_URL+"myaccount/api/v1/scaler/scalegroups?apikey="+ API_key+"&location=Delhi"
-        req="GET"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
-        
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        my_payload = {}
+        url = "myaccount/api/v1/scaler/scalegroups?apikey=" + API_key+"&location=Delhi"
+        req = "GET"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
+
+        Checks.status_result(status)
+        Checks.show_json(status)
         # if Checks.status_result(status, req):
         #         Py_version_manager.py_print("Your autoscalings : ")
         #         try:
         #             list=status['data']
         #             i=1
         #             x = PrettyTable()
         #             x.field_names = ["index", "ID", "Policy", "Name", "Max_nodes", "Min_nodes"]
         #             for element in list:
         #                 x.add_row([i, element['id'], element['policy'], element['name'], element['max_nodes'], element["min_nodes"]])
         #                 i = i+1
         #             Py_version_manager.py_print(x)
         #         except Exception as e:
         #               Py_version_manager.py_print("Errors : ", e)
-                        
+
         # if('json' in self.kwargs["inputs"]):
         #             Checks.show_json(status)
-        Checks.status_result(status)
-        Checks.show_json(status) 
-
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/auto_scaling/autoscaling_routing.py` & `e2e_cli-0.9.9.9/e2e_cli/auto_scaling/autoscaling_routing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import subprocess
 
 from e2e_cli.core.py_manager import Py_version_manager
-from e2e_cli.auto_scaling.auto_scaling import autoscaling_Crud
+from e2e_cli.auto_scaling.auto_scaling import AutoscalingCrud
 
 class autoscaling_Routing:
     def __init__(self, arguments):
         self.arguments = arguments
         
         
     def route(self, Parsing_Errors):
@@ -16,34 +16,23 @@
                 Py_version_manager.py_print("")
             subprocess.call(['e2e_cli', 'autoscaling', '-h'])
 
         # elif (self.arguments.args.autoscaling_commands is not None) and (self.arguments.args.action is not None):
         #       Py_version_manager.py_print("Only one action at a time !!")
 
         elif(self.arguments.args.autoscaling_commands is not None):
-            auto_scaling_operations = autoscaling_Crud(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
+            auto_scaling_operations = AutoscalingCrud(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
             if(auto_scaling_operations.possible):
-
-                if self.arguments.args.autoscaling_commands == 'create':
-                                try:
-                                    auto_scaling_operations.create_autoscaling()
-                                except KeyboardInterrupt:
-                                    Py_version_manager.py_print(" ")
-
-                elif self.arguments.args.autoscaling_commands == 'delete':
-                                try:
-                                    auto_scaling_operations.delete_autoscaling()
-                                except KeyboardInterrupt:
-                                    Py_version_manager.py_print(" ")
-                                
-                elif self.arguments.args.autoscaling_commands == 'list':
-                                try:
-                                    auto_scaling_operations.list_autoscaling()
-                                except KeyboardInterrupt:
-                                    Py_version_manager.py_print(" ")
-           
+                operation = auto_scaling_operations.caller(
+                    self.arguments.args.autoscaling_commands)
+                if operation:
+                    try:
+                        operation()
+                    except KeyboardInterrupt:
+                        Py_version_manager.py_print(" ")
+        
             
         else:
             Py_version_manager.py_print("command not found")
             if(Parsing_Errors):
                 Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_actions/bucket_actions.py` & `e2e_cli-0.9.9.9/e2e_cli/bucket_store/bucket_actions/bucket_actions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,213 +1,217 @@
 from prettytable import PrettyTable
 import json
 
 from e2e_cli.core.py_manager import Py_version_manager
 from e2e_cli.core.request_service import Request
 from e2e_cli.core.alias_service import get_user_cred
 from e2e_cli.core.helper_service import Checks
-from e2e_cli.core.constants import BASE_URL
+from e2e_cli.bucket_store.bucket_actions import helpers
 
 
 class BucketActions:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
-        if(get_user_cred(kwargs['alias'])):
-            self.API_key=get_user_cred(kwargs['alias'])[1]
-            self.Auth_Token=get_user_cred(kwargs['alias'])[0]
-            self.possible=True
+        if (get_user_cred(kwargs['alias'])):
+            self.API_key = get_user_cred(kwargs['alias'])[1]
+            self.Auth_Token = get_user_cred(kwargs['alias'])[0]
+            self.possible = True
         else:
-            self.possible=False
+            self.possible = False
+
+    def caller(self, method):
+        function_set = {"enable_versioning": self.enable_versioning,
+                        "disable_versioning": self.disable_versioning,
+                        "create_key": self.create_key,
+                        "delete_key": self.delete_key,
+                        "list_key": self.list_key,
+                        "lock_key": self.lock_key,
+                        "unlock_key": self.unlock_key,
+                        "add_permission": self.add_permission
+                        }
+        return function_set.get(method)
 
 
     def enable_versioning(self):
-        bucket_name=Checks.take_input(self.kwargs["inputs"], "bucket_name")
-        while(Checks.bucket_name_validity(bucket_name)):
-                bucket_name=Py_version_manager.py_input("Only following chars are supported: lowercase letters (a-z) or numbers(0-9)  Re-enter : ")
-        my_payload= json.dumps({
-                        "bucket_name": bucket_name,
-                        "new_versioning_state": "Enabled"
-                }) 
-        
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/storage/bucket_versioning/"+ bucket_name +"/?apikey="+API_key+"&location=Delhi"
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.bucket_versioning_helper(self.kwargs["inputs"])
+        bucket_name = self.kwargs["inputs"]["bucket_name"]
+        my_payload = json.dumps({
+            "bucket_name": bucket_name,
+            "new_versioning_state": "Enabled"
+        })
+        url = "myaccount/api/v1/storage/bucket_versioning/" + \
+            bucket_name + "/?apikey="+API_key+"&location=Delhi"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
         Checks.status_result(status)
         Checks.show_json(status)
 
 
     def disable_versioning(self):
-        bucket_name=Checks.take_input(self.kwargs["inputs"], "bucket_name")
-        while(Checks.bucket_name_validity(bucket_name)):
-                bucket_name=Py_version_manager.py_input("Only following chars are supported: lowercase letters (a-z) or numbers(0-9)  Re-enter : ")
-        my_payload= json.dumps({
-                        "bucket_name": bucket_name,
-                        "new_versioning_state": "Disabled"
-                }) 
-        
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/storage/bucket_versioning/"+ bucket_name +"/?apikey="+API_key+"&location=Delhi"
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.bucket_versioning_helper(self.kwargs["inputs"])
+        bucket_name = self.kwargs["inputs"]["bucket_name"]
+        my_payload = json.dumps({
+            "bucket_name": bucket_name,
+            "new_versioning_state": "Disabled"
+        })
+        url = "myaccount/api/v1/storage/bucket_versioning/" + \
+            bucket_name + "/?apikey="+API_key+"&location=Delhi"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
         Checks.status_result(status)
         Checks.show_json(status)
 
 
     def create_key(self):
-        key_name=Checks.take_input(self.kwargs["inputs"], "key_name")
-        while(Checks.bucket_name_validity(key_name)):
-                key_name=Py_version_manager.py_input("Only following chars are supported: lowercase letters (a-z) or numbers(0-9)  Re-enter : ")
-        my_payload= json.dumps({
-                        "tag": key_name
-                }) 
-        
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/storage/core/users/?apikey="+API_key+"&location=Delhi"
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.bucket_create_key(self.kwargs["inputs"])
+        key_name = self.kwargs["inputs"]["key_name"]
+        my_payload = json.dumps({
+            "tag": key_name
+        })
+        url = "myaccount/api/v1/storage/core/users/?apikey="+API_key+"&location=Delhi"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
-        if(Checks.status_result(status)):
-              Py_version_manager.py_print("Key Created successfully")
+        if (Checks.status_result(status)):
+            Py_version_manager.py_print("Key Created successfully")
 
         Checks.show_json(status)
-    
+
 
     def delete_key(self):
-        access_key=Checks.take_input(self.kwargs["inputs"], "access_key")
-        my_payload= {} 
-        query= dict()
-        query['access_key']=access_key
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/storage/core/users/?apikey="+API_key+"&location=Delhi"
-        req="DELETE"
-        status=Request(url, Auth_Token, my_payload, req, query=query).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.bucket_delete_key(self.kwargs["inputs"])
+        access_key = self.kwargs["inputs"]["access_key"]
+        my_payload = {}
+        query = dict()
+        query['access_key'] = access_key
+        url = "myaccount/api/v1/storage/core/users/?apikey="+API_key+"&location=Delhi"
+        req = "DELETE"
+        status = Request(url, Auth_Token, my_payload,
+                         req, query=query).response.json()
 
-        if(Checks.status_result(status)):
-              Py_version_manager.py_print("Key deleted successfully")
+        if (Checks.status_result(status)):
+            Py_version_manager.py_print("Key deleted successfully")
 
         Checks.show_json(status)
 
-    
+
     def list_key(self):
-        my_payload={}
-        API_key= self.API_key  
-        Auth_Token= self.Auth_Token 
-        url =  BASE_URL+"myaccount/api/v1/storage/core/list/users/?apikey="+ API_key+"&location=Delhi"
-        req="GET"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
-        
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        my_payload = {}
+        url = "myaccount/api/v1/storage/core/list/users/?apikey=" + API_key+"&location=Delhi"
+        req = "GET"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
+
         # if Checks.status_result(status, req):
         #         Py_version_manager.py_print("Your Keys : ")
         #         try:
         #             list=status['data']
         #             i=1
         #             x = PrettyTable()
         #             x.field_names = ["index", "ID", "Name", "access_key" ]
         #             for element in list:
         #                 x.add_row([i, element['id'], element['tag'], element['access_key']])
         #                 i = i+1
         #             Py_version_manager.py_print(x)
         #         except Exception as e:
         #               Checks.show_json(status, e)
-        #               return    
+        #               return
         Checks.status_result(status)
         Checks.show_json(status)
 
 
     def lock_key(self):
-        key_id=Checks.take_input(self.kwargs["inputs"], "key_id")
-        while(not Checks.is_int(key_id)):
-                key_id=Py_version_manager.py_input("Only integer allowed ")
-        my_payload= json.dumps({
-                "disabled": True,
-                "id": key_id
-                }) 
-        
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/storage/core/users/?apikey="+API_key+"&location=Delhi"
-        req="PUT"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
-        
-        if(Checks.status_result(status)):
-              Py_version_manager.py_print("Key locked")
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.bucket_lock_unlock_key(self.kwargs["inputs"])
+        key_id = self.kwargs["inputs"]["key_id"]
+        my_payload = json.dumps({
+            "disabled": True,
+            "id": key_id
+        })
+        url = "myaccount/api/v1/storage/core/users/?apikey="+API_key+"&location=Delhi"
+        req = "PUT"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
+        if (Checks.status_result(status)):
+            Py_version_manager.py_print("Key locked")
         Checks.show_json(status)
 
-    
-    def unlock_key(self):
-        key_id=Checks.take_input(self.kwargs["inputs"], "key_id")
-        while(not Checks.is_int(key_id)):
-                key_id=Py_version_manager.py_input("Only integer allowed ")
-        my_payload= json.dumps({
-                "disabled": False,
-                "id": key_id
-                }) 
-        
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/storage/core/users/?apikey="+API_key+"&location=Delhi"
-        req="PUT"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
 
-        if(Checks.status_result(status)):
-              Py_version_manager.py_print("Key unlocked")
+    def unlock_key(self):
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.bucket_lock_unlock_key(self.kwargs["inputs"])
+        key_id = self.kwargs["inputs"]["key_id"]
+        my_payload = json.dumps({
+            "disabled": False,
+            "id": key_id
+        })
+        url = "myaccount/api/v1/storage/core/users/?apikey="+API_key+"&location=Delhi"
+        req = "PUT"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
+        if (Checks.status_result(status)):
+            Py_version_manager.py_print("Key unlocked")
         Checks.show_json(status)
-    
+
 
     def add_permission(self):
-        bucket_name=Checks.take_input(self.kwargs["inputs"], "bucket_name")
-        while(Checks.bucket_name_validity(bucket_name)):
-                bucket_name=Py_version_manager.py_input("Only following chars are supported: lowercase letters (a-z) or numbers(0-9)  Re-enter : ")
-        my_payload= json.dumps({
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        bucket_name = self.kwargs["inputs"]["bucket_name"]
+        my_payload = json.dumps({
             "role_name": "Bucket Admin",
             "users": [
-            {
-                "access_key": Py_version_manager.py_input("input access key (Alphanumeric): "),
-                "disabled": False,
-                "email": "",
-                "id": Py_version_manager.py_input("enter bucket id "),
-                "is_default": False,
-                "my_account_id": None,
-                "secret_key": None,
-                "tag": Py_version_manager.py_input("name "),
-                "user_name": Py_version_manager.py_input("username ")
-            }
+                {
+                    "access_key": Py_version_manager.py_input("input access key (Alphanumeric): "),
+                    "disabled": False,
+                    "email": "",
+                    "id": Py_version_manager.py_input("enter bucket id "),
+                    "is_default": False,
+                    "my_account_id": None,
+                    "secret_key": None,
+                    "tag": Py_version_manager.py_input("name "),
+                    "user_name": Py_version_manager.py_input("username ")
+                }
             ]
-            })
-        query= dict()
-        query['bucket_name']=bucket_name
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/storage/bucket_perms/?apikey="+API_key+"&location=Delhi"
-        req="PUT"
-        status=Request(url, Auth_Token, my_payload, req, query=query).response.json()
-
-        if(Checks.status_result(status)):
-              Py_version_manager.py_print("Key deleted successfully")
-              
+        })
+        query = dict()
+        query['bucket_name'] = bucket_name
+        url = "myaccount/api/v1/storage/bucket_perms/?apikey="+API_key+"&location=Delhi"
+        req = "PUT"
+        status = Request(url, Auth_Token, my_payload,
+                         req, query=query).response.json()
+
+        if (Checks.status_result(status)):
+            Py_version_manager.py_print("Premission added successfully")
         Checks.show_json(status)
 
 
     def remove_permission(self):
-        access_key=Checks.take_input(self.kwargs["inputs"], "access_key")
-        my_payload= {} 
-        query= dict()
-        query['access_key']=access_key
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/storage/core/users/?apikey="+API_key+"&location=Delhi"
-        req="DELETE"
-        status=Request(url, Auth_Token, my_payload, req, query=query).response.json()
-
-        if(Checks.status_result(status)):
-              Py_version_manager.py_print("Key deleted successfully")
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.bucket_remove_permission(self.kwargs["inputs"])
+        bucket_name = self.kwargs["inputs"]["bucket_name"]
+        bucket_permission_id = self.kwargs["inputs"]["bucket_permission_id"]
+        my_payload = {}
+        query = dict()
+        query['access_key'] = bucket_name
+        url = f"myaccount/api/v1/storage/bucket_perm/{bucket_permission_id}/?apikey={API_key}"
+        req = "DELETE"
+        status = Request(url, Auth_Token, my_payload,
+                         req, query=query).response.json()
 
+        if (Checks.status_result(status)):
+            Py_version_manager.py_print("Premission removed")
         Checks.show_json(status)
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/bucket_store/bucket_crud/bucket_storage.py` & `e2e_cli-0.9.9.9/e2e_cli/bucket_store/bucket_crud/bucket_storage.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,92 @@
 from prettytable import PrettyTable
 
 from e2e_cli.core.py_manager import Py_version_manager
 from e2e_cli.core.request_service import Request
 from e2e_cli.core.alias_service import get_user_cred
 from e2e_cli.core.helper_service import Checks
-from e2e_cli.core.constants import BASE_URL
+from e2e_cli.bucket_store.bucket_crud.helpers import bucket_crud_helper
 
 
-class bucketCrud:
+class BucketCrud:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
-        if(get_user_cred(kwargs['alias'])):
-            self.API_key=get_user_cred(kwargs['alias'])[1]
-            self.Auth_Token=get_user_cred(kwargs['alias'])[0]
-            self.possible=True
+        if (get_user_cred(kwargs['alias'])):
+            self.API_key = get_user_cred(kwargs['alias'])[1]
+            self.Auth_Token = get_user_cred(kwargs['alias'])[0]
+            self.possible = True
         else:
-            self.possible=False
-        
+            self.possible = False
+
+    def caller(self, method):
+        function_set = {"create": self.create_bucket,
+                        "delete": self.delete_bucket,
+                        "list": self.list_bucket
+                        }
+        return function_set.get(method)
+
 
     def create_bucket(self):
         Py_version_manager.py_print("Creating")
-        my_payload= {}  
-        bucket_name=Checks.take_input(self.kwargs["inputs"], "bucket_name")
-        while(Checks.bucket_name_validity(bucket_name)):
-                bucket_name=Py_version_manager.py_input("Only following chars are supported: lowercase letters (a-z) or numbers(0-9)  Re-enter : ")
-
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/storage/buckets/"+ bucket_name +"/?apikey="+API_key+"&location=Delhi"
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
-               
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        bucket_crud_helper(self.kwargs["inputs"])
+        my_payload = {}
+        bucket_name = self.kwargs["inputs"]["bucket_name"]
+        url = "myaccount/api/v1/storage/buckets/" + \
+            bucket_name + "/?apikey="+API_key+"&location=Delhi"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
+
+        Checks.status_result(status)
+        Checks.show_json(status)
         # if Checks.status_result(status, req):
         #     try:
         #         x = PrettyTable()
         #         x.field_names = ["ID", "Name", "Created at"]
         #         x.add_row([status['data']['id'], status['data']['name'], status['data']['created_at']])
         #         Py_version_manager.py_print(x)
         #     except Exception as e:
         #             Py_version_manager.py_print("Errors : ", e)
-                  
+
         # if('json' in self.kwargs["inputs"]):
-        #     Checks.show_json(status) 
-        Checks.status_result(status)
-        Checks.show_json(status)   
+        #     Checks.show_json(status)
+        
 
 
     def delete_bucket(self):
-        my_payload={}
-        bucket_name=Checks.take_input(self.kwargs["inputs"], "bucket_name")
-        while(Checks.bucket_name_validity(bucket_name)):
-                bucket_name=Py_version_manager.py_input("Only following chars are supported: lowercase letters (a-z) or numbers(0-9)  Re-enter : ")
-        
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/storage/buckets/"+ bucket_name +"/?apikey="+API_key+"&location=Delhi"
-        req="DELETE"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
-
-        if Checks.status_result(status,req):
-                        Py_version_manager.py_print("Bucket Successfully deleted")
-                        Py_version_manager.py_print("use following command -> e2e_cli <alias> bucket list to check if bucket has been deleted")
-        
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        bucket_crud_helper(self.kwargs["inputs"])
+        my_payload = {}
+        bucket_name = self.kwargs["inputs"]["bucket_name"]
+        url = "myaccount/api/v1/storage/buckets/" + \
+            bucket_name + "/?apikey="+API_key+"&location=Delhi"
+        req = "DELETE"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
+
+        if Checks.status_result(status, req):
+            Py_version_manager.py_print("Bucket Successfully deleted")
+            Py_version_manager.py_print(
+                "use following command -> e2e_cli <alias> bucket list to check if bucket has been deleted")
+        Checks.show_json(status)
         # if('json' in self.kwargs["inputs"]):
         #     Checks.show_json(status)
-        Checks.show_json(status)
+        
 
     def list_bucket(self):
-        my_payload={}
-        API_key= self.API_key  
-        Auth_Token= self.Auth_Token 
-        url =  BASE_URL+"myaccount/api/v1/storage/buckets/?apikey="+ API_key+"&location=Delhi"
-        req="GET"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
-        
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        my_payload = {}
+        url = "myaccount/api/v1/storage/buckets/?apikey=" + API_key+"&location=Delhi"
+        req = "GET"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
+
+        Checks.status_result(status)
+        Checks.show_json(status)
         # if Checks.status_result(status, req):
         #         Py_version_manager.py_print("Your Buckets : ")
         #         try:
         #             list=status['data']
         #             i=1
         #             x = PrettyTable()
         #             x.field_names = ["index", "ID", "Name", "Created at", "bucket size"]
@@ -86,11 +95,7 @@
         #                 i = i+1
         #             Py_version_manager.py_print(x)
         #         except Exception as e:
         #             Py_version_manager.py_print("Errors : ", e)
 
         # if('json' in self.kwargs["inputs"]):
         #     Checks.show_json(status)
-        Checks.status_result(status)
-        Checks.show_json(status)
-    
-
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_crud/cdn.py` & `e2e_cli-0.9.9.9/e2e_cli/volumes/volumes_crud/volumes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,105 @@
 from prettytable import PrettyTable
+import json
 
 from e2e_cli.core.py_manager import Py_version_manager
 from e2e_cli.core.request_service import Request
 from e2e_cli.core.alias_service import get_user_cred
 from e2e_cli.core.helper_service import Checks
-from e2e_cli.core.constants import BASE_URL
+from e2e_cli.volumes.volumes_crud import helpers
+from e2e_cli.volumes.volumes_crud.constants import VOLUME_IOPS
 
 
-class cdn_Crud:
+class VolumesCrud:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
         if(get_user_cred(kwargs['alias'])):
             self.API_key=get_user_cred(kwargs['alias'])[1]
             self.Auth_Token=get_user_cred(kwargs['alias'])[0]
             self.possible=True
         else:
             self.possible=False
-        
+    
+    def caller(self, method):
+        function_set = {"create": self.create_volumes,
+                        "delete": self.delete_volumes,
+                        "list": self.list_volumes
+                        }
+        return function_set.get(method)
+
+
+    def create_volumes(self):
+        Py_version_manager.py_print("Creating")
+        API_key=self.API_key
+        Auth_Token=self.Auth_Token
+        helpers.create_volumes_helper(self.kwargs["inputs"])
+        my_payload= json.dumps({
+            "name":self.kwargs["inputs"]["name"],
+            "size": self.kwargs["inputs"]["size"],
+            "iops": VOLUME_IOPS[self.kwargs["inputs"]["size"]]
+        })
+        url =  "myaccount/api/v1/block_storage/?apikey="+API_key+"&location=Delhi"
+        req="POST"
+        status=Request(url, Auth_Token, my_payload, req).response.json()
 
-    def create_cdn(self):
-        Py_version_manager.py_print("Currently not integrated")
-        # my_payload= {}  
-        # cdn_name=Py_version_manager.py_input("input name of your new cdn : ")
-        # while(Checks.cdn_name_validity(cdn_name)):
-        #         cdn_name=Py_version_manager.py_input("Only following chars are supported: lowercase letters (a-z) or numbers(0-9)  Re-enter : ")
-
-        # API_key=self.API_key
-        # Auth_Token=self.Auth_Token
-        # url =  BASE_URL+"myaccount/api/v1/storage/cdns/"+ cdn_name +"/?apikey="+API_key+"&location=Delhi"
-        # req="POST"
-        # status=Request(url, Auth_Token, my_payload, req).response.json()
-               
+        Checks.status_result(status)
+        Checks.show_json(status)      
         # if Checks.status_result(status, req):
         #     try:
         #         x = PrettyTable()
-        #         x.field_names = ["ID", "Name", "Created at"]
-        #         x.add_row([status['data']['id'], status['data']['name'], status['data']['created_at']])
+        #         x.field_names = ["block_storage_id", "name"]
+        #         x.add_row([status['data']['block_storage_id'], status['data']['image_name']])
         #         Py_version_manager.py_print(x)
         #     except Exception as e:
         #               Checks.show_json(status, e)
         #               return
                   
-        # Checks.show_json(status)    
+        # if('json' in self.kwargs["inputs"]):
+        #     Checks.show_json(status)      
 
 
-    def delete_cdn(self):
-        my_payload={}
-        query=dict()
-        query['domain_id']=Checks.take_input(self.kwargs["inputs"], "domain_id")
+    def delete_volumes(self):
         API_key=self.API_key
         Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/cdn/distributions/?apikey="+API_key
+        helpers.delete_volumes_helper(self.kwargs["inputs"])
+        my_payload={}
+        blockstorage_id=self.kwargs["inputs"]["blockstorage_id"]
+        url =  "myaccount/api/v1/block_storage/"+blockstorage_id+"/?apikey="+API_key+"&location=Delhi"
         req="DELETE"
-        status=Request(url, Auth_Token, my_payload, req, query=query).response.json()
+        status=Request(url, Auth_Token, my_payload, req).response.json()
 
         if Checks.status_result(status,req):
-                        Py_version_manager.py_print("CDN Successfully deleted")
-                        Py_version_manager.py_print("use following command -> e2e_cli <alias> cdn list to check if cdn has been deleted")
-        
+                        Py_version_manager.py_print("volume Successfully deleted")
+                        Py_version_manager.py_print("use following command -> e2e_cli <alias> volumes list to check if volumes has been deleted")
         Checks.show_json(status)
 
 
-    def list_cdn(self):
-        my_payload={}
+    def list_volumes(self):
         API_key= self.API_key  
         Auth_Token= self.Auth_Token 
-        url =  BASE_URL+"myaccount/api/v1/cdn/distributions/?apikey="+ API_key
+        my_payload={}
+        url =  "myaccount/api/v1/block_storage/?apikey="+ API_key+"&location=Delhi"
         req="GET"
         status=Request(url, Auth_Token, my_payload, req).response.json()
         
+        Checks.status_result(status)
+        Checks.show_json(status)
         # if Checks.status_result(status, req):
-        #         Py_version_manager.py_print("Your cdns : ")
+        #         Py_version_manager.py_print("Your volumess : ")
         #         try:
         #             list=status['data']
         #             i=1
         #             x = PrettyTable()
-        #             x.field_names = ["index", "ID", "user_domain_name", "Created at", "domain_id"]
+        #             x.field_names = ["index", "name", "block_id", "status"]
         #             for element in list:
-        #                 x.add_row([i, element['id'], element['user_domain_name'], element['created_at'], element['domain_id']])
+        #                 x.add_row([i, element['name'], element['block_id'], element["status"]])
         #                 i = i+1
         #             Py_version_manager.py_print(x)
         #         except Exception as e:
         #             Py_version_manager.py_print("Errors : ", e)
-                    
+
         # if('json' in self.kwargs["inputs"]):
-        #     Checks.show_json(status)
-        Checks.status_result(status)
-        Checks.show_json(status)     
+        #     Checks.show_json(status) 
+         
+
+
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/cdn/cdn_routing.py` & `e2e_cli-0.9.9.9/e2e_cli/bucket_store/bucket_routing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,87 +1,59 @@
 import subprocess
 
 from e2e_cli.core.py_manager import Py_version_manager
-from e2e_cli.cdn.cdn_crud.cdn import cdn_Crud
-from e2e_cli.cdn.cdn_actions.cdn_action import cdnActions
+from e2e_cli.bucket_store.bucket_crud.bucket_storage import BucketCrud
+from e2e_cli.bucket_store.bucket_actions.bucket_actions import BucketActions
 
-class cdn_Routing:
+class BucketRouting:
     def __init__(self, arguments):
         self.arguments = arguments
         
         
     def route(self, Parsing_Errors):
-        if (self.arguments.args.action is None) and (self.arguments.args.cdn_commands is None):
+        if (self.arguments.args.bucket_commands is None) and (self.arguments.args.action is None):
             if(Parsing_Errors):
                 Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
                 Py_version_manager.py_print("")
-            subprocess.call(['e2e_cli', 'cdn', '-h'])
+            subprocess.call(['e2e_cli', 'bucket', '-h'])
 
 
-        elif (self.arguments.args.cdn_commands is not None) and (self.arguments.args.action is not None):
+        elif (self.arguments.args.bucket_commands is not None) and (self.arguments.args.action is not None):
               Py_version_manager.py_print("Only one action at a time !!")
 
 
-        elif(self.arguments.args.cdn_commands is not None):
-            cdn_operations = cdn_Crud(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
-            if(cdn_operations.possible):
-
-                if self.arguments.args.cdn_commands == 'create':
-                        try:
-                            cdn_operations.create_cdn()
-                        except KeyboardInterrupt:
-                            Py_version_manager.py_print(" ")
-
-                elif self.arguments.args.cdn_commands == 'delete':
-                        try:
-                            cdn_operations.delete_cdn()
-                        except KeyboardInterrupt:
-                            Py_version_manager.py_print(" ")
-                        
-                elif self.arguments.args.cdn_commands == 'list':
-                        try:
-                            cdn_operations.list_cdn()
-                        except KeyboardInterrupt:
-                            Py_version_manager.py_print(" ")
+        elif(self.arguments.args.bucket_commands is not None):
+            bucket_operations = BucketCrud(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
+            if(bucket_operations.possible):
+                operation = bucket_operations.caller(
+                    self.arguments.args.bucket_commands)
+                if (operation):
+                    try:
+                        operation()
+                    except KeyboardInterrupt:
+                        Py_version_manager.py_print(" ")
 
 
         elif(self.arguments.args.action is not None):
-            cdn_operations = cdnActions(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
-            if(cdn_operations.possible):
-                
-                if self.arguments.args.action == "enable_cdn":
-                        try:
-                            cdn_operations.enable_cdn()
-                        except KeyboardInterrupt:
-                            Py_version_manager.py_print(" ")
-
-                elif self.arguments.args.action == "disable_cdn":
-                        try:
-                            cdn_operations.disable_cdn()
-                        except KeyboardInterrupt:
-                            Py_version_manager.py_print(" ")
-                
-                elif self.arguments.args.action == "cdn_monitoring":
-                        try:
-                            cdn_operations.cdn_monitoring()
-                        except KeyboardInterrupt:
-                            Py_version_manager.py_print(" ")
-
-                elif self.arguments.args.action == "cdn_bandwidth_usage":
-                        try:
-                            cdn_operations.cdn_bandwidth_usage()
-                        except KeyboardInterrupt:
-                            Py_version_manager.py_print(" ")
-                
+            bucket_operations=BucketActions(alias=self.arguments.args.alias, inputs=self.arguments.inputs)     
+            if(bucket_operations.possible):
+                operation = bucket_operations.caller(
+                    self.arguments.args.action)
+                if (operation):
+                    try:
+                        operation()
+                    except KeyboardInterrupt:
+                        Py_version_manager.py_print(" ")
+
                 else:
                     Py_version_manager.py_print("command not found")
                     if(Parsing_Errors):
                         Py_version_manager.py_print("Parsing Errors :")
                         Py_version_manager.py_print(*Parsing_Errors, sep="\n")
-                
+
 
         else:
             Py_version_manager.py_print("command not found")
             if(Parsing_Errors):
                 Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/commands_routing.py` & `e2e_cli-0.9.9.9/e2e_cli/commands_routing.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from e2e_cli.bucket_store.bucket_routing import BucketRouting
 from e2e_cli.dbaas.dbaas_routing import DBaaSRouting
 from e2e_cli.image.image_routing import ImageRouting
 from e2e_cli.auto_scaling.autoscaling_routing import autoscaling_Routing
 from e2e_cli.cdn.cdn_routing import cdn_Routing
 from e2e_cli.vpc.vpc_routing import vpc_Routing
 from e2e_cli.volumes.volumes_routing import volumes_Routing
+
+from e2e_cli.add_on_services.view_security_groups import SecurityGroup
 from e2e_cli.man_display import man_page
 
 class CommandsRouting:
     def __init__(self, arguments):
         self.arguments = arguments
 
     def route(self, Parsing_Errors):
@@ -54,15 +56,26 @@
                                 # action_on_exception(e, self.arguments.args.alias, traceback.print_exc())
             else:
                 if(Parsing_Errors):
                     Py_version_manager.py_print("Parsing Errors :")
                     Py_version_manager.py_print(*Parsing_Errors, sep="\n")
                     Py_version_manager.py_print("")
                 subprocess.call(['e2e_cli', "alias","-h"])
-    
+
+
+        elif self.arguments.args.command == "security_groups":
+        # introduced this block for add_on_services like security group view 
+                try:
+                    sg_groups=SecurityGroup(alias=self.arguments.args.alias)
+                    if(sg_groups.possible):
+                          sg_groups.list_security_groups()
+                except Exception as e:
+                            if("debug" in self.arguments.inputs):
+                                Checks.manage_exception(e)
+
     
         else:
             if(self.arguments.args.alias=="default"):
                 Py_version_manager.py_print("Using default alias")
 
             if self.arguments.args.command == "node":
                 try:
@@ -123,15 +136,15 @@
                 try:
                     vpc_Routing(self.arguments).route(Parsing_Errors)
                 except Exception as e:
                             if("debug" in self.arguments.inputs):
                                 Checks.manage_exception(e)
                             # action_on_exception(e, self.arguments.args.alias, traceback.print_exc())  
 
-            elif self.arguments.args.command == "volumes":
+            elif self.arguments.args.command == "volume":
                 try:
                     volumes_Routing(self.arguments).route(Parsing_Errors)
                 except Exception as e:
                             if("debug" in self.arguments.inputs):
                                 Checks.manage_exception(e)
                             # action_on_exception(e, self.arguments.args.alias, traceback.print_exc())
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/config/config.py` & `e2e_cli-0.9.9.9/e2e_cli/config/config.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.8/e2e_cli/config/config_routing.py` & `e2e_cli-0.9.9.9/e2e_cli/config/config_routing.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.8/e2e_cli/core/alias_service.py` & `e2e_cli-0.9.9.9/e2e_cli/core/alias_service.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.8/e2e_cli/core/constants.py` & `e2e_cli-0.9.9.9/e2e_cli/core/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 # constant, reserved keywords
-RESERVES=["alias", "all", "config", "node", "bucket", "lb", "dbaas", "create", "get", "list", "update", "edit", "delete", "file", "doc", "help", "default"]
+RESERVES = ["alias", "all", "config", "node", "bucket", "lb", "dbaas", "create",
+            "get", "list", "update", "edit", "delete", "file", "doc", "help", "default"]
 
-#version
-packagke_version="e2e-cli/1.0.0 Python Linux/Mac/Windows"
+# version
+PACKAGE_VERSION = "e2e-cli/1.0.0 Python Linux/Mac/Windows"
 
-#package_info
-packagke_info=" A command line tool developed by E2E Networks Ltd. \n Used to access and manage my_account/e2e_cloud services from cmd/shell \n Published 1st April 2023"
+# package_info
+PACKAGE_INFO = " A command line tool developed by E2E Networks Ltd. \n Used to access and manage my_account/e2e_cloud services from cmd/shell \n Published 1st April 2023"
 
-#url for api request
-BASE_URL="https://api.e2enetworks.com/"
+# url for api request
+BASE_URL = "https://api.e2enetworks.com/"
 
 
 # for better error handeling, write --action options and related help strings here for argparser
 
-NODE_ACTIONS=["enable_recovery", "disable_recovery", "reinstall", "reboot", "power_on", "power_off", "rename_node", "lock_vm", "unlock_vm", "monitor"]
-NODE_ACTIONS_STR="""
+NODE_ACTIONS = ["enable_recovery", "disable_recovery", "reinstall", "reboot",
+                "power_on", "power_off", "rename_node", "lock_vm", "unlock_vm", "monitor"]
+NODE_ACTIONS_STR = """
         lock_vm
         unlock_vm
         reinstall
         reboot
         power_on
         power_off
         monitor
         rename_node
         enable_recovery
         disable_recovery
 """
 
-BUCKET_ACTIONS=["enable_versioning", "disable_versioning", "create_key", "delete_key", "list_key", "lock_key", "unlock_key", "add_permission"]
-BUCKET_ACTIONS_STR="""
+BUCKET_ACTIONS = ["enable_versioning", "disable_versioning", "create_key",
+                  "delete_key", "list_key", "lock_key", "unlock_key", "add_permission"]
+BUCKET_ACTIONS_STR = """
         enable_versioning
         disable_versioning
         create_key
         delete_key
         list_key
         lock_key
         unlock_key
         add_permission
 """
 
-DBAAS_ACTIONS=["take_snapshot", "reset_password", "stop_db", "start_db", "restart_db", "enable_backup", "disable_backup", "add_parameter_group", "remove_parameter_group", "add_vpc", "remove_vpc"]
-DBAAS_ACTIONS_STR="""
+DBAAS_ACTIONS = ["take_snapshot", "reset_password", "stop_db", "start_db", "restart_db", "enable_backup",
+                 "disable_backup", "add_parameter_group", "remove_parameter_group", "add_vpc", "remove_vpc"]
+DBAAS_ACTIONS_STR = """
         take_snapshot
         reset_password
         add_vpc
         remove_vpc
         stop_db
         start_db
         restart_db
         enable_backup
         disable_backup
         add_parameter_group
         remove_parameter_group
 """
 
-CDN_ACTIONS=["enable_cdn", "disable_cdn", "cdn_monitoring", "cdn_bandwidth_usage"]
-CDN_ACTIONS_STR="""
+CDN_ACTIONS = ["enable_cdn", "disable_cdn",
+               "cdn_monitoring", "cdn_bandwidth_usage"]
+CDN_ACTIONS_STR = """
         enable_cdn
         disable_cdn
         cdn_monitoring
         cdn_bandwidth_usage
 """
 
-VOLUMES_ACTIONS=[]
+VOLUMES_ACTIONS = []
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/core/error_logs_service.py` & `e2e_cli-0.9.9.9/e2e_cli/core/error_logs_service.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.8/e2e_cli/core/help_messages.py` & `e2e_cli-0.9.9.9/e2e_cli/core/help_messages.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,11 +41,11 @@
 
 
 
 # =========================
 # e2e pkg/ver-info functions
 # =========================
 def e2e_version_info():
-        Py_version_manager.py_print(constants.packagke_version)
+        Py_version_manager.py_print(constants.PACKAGE_VERSION)
 
 def e2e_pakage_info():
-        Py_version_manager.py_print(constants.packagke_info)
+        Py_version_manager.py_print(constants.PACKAGE_INFO)
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/core/py_manager.py` & `e2e_cli-0.9.9.9/e2e_cli/core/py_manager.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_actions/dbaas_action.py` & `e2e_cli-0.9.9.9/e2e_cli/dbaas/dbaas_actions/dbaas_action.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,205 +1,205 @@
 from prettytable import PrettyTable
 import json
 
 from e2e_cli.core.py_manager import Py_version_manager
 from e2e_cli.core.request_service import Request
 from e2e_cli.core.alias_service import get_user_cred
 from e2e_cli.core.helper_service import Checks
-from e2e_cli.core.constants import BASE_URL
+from e2e_cli.dbaas.dbaas_actions import helpers
 
 
 class DBaasAction:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
-        if(get_user_cred(kwargs['alias'])):
-            self.API_key=get_user_cred(kwargs['alias'])[1]
-            self.Auth_Token=get_user_cred(kwargs['alias'])[0]
-            self.possible=True
+        if (get_user_cred(kwargs['alias'])):
+            self.API_key = get_user_cred(kwargs['alias'])[1]
+            self.Auth_Token = get_user_cred(kwargs['alias'])[0]
+            self.possible = True
         else:
-            self.possible=False
+            self.possible = False
+
+    def caller(self, method):
+        function_set = {"take_snapshot": self.take_snapshot,
+                        "reset_password": self.reset_password,
+                        "stop_db": self.stop_db,
+                        "start_db": self.start_db,
+                        "restart_db": self.restart_db,
+                        "add_parameter_group": self.add_parameter_group,
+                        "remove_parameter_group": self.remove_parameter_group,
+                        "add_vpc": self.add_vpc,
+                        "remove_vpc": self.remove_vpc,
+                        "enable_backup": self.enable_backup,
+                        "disable_backup": self.disable_backup
+                        }
+        return function_set.get(method)
 
 
     def take_snapshot(self):
-        dbaas_id =Checks.take_input(self.kwargs["inputs"], "dbaas_id")
-        while(not Checks.is_int(dbaas_id )):
-                dbaas_id =Py_version_manager.py_input("Only integers : ")
-        my_payload= json.dumps({
-                "name": "sanap3"
-                })
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/rds/cluster/"+ dbaas_id +"/snapshot?apikey="+API_key
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.db_common_helper(self.kwargs["inputs"])
+        dbaas_id = self.kwargs["inputs"]["dbaas_id"]
+        my_payload = json.dumps({
+            "name": "sanap3"
+        })
+        url = f"myaccount/api/v1/rds/cluster/{dbaas_id}/snapshot?apikey={API_key}"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
         Checks.status_result(status)
         Checks.show_json(status)
 
 
     def reset_password(self):
-        dbaas_id =Checks.take_input(self.kwargs["inputs"], "dbaas_id")
-        while(not Checks.is_int(dbaas_id )):
-                dbaas_id =Py_version_manager.py_input("Only integers : ")
-        my_payload= json.dumps({
-                 "password": Checks.take_input(self.kwargs["inputs"], "new_password"),
-                 "username": Checks.take_input(self.kwargs["inputs"], "username")
-                })
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/rds/cluster/"+dbaas_id+"/reset-password/?apikey="+API_key
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.db_common_helper(self.kwargs["inputs"])
+        dbaas_id = self.kwargs["inputs"]["dbaas_id"]
+        my_payload = json.dumps({
+            "password": self.kwargs["inputs"]["new_password"],
+            "username": self.kwargs["inputs"]["username"]
+        })
+        url = f"myaccount/api/v1/rds/cluster/{dbaas_id}/reset-password/?apikey={API_key}"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
         Checks.status_result(status)
         Checks.show_json(status)
 
 
     def stop_db(self):
-        dbaas_id =Checks.take_input(self.kwargs["inputs"], "dbaas_id")
-        while(not Checks.is_int(dbaas_id )):
-                dbaas_id =Py_version_manager.py_input("Only integers : ")
-        my_payload= {}
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/rds/cluster/"+dbaas_id+"/shutdown?apikey="+API_key
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.db_common_helper(self.kwargs["inputs"])
+        dbaas_id = self.kwargs["inputs"]["dbaas_id"]
+        my_payload = {}
+        url = f"myaccount/api/v1/rds/cluster/{dbaas_id}/shutdown?apikey={API_key}"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
         Checks.status_result(status)
         Checks.show_json(status)
 
 
     def start_db(self):
-        dbaas_id =Checks.take_input(self.kwargs["inputs"], "dbaas_id")
-        while(not Checks.is_int(dbaas_id )):
-                dbaas_id =Py_version_manager.py_input("Only integers : ")
-        my_payload= {}
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/rds/cluster/"+dbaas_id+"/resume?apikey="+API_key
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.db_common_helper(self.kwargs["inputs"])
+        dbaas_id = self.kwargs["inputs"]["dbaas_id"]
+        my_payload = {}
+        url = f"myaccount/api/v1/rds/cluster/{dbaas_id}/resume?apikey={API_key}"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
         Checks.status_result(status)
         Checks.show_json(status)
 
-    
+
     def restart_db(self):
-        dbaas_id =Checks.take_input(self.kwargs["inputs"], "dbaas_id")
-        while(not Checks.is_int(dbaas_id )):
-                dbaas_id =Py_version_manager.py_input("Only integers : ")
-        my_payload= {}
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/rds/cluster/"+dbaas_id+"/restart?apikey="+API_key
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.db_common_helper(self.kwargs["inputs"])
+        dbaas_id = self.kwargs["inputs"]["dbaas_id"]
+        my_payload = {}
+        url = f"myaccount/api/v1/rds/cluster/{dbaas_id}/restart?apikey={API_key}"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
         Checks.status_result(status)
         Checks.show_json(status)
 
 
     def add_parameter_group(self):
-        dbaas_id =Checks.take_input(self.kwargs["inputs"], "dbaas_id")
-        while(not Checks.is_int(dbaas_id )):
-                dbaas_id =Py_version_manager.py_input("Only integers : ")
-        parameter_group_id =Checks.take_input(self.kwargs["inputs"], "parameter_group_id")
-        while(not Checks.is_int(parameter_group_id )):
-                parameter_group_id =Py_version_manager.py_input("Only integers : ")
-        my_payload= {}
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/rds/cluster/"+dbaas_id+"/parameter-group/"+parameter_group_id+"/add?apikey="+API_key
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.db_add_rempove_paramter(self.kwargs["inputs"])
+        dbaas_id = self.kwargs["inputs"]["dbaas_id"]
+        parameter_group_id = self.kwargs["inputs"]["parameter_group_id"]
+        my_payload = {}
+        url = f"myaccount/api/v1/rds/cluster/{dbaas_id}/parameter-group/{parameter_group_id}/add?apikey={API_key}"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
         Checks.status_result(status)
         Checks.show_json(status)
-    
+
 
     def remove_parameter_group(self):
-        dbaas_id =Checks.take_input(self.kwargs["inputs"], "dbaas_id")
-        while(not Checks.is_int(dbaas_id )):
-                dbaas_id =Py_version_manager.py_input("Only integers : ")
-        parameter_group_id =Checks.take_input(self.kwargs["inputs"], "parameter_group_id")
-        while(not Checks.is_int(parameter_group_id )):
-                parameter_group_id =Py_version_manager.py_input("Only integers : ")
-        my_payload= {}
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/rds/cluster/"+dbaas_id+"/parameter-group/"+parameter_group_id+"/detach?apikey="+API_key
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.db_add_rempove_paramter(self.kwargs["inputs"])
+        dbaas_id = self.kwargs["inputs"]["dbaas_id"]
+        parameter_group_id = self.kwargs["inputs"]["parameter_group_id"]
+        my_payload = {}
+        url = f"myaccount/api/v1/rds/cluster/{dbaas_id}/parameter-group/{parameter_group_id}/detach?apikey={API_key}"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
         Checks.status_result(status)
         Checks.show_json(status)
-    
+
 
     def add_vpc(self):
-        dbaas_id =Checks.take_input(self.kwargs["inputs"], "dbaas_id")
-        while(not Checks.is_int(dbaas_id )):
-                dbaas_id =Py_version_manager.py_input("Only integers : ")
-        my_payload= json.dumps({
-                   "action": "attach",
-                   "network_id": Checks.take_input(self.kwargs["inputs"], "network_id")
-                     })
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/rds/cluster/"+dbaas_id+"//vpc-attach/?apikey="+API_key
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.db_add_rempove_vpc(self.kwargs["inputs"])
+        dbaas_id = self.kwargs["inputs"]["dbaas_id"]
+        my_payload = json.dumps({
+            "action": "attach",
+            "network_id": self.kwargs["inputs"]["network_id"]
+        })
+        url = f"myaccount/api/v1/rds/cluster/{dbaas_id}//vpc-attach/?apikey={API_key}"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
         Checks.status_result(status)
         Checks.show_json(status)
 
 
     def remove_vpc(self):
-        dbaas_id =Checks.take_input(self.kwargs["inputs"], "dbaas_id")
-        while(not Checks.is_int(dbaas_id )):
-                dbaas_id =Py_version_manager.py_input("Only integers : ")
-        my_payload= json.dumps({
-                   "action": "detach",
-                   "network_id": Checks.take_input(self.kwargs["inputs"], "network_id")
-                     })
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/rds/cluster/"+dbaas_id+"/vpc-detach/?apikey="+API_key
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.db_add_rempove_vpc(self.kwargs["inputs"])
+        dbaas_id = self.kwargs["inputs"]["dbaas_id"]
+        my_payload = json.dumps({
+            "action": "detach",
+            "network_id": self.kwargs["inputs"]["network_id"]
+        })
+        url = f"myaccount/api/v1/rds/cluster/{dbaas_id}/vpc-detach/?apikey={API_key}"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
         Checks.status_result(status)
         Checks.show_json(status)
 
 
     def enable_backup(self):
-        dbaas_id =Checks.take_input(self.kwargs["inputs"], "dbaas_id")
-        while(not Checks.is_int(dbaas_id )):
-                dbaas_id =Py_version_manager.py_input("Only integers : ")
-        my_payload= json.dumps({
-                 "access_key": Checks.take_input(self.kwargs["inputs"], "access_key"),
-                 "bucket_location": Checks.take_input(self.kwargs["inputs"], "bucket_location"),
-                 "secret_key": Checks.take_input(self.kwargs["inputs"], "secret_key")
-                    })
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/rds/cluster/"+dbaas_id+"/enable-backup?apikey="+API_key
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.db_enable_backup(self.kwargs["inputs"])
+        dbaas_id = self.kwargs["inputs"]["dbaas_id"]
+        my_payload = json.dumps({
+            "access_key": self.kwargs["inputs"]["access_key"],
+            "bucket_location": self.kwargs["inputs"]["bucket_location"],
+            "secret_key": self.kwargs["inputs"]["secret_key"]
+        })
+        url = f"myaccount/api/v1/rds/cluster/{dbaas_id}/enable-backup?apikey={API_key}"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
         Checks.status_result(status)
         Checks.show_json(status)
 
 
     def disable_backup(self):
-        dbaas_id =Checks.take_input(self.kwargs["inputs"], "dbaas_id")
-        while(not Checks.is_int(dbaas_id )):
-                dbaas_id =Py_version_manager.py_input("Only integers : ")
-        my_payload= {}
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/rds/cluster/"+dbaas_id+"/disable-backup?apikey="+API_key
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.db_common_helper(self.kwargs["inputs"])
+        dbaas_id = self.kwargs["inputs"]["dbaas_id"]
+        my_payload = {}
+        url = f"myaccount/api/v1/rds/cluster/{dbaas_id}/disable-backup?apikey={API_key}"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
         Checks.status_result(status)
         Checks.show_json(status)
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_crud/dbaas.py` & `e2e_cli-0.9.9.9/e2e_cli/dbaas/dbaas_crud/dbaas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from prettytable import PrettyTable
 
 from e2e_cli.core.py_manager import Py_version_manager
 from e2e_cli.dbaas.dbaas_crud.dbaas_services import DBaaSServices
 from e2e_cli.core.helper_service import Checks
 
-class DBaaSClass:
+class DBaaSCrud:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
     def list_dbaas(self):
         alias = self.kwargs["alias"]
         dbaas_services_object = DBaaSServices(alias)
         dbaas_service_response_object = dbaas_services_object.all_dbaas()
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/dbaas/dbaas_crud/dbaas_services.py` & `e2e_cli-0.9.9.9/e2e_cli/dbaas/dbaas_crud/dbaas_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self.alias_service_object = AliasServices(alias)
 
     def all_dbaas(self):
         api_key_credentials_object = self.alias_service_object.get_api_credentials()
         if api_key_credentials_object["message"] == "Invalid alias provided":
             return api_key_credentials_object
         else:
-            url =  BASE_URL+"myaccount/api/v1/rds/cluster/?apikey=" + \
+            url =  "myaccount/api/v1/rds/cluster/?apikey=" + \
                   api_key_credentials_object["api_credentials"]["api_key"] + "&location=Delhi"
             payload = {}
             Auth_Token= api_key_credentials_object["api_credentials"]["api_auth_token"]
 
             response = json.loads(Request(req="GET", url=url,  Auth_Token=Auth_Token, payload=payload).response.content)
 
             return {"dbaas_api_response": response,
@@ -37,15 +37,15 @@
         if not password.islower() and not password.isupper() and len(password)>=16 and bool(re.search(r'\d', password)) and \
                 any(not c.isalnum() for c in password):
             return False
         else:
             return True
         
     def select_a_software(self, api_key, api_auth_token):
-        url =  BASE_URL+"myaccount/api/v1/rds/plans/?apikey=" + api_key
+        url =  "myaccount/api/v1/rds/plans/?apikey=" + api_key
         payload = {}
         Auth_Token= api_auth_token
         response =  Request(req="GET", url=url, Auth_Token=Auth_Token, payload=payload).response.json()
         if 'responseCode' in response:
             if "No client" in response["message"]:
                 Py_version_manager.py_print("No Client found for this api credentials")
                 return "/" 
@@ -58,15 +58,15 @@
         while(not Checks.is_int(software_id) or not 0<int(software_id)<=len(software_engines)):
             Py_version_manager.py_print("Please select one of above only")
             software_id = Py_version_manager.py_input(": ")
         software_id=int(software_id)
         return software_engines[software_id-1]["id"]
     
     def select_a_template(self, software_id, api_key, api_auth_token):
-        url =  BASE_URL+"myaccount/api/v1/rds/plans/?apikey=" + api_key + "&software_id=" + str(software_id)
+        url =  "myaccount/api/v1/rds/plans/?apikey=" + api_key + "&software_id=" + str(software_id)
         payload = {}
         Auth_Token= api_auth_token
         response =  Request(req="GET", url=url, Auth_Token=Auth_Token, payload=payload).response.json()
         template_engines = response["data"]["template_plans"]
         table = PrettyTable(["Template ID", "Template Name", "Template Price"])
         templates_id = 1
         for template_instance in template_engines:
@@ -105,15 +105,15 @@
             software_id = self.select_a_software(api_key_credentials_object["api_credentials"]["api_key"],
                                                  api_key_credentials_object["api_credentials"]["api_auth_token"])
             if software_id == '/':
                 return None
             else:
                 template_id = self.select_a_template(software_id, api_key_credentials_object["api_credentials"]["api_key"],
                                                     api_key_credentials_object["api_credentials"]["api_auth_token"])
-                url =  BASE_URL+"myaccount/api/v1/rds/cluster/?apikey=" + \
+                url =  "myaccount/api/v1/rds/cluster/?apikey=" + \
                     api_key_credentials_object["api_credentials"]["api_key"] + "&location=Delhi"
 
                 payload = json.dumps({
                     "database": {
                         "name": name_assigned_to_database,
                         "password": password_assigned_to_database,
                         "user": username_assigned_to_database
@@ -140,15 +140,15 @@
         choice = Py_version_manager.py_input("Do you still want to continue?(Y/N)")
         if choice.upper() == "Y":
             api_key_credentials_object = self.alias_service_object.get_api_credentials()
             if api_key_credentials_object["message"] == "Invalid alias provided":
                 return api_key_credentials_object
             else:
 
-                url =  BASE_URL+"myaccount/api/v1/rds/cluster/" + database_id + "/?apikey=" + \
+                url =  "myaccount/api/v1/rds/cluster/" + database_id + "/?apikey=" + \
                       api_key_credentials_object["api_credentials"]["api_key"]
 
                 payload = {}
             
                 Auth_Token= api_key_credentials_object["api_credentials"]["api_auth_token"]
                 response = Request(req="DELETE", url=url, Auth_Token=Auth_Token, payload=payload).response.json()
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/docs/e2e_cli.1` & `e2e_cli-0.9.9.9/e2e_cli/docs/e2e_cli.1`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.8/e2e_cli/image/image_crud/image.py` & `e2e_cli-0.9.9.9/e2e_cli/image/image_crud/image.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,91 +1,92 @@
 import json
 
 from e2e_cli.core.py_manager import Py_version_manager
 from e2e_cli.core.alias_service import get_user_cred
 from e2e_cli.core.request_service import Request
 from e2e_cli.core.helper_service import Checks
-from e2e_cli.core.constants import BASE_URL
+from e2e_cli.image.image_crud import helpers
 
 
-def response_output(status, req): 
+def response_output(status, req):
     Checks.status_result(status, req)
     Checks.show_json(status)
 
 
 class ImageCrud:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
-        if(get_user_cred(kwargs['alias'])):
-            self.API_key=get_user_cred(kwargs['alias'])[1]
-            self.Auth_Token=get_user_cred(kwargs['alias'])[0]
-            self.possible=True
+        if (get_user_cred(kwargs['alias'])):
+            self.API_key = get_user_cred(kwargs['alias'])[1]
+            self.Auth_Token = get_user_cred(kwargs['alias'])[0]
+            self.possible = True
         else:
-            self.possible=False
-    
+            self.possible = False
+
+    def caller(self, method):
+        function_set = {"create": self.create_image,
+                        "delete": self.delete_image,
+                        "list": self.list_image,
+                        "rename": self.rename_image
+                        }
+        return function_set.get(method)
+
 
     def create_image(self):
-        node_id = Checks.take_input(self.kwargs["inputs"], "node_id")
-        new_image_name= Checks.take_input(self.kwargs["inputs"], "new_image_name")
-        my_payload= json.dumps({
-                        "name": new_image_name,
-                        "type": "save_images"
-                }) 
-        
-        while(not Checks.is_int(node_id)):
-              node_id = Py_version_manager.py_input("please enter node id (integer only) ")
-        
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/nodes/"+ node_id +"/actions/?apikey="+API_key+"&location=Delhi"
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.create_image_helper(self.kwargs["inputs"])
+        node_id = self.kwargs["inputs"]["node_id"]
+        new_image_name = self.kwargs["inputs"]["image_name"]
+        my_payload = json.dumps({
+            "name": new_image_name,
+            "type": "save_images"
+        })
+        url = f"myaccount/api/v1/nodes/{node_id}/actions/?apikey={API_key}&location=Delhi"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
+
+        response_output(status, req)
 
-        response_output(status, req)                
-        
 
     def delete_image(self):
-        image_id = Checks.take_input(self.kwargs["inputs"], "image_id")
-        while(not Checks.is_int(image_id)):
-              image_id = Py_version_manager.py_input("please enter image id (integer only) ")
-        my_payload= json.dumps({
-                        "action_type": "delete_image"
-                }) 
-        
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/images/"+ image_id +"/?apikey="+API_key+"&location=Delhi"
-        req="POST"
-        if(Py_version_manager.py_input("Are you sure you want to delete : ").lower()=="y"):
-            status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.delete_image_helper(self.kwargs["inputs"])
+        image_id = self.kwargs["inputs"]["image_id"]
+        my_payload = json.dumps({
+            "action_type": "delete_image"
+        })
+        url = f"myaccount/api/v1/images/{image_id}/?apikey={API_key}&location=Delhi"
+        req = "POST"
+        if (Py_version_manager.py_input("Are you sure you want to delete : ").lower() == "y"):
+            status = Request(url, Auth_Token, my_payload, req).response.json()
 
         response_output(status, req)
 
 
     def rename_image(self):
-        image_id = Checks.take_input(self.kwargs["inputs"], "image_id")
-        while(not Checks.is_int(image_id)):
-              image_id = Py_version_manager.py_input("please enter image id (integer only) ")
-        new_name= Checks.take_input(self.kwargs["inputs"], "new_name")
-        my_payload= json.dumps({
-                        "name": new_name,
-                        "action_type": "rename"
-                }) 
-        
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/images/"+ image_id +"/?apikey="+API_key+"&location=Delhi"
-        req="POST"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        helpers.rename_image_helper(self.kwargs["inputs"])
+        image_id = self.kwargs["inputs"]["image_id"]
+        new_name = self.kwargs["inputs"]["new_name"]
+        my_payload = json.dumps({
+            "name": new_name,
+            "action_type": "rename"
+        })
+        url = f"myaccount/api/v1/images/{image_id}/?apikey={API_key}&location=Delhi"
+        req = "POST"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
         response_output(status, req)
 
 
     def list_image(self):
-        my_payload= {}
-        API_key=self.API_key
-        Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/images/saved-images/?apikey="+API_key+"&location=Delhi"
-        req= "GET"
-        status=Request(url, Auth_Token, my_payload, req).response.json()
+        my_payload = {}
+        API_key = self.API_key
+        Auth_Token = self.Auth_Token
+        url = "myaccount/api/v1/images/saved-images/?apikey="+API_key+"&location=Delhi"
+        req = "GET"
+        status = Request(url, Auth_Token, my_payload, req).response.json()
 
         response_output(status, req)
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/image/image_listing/image_list.py` & `e2e_cli-0.9.9.9/e2e_cli/image/image_listing/image_list.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.8/e2e_cli/image/image_routing.py` & `e2e_cli-0.9.9.9/e2e_cli/dbaas/dbaas_routing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 import subprocess
 
+from e2e_cli.dbaas.dbaas_crud.dbaas import DBaaSCrud
 from e2e_cli.core.py_manager import Py_version_manager
-from e2e_cli.image.image_crud.image import ImageCrud
-from e2e_cli.image.image_listing.image_list import ImageListing
+from e2e_cli.dbaas.dbaas_actions.dbaas_action import DBaasAction
 
-class ImageRouting:
+
+
+class DBaaSRouting:
     def __init__(self, arguments):
         self.arguments = arguments
-        
 
     def route(self, Parsing_Errors):
-        if (self.arguments.args.image_commands is None) and (self.arguments.args.list_by is None):
+        if (self.arguments.args.dbaas_commands is None) and (self.arguments.args.action is None):
             if(Parsing_Errors):
                 Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
                 Py_version_manager.py_print("")
-            subprocess.call(['e2e_cli', 'image', '-h'])
+            subprocess.call(['e2e_cli','dbaas', '-h'])
+
 
+        elif (self.arguments.args.dbaas_commands is not None) and (self.arguments.args.action is not None):
+              Py_version_manager.py_print("Only one action at a time !!")
 
-        elif (self.arguments.args.image_commands is not None) and (self.arguments.args.list_by is not None):
-            Py_version_manager.py_print("Only one action at a time !!")
 
+        elif (self.arguments.args.dbaas_commands is not None):
+            dbaas_class_object = DBaaSCrud(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
+
+            if self.arguments.args.dbaas_commands == 'create':
+                try:
+                    dbaas_class_object.create_dbaas()
+                except KeyboardInterrupt:
+                    Py_version_manager.py_print(" ")
+
+            elif self.arguments.args.dbaas_commands == 'list' or self.arguments.args.dbaas_commands == 'ls':
+                try:
+                    dbaas_class_object.list_dbaas()
+                except KeyboardInterrupt:
+                    Py_version_manager.py_print(" ")
+
+            elif self.arguments.args.dbaas_commands == 'delete':
+                try:
+                    dbaas_class_object.delete_dbaas_by_name()
+                except KeyboardInterrupt:
+                    Py_version_manager.py_print(" ")
+        
 
-        elif(self.arguments.args.image_commands is not None):
-            image_operations = ImageCrud(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
-            if(image_operations.possible):
-
-                if self.arguments.args.image_commands == 'create' or self.arguments.args.image_commands=="save":
-                        try:
-                           image_operations.create_image()
-                        except KeyboardInterrupt:
-                            Py_version_manager.py_print(" ")  
-                                    
-                elif self.arguments.args.image_commands == 'delete':
-                        try:
-                           image_operations.delete_image()
-                        except KeyboardInterrupt:
-                            Py_version_manager.py_print(" ")
-                                
-                elif self.arguments.args.image_commands == 'rename':
-                        try:
-                           image_operations.rename_image()
-                        except KeyboardInterrupt:
-                            Py_version_manager.py_print(" ")
-                                                        
-                elif self.arguments.args.image_commands == 'list':
-                        try: 
-                           image_operations.list_image()
-                        except KeyboardInterrupt:
-                            Py_version_manager.py_print(" ")
-                        
-        # elif self.arguments.args.list_by == 'image_type':
-        #     image_operations=ImageListing(alias=self.arguments.args.alias)     
-        #     if(image_operations.possible):
-        #                 try: 
-        #                    image_operations.all()
-        #                 except KeyboardInterrupt:
-        #                     Py_version_manager.py_print(" ")
+        elif(self.arguments.args.action is not None):
+            DBaas_operations=DBaasAction(alias=self.arguments.args.alias, inputs=self.arguments.inputs)     
+            if(DBaas_operations.possible):
+                operation = DBaas_operations.caller(
+                    self.arguments.args.action)
+                if operation:
+                    try:
+                        operation()
+                    except KeyboardInterrupt:
+                        Py_version_manager.py_print(" ")
+                
+                else:
+                    Py_version_manager.py_print("command not found")
+                    if(Parsing_Errors):
+                        Py_version_manager.py_print("Parsing Errors :")
+                        Py_version_manager.py_print(*Parsing_Errors, sep="\n")
+                
 
         else:
             Py_version_manager.py_print("command not found")
             if(Parsing_Errors):
                 Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/loadbalancer/lb.py` & `e2e_cli-0.9.9.9/e2e_cli/loadbalancer/lb.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 from e2e_cli.loadbalancer.lb_services import LBServices
 
 
 class LBClass:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
+    def caller(self, method):
+        function_set = {"create": self.create_lb,
+                        "delete": self.delete_lb,
+                        "list": self.list_lb,
+                        "edit": self.edit_lb
+                        }
+        return function_set.get(method)
+
+
     def list_lb(self):
         alias = self.kwargs["alias"]
         lb_services_object = LBServices(alias)
         lb_service_response_object = lb_services_object.all_lb()
         if lb_service_response_object["message"] == "Valid alias":
             lb_api_response_object = lb_service_response_object["lb_api_response"]
             if "code" in lb_api_response_object:
@@ -68,16 +77,15 @@
                 Py_version_manager.py_print("  Your instance have been deleted")
                 Py_version_manager.py_print(
                     "To check the state of the LB you can run e2e_cli lb list <alias> "
                 )
             elif lb_delete_response_object["message"] == "Aborted":
                 Py_version_manager.py_print(lb_delete_response_object["message"])
             elif lb_delete_response_object["code"] == 404:
-                Py_version_manager.py_print("" + lb_delete_response_object["message"])
-            
+                Py_version_manager.py_print("" + lb_delete_response_object["message"])     
 
 
     def edit_lb(self):
         return_val = self.list_lb()
         if return_val == 0:
             pass
         else:
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/loadbalancer/lb_routing.py` & `e2e_cli-0.9.9.9/e2e_cli/loadbalancer/lb_routing.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,32 +15,15 @@
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
                 Py_version_manager.py_print("")
             subprocess.call(['e2e_cli', 'lb', '-h'])
 
 
         elif(self.arguments.args.lb_commands is not None):
             lb_class_object = LBClass(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
-            
-            if self.arguments.args.lb_commands == 'create':
+            operation = lb_class_object.caller(
+                    self.arguments.args.lb_commands)
+            if operation:
                 try:
-                    lb_class_object.create_lb()
-                except KeyboardInterrupt:
-                    Py_version_manager.py_print(" ")
-                
-            elif self.arguments.args.lb_commands == 'list' or self.arguments.args.lb_commands == 'ls':
-                try:
-                    lb_class_object.list_lb()
-                except KeyboardInterrupt:
-                    Py_version_manager.py_print(" ")
-                
-            elif self.arguments.args.lb_commands == 'delete':
-                try:
-                    lb_class_object.delete_lb()
-                except KeyboardInterrupt:
-                    Py_version_manager.py_print(" ")
-                
-            elif self.arguments.args.lb_commands == 'edit':
-                try:
-                    lb_class_object.edit_lb()
+                    operation()
                 except KeyboardInterrupt:
                     Py_version_manager.py_print(" ")
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/loadbalancer/lb_services.py` & `e2e_cli-0.9.9.9/e2e_cli/loadbalancer/lb_services.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.8/e2e_cli/main.py` & `e2e_cli-0.9.9.9/e2e_cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         inputs=Namespace()
         for element in argv:
             if "=" in element:
                     x=element.split("=")
                     setattr(inputs, x[0], x[1])
             elif(element.startswith('-')):
                     setattr(inputs, element.lstrip('-'), True)
-        return inputs        
+        return inputs.__dict__       
         
     def parse_args(self, args=None, namespace=None):
         args, argv = self.parse_known_args(args, namespace)
         if argv:
             msg = argparse._('unrecognized arguments: %s')
             self.error(msg % ' '.join(argv))
         # here args is used for routing to service and inputs as input to service
@@ -195,14 +195,15 @@
     bucket_parser = sub_parsers.add_parser("bucket", help="To create/delete/list buckets of the user", formatter_class=argparse.RawTextHelpFormatter)
     dbaas_parser = sub_parsers.add_parser("dbaas", help="To perform operations over DBaaS service provided", formatter_class=argparse.RawTextHelpFormatter)
     image_parser = sub_parsers.add_parser("image", help="To perform operations over Image service provided", formatter_class=argparse.RawTextHelpFormatter)
     autoscaling_parser= sub_parsers.add_parser("autoscaling", help="To create/delete/list autoscaling for the user", formatter_class=argparse.RawTextHelpFormatter)
     vpc_parser= sub_parsers.add_parser("vpc", help="To create/delete/list vpc for the user", formatter_class=argparse.RawTextHelpFormatter)
     cdn_parser= sub_parsers.add_parser("cdn", help="To create/delete/list cdn for the user", formatter_class=argparse.RawTextHelpFormatter)
     volumes_parser= sub_parsers.add_parser("volume", help="To create/delete/list volume for the user", formatter_class=argparse.RawTextHelpFormatter)
+    security_groups_parser= sub_parsers.add_parser("security_groups", help="To view security_groups for user")
     
     m = Main()
     m.alias(alias_parser)
     m.bucket(bucket_parser)
     m.node(node_parser)
     m.dbaas(dbaas_parser)
     m.lb(lb_parser)
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/node/node_crud/node.py` & `e2e_cli-0.9.9.9/e2e_cli/node/node_crud/node.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,56 @@
 import json
+
 from prettytable import PrettyTable
 
 
 from e2e_cli.core.py_manager import Py_version_manager
 from e2e_cli.core.alias_service import get_user_cred
 from e2e_cli.core.request_service import Request
 from e2e_cli.core.helper_service import Checks
-from e2e_cli.core.constants import BASE_URL
+from e2e_cli.node.node_crud.helpers import node_create_helper, node_delete_helper, node_get_helper
 from e2e_cli.node.node_crud.node_listing_service import Nodelisting
 
-    
-class payload:
-    def __init__(self, arguments):
-
-        if('auto' in arguments["inputs"]):
-            node_specifications=Nodelisting(arguments['alias']).node_listing()
-            self.image = node_specifications['image']
-            self.plan = node_specifications['plan']
-            if(node_specifications['location']=='Delhi'):
-                    self.region='ncr'
-            else:
-                    self.region='mumbai'
-        else :
-            self.image = Checks.take_input(arguments["inputs"], "image")
-            self.plan = Checks.take_input(arguments["inputs"], "plan")
-            self.region = Checks.take_input(arguments["inputs"], "region")
-                    
-        self.security_group_id = Checks.take_input(arguments["inputs"], "security_group_id")
-        self.name = Checks.take_input(arguments["inputs"], "name")
-        self.ssh_keys = []
-
 
 class NodeCrud:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
         if (get_user_cred(kwargs['alias'])):
             self.API_key = get_user_cred(kwargs['alias'])[1]
             self.Auth_Token = get_user_cred(kwargs['alias'])[0]
             self.possible = True
         else:
             self.possible = False
 
 
+    def caller(self, method):
+        function_set = {"create": self.create_node,
+                        "delete": self.delete_node,
+                        "get": self.get_node_by_id,
+                        "list": self.list_node
+                        }
+        return function_set.get(method)
+
+
     def create_node(self):
         Py_version_manager.py_print("Creating")
-        my_payload = payload(self.kwargs)
+        my_payload = node_create_helper(self.kwargs)
         API_key = self.API_key
         Auth_Token = self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/nodes/?apikey=" + API_key+"&location=Delhi"
+        url = "myaccount/api/v1/nodes/?apikey=" + API_key+"&location=Delhi"
         req = "POST"
         if ('auto' in self.kwargs["inputs"]):
-                        user_agent='cli_python'
+            user_agent = 'cli_python'
         else:
-                user_agent='cli-e2e'
-        my_payload=my_payload.__dict__
+            user_agent = 'cli-e2e'
+        my_payload = my_payload.__dict__
+
+        status = Request(url, Auth_Token, json.dumps(
+            my_payload), req, user_agent).response.json()
 
-        status = Request(url, Auth_Token, json.dumps(my_payload), req, user_agent).response.json()
-    
         # if Checks.status_result(status,req):
         #     try :
         #         x = PrettyTable()
         #         x.field_names = ["ID", "Name", "Created at", "disk", "Status", "Plan"]
         #         x.add_row([status['data']['id'], status['data']['name'],
         #               status['data']['created_at'], status['data']['disk'], status['data']['status'], status['data']['plan']])
         #         Py_version_manager.py_print(x)
@@ -73,66 +63,68 @@
         Checks.show_json(status)
 
 
     def delete_node(self):
         my_payload = {}
         API_key = self.API_key
         Auth_Token = self.Auth_Token
-        node_id = Checks.take_input(self.kwargs["inputs"], "node_id")
-        while(not Checks.is_int(node_id)):
-              node_id = Py_version_manager.py_input("please enter node id (integer only) ")
-        url =  BASE_URL+"myaccount/api/v1/nodes/" + str(node_id) + "/?apikey="+API_key
+        node_delete_helper(self.kwargs["inputs"])
+        node_id = self.kwargs["inputs"]["node_id"]
+        url = "myaccount/api/v1/nodes/" + \
+            str(node_id) + "/?apikey="+API_key
         req = "DELETE"
 
-        confirmation =Py_version_manager.py_input("are you sure you want to delete press y for yes, else any other key : ")
-        if(confirmation.lower()=="y"):
+        confirmation = Py_version_manager.py_input(
+            "are you sure you want to delete press y for yes, else any other key : ")
+        if (confirmation.lower() == "y"):
             status = Request(url, Auth_Token, my_payload, req).response.json()
-            if Checks.status_result(status,req):
-                        Py_version_manager.py_print("Node Successfully deleted")
-                        Py_version_manager.py_print("use following command -> e2e_cli <alias> node list to check if bucket has been deleted")
-            
+            if Checks.status_result(status, req):
+                Py_version_manager.py_print("Node Successfully deleted")
+                Py_version_manager.py_print(
+                    "use following command -> e2e_cli <alias> node list to check if bucket has been deleted")
+
             # if('json' in self.kwargs["inputs"]):
             #     Checks.show_json(status)
         Checks.show_json(status)
 
 
     def get_node_by_id(self):
         my_payload = {}
         API_key = self.API_key
         Auth_Token = self.Auth_Token
-        node_id = node_id = Checks.take_input(self.kwargs["inputs"], "node_id")
-        while(not Checks.is_int(node_id)):
-              node_id = Py_version_manager.py_input("please enter node id (integer only) ")
-        url =  BASE_URL+"myaccount/api/v1/nodes/" + str(node_id) + "/?apikey="+API_key
+        node_get_helper(self.kwargs["inputs"])
+        node_id = self.kwargs["inputs"]["node_id"]
+        url = "myaccount/api/v1/nodes/" + \
+            str(node_id) + "/?apikey="+API_key
         req = "GET"
         status = Request(url, Auth_Token, my_payload, req).response.json()
 
         # if Checks.status_result(status, req):
         #     try:
         #         x = PrettyTable()
         #         x.field_names = ["VM id", "Name", "Created at", "disk", "Plan", "Public IP", "Status"]
         #         x.add_row([ status['data']['vm_id'], status['data']['name'], status['data']['created_at'], status['data']['disk'],  status['data']['plan'], status['data']['public_ip_address'], status['data']['status'] ])
         #         Py_version_manager.py_print(x)
         #     except Exception as e:
         #                 Py_version_manager.py_print("Errors : ", e)
-        
+
         # if('json' in self.kwargs["inputs"]):
         #     Checks.show_json(status)
         Checks.status_result(status)
         Checks.show_json(status)
 
 
     def list_node(self, parameter=0):
         my_payload = {}
         API_key = self.API_key
         Auth_Token = self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/nodes/?apikey=" + API_key+"&location=Delhi"
+        url = "myaccount/api/v1/nodes/?apikey=" + API_key+"&location=Delhi"
         req = "GET"
         status = Request(url, Auth_Token, my_payload,
-                       req).response.json()
+                         req).response.json()
 
         if parameter == 0:
             # if Checks.status_result(status, req):
             #     list=status['data']
             #     try:
             #         i = 1
             #         x = PrettyTable()
@@ -140,21 +132,21 @@
             #         for element in list:
             #             x.add_row([i, element['id'], element['name'],
             #                       element['plan'],  element['status']])
             #             i = i+1
             #         Py_version_manager.py_print(x)
             #     except Exception as e:
             #             Py_version_manager.py_print("Errors : ", e)
-                        
+
             #     if('json' in self.kwargs["inputs"]):
             #         Checks.show_json(status)
             Checks.status_result(status)
             Checks.show_json(status)
-            
-        elif parameter==1:
-                    return status['data']
+
+        elif parameter == 1:
+            return status['data']
 
 
     def update_node(self):
         API_key = self.API_key
         Auth_Token = self.Auth_Token
         Py_version_manager.py_print("update call")
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/node/node_crud/node_listing_service.py` & `e2e_cli-0.9.9.9/e2e_cli/node/node_crud/node_listing_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from prettytable import PrettyTable
 
 from e2e_cli.core.py_manager import Py_version_manager
 from e2e_cli.core.alias_service import get_user_cred
 from e2e_cli.core.request_service import Request
-from e2e_cli.core.constants import BASE_URL
 
 
 class Nodelisting:
     def __init__(self, alias):
         if (get_user_cred(alias)):
             self.API_key = get_user_cred(alias)[1]
             self.Auth_Token = get_user_cred(alias)[0]
 
 
     def node_listing(self):
-        url =  BASE_URL+"myaccount/api/v1/images/category-list/?apikey=" +self.API_key+ "&contact_person_id=null&location=Delhi"
+        url =  "myaccount/api/v1/images/category-list/?apikey=" +self.API_key+ "&contact_person_id=null&location=Delhi"
         req= "GET"
         my_payload={}
         response= Request(url, self.Auth_Token, my_payload, req, user_agent='cli_python').response.json()['data']
 
         i=1
         x=PrettyTable()
         x.field_names=["ID", 'Types of node']
@@ -64,15 +63,15 @@
         node_type=node_type.split()
         node_type1=""
         for ele in node_type:
               node_type1=node_type1+ele+"%20"
       
       
 
-        url =  BASE_URL+"myaccount/api/v1/images/?apikey="+ self.API_key+"&contact_person_id=null&display_category="+node_type1 +"&category="+Os_type +"&osversion="+Os_version +"&gpu_type=&ng_container=null&os="+Os_type +"&location=Delhi"
+        url =  "myaccount/api/v1/images/?apikey="+ self.API_key+"&contact_person_id=null&display_category="+node_type1 +"&category="+Os_type +"&osversion="+Os_version +"&gpu_type=&ng_container=null&os="+Os_type +"&location=Delhi"
         req= "GET"
         my_payload={}
         response= Request(url, self.Auth_Token, my_payload, req, user_agent='cli_python').response.json()['data']
         i=1
         x=PrettyTable()
         x.field_names=["ID", 'Plan', 'image', 'location', 'Price(Monthly)', 'Price(Hourly)']
         Plan_list=dict()
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_actions/volumes_action.py` & `e2e_cli-0.9.9.9/e2e_cli/volumes/volumes_actions/volumes_action.py`

 * *Files identical despite different names*

### Comparing `e2e_cli-0.9.9.8/e2e_cli/volumes/volumes_routing.py` & `e2e_cli-0.9.9.9/e2e_cli/volumes/volumes_routing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import subprocess
 
 from e2e_cli.core.py_manager import Py_version_manager
-from e2e_cli.volumes.volumes_crud.volumes import volumes_Crud
+from e2e_cli.volumes.volumes_crud.volumes import VolumesCrud
 from e2e_cli.volumes.volumes_actions.volumes_action import volumesActions
 
 class volumes_Routing:
     def __init__(self, arguments):
         self.arguments = arguments
         
         
@@ -19,34 +19,24 @@
 
 
         elif (self.arguments.args.volumes_commands is not None) and (self.arguments.args.action is not None):
               Py_version_manager.py_print("Only one action at a time !!")
 
 
         elif(self.arguments.args.volumes_commands is not None):
-            volumes_operations = volumes_Crud(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
+            volumes_operations = VolumesCrud(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
             if(volumes_operations.possible):
-
-                if self.arguments.args.volumes_commands == 'create':
-                        try:
-                            volumes_operations.create_volumes()
-                        except KeyboardInterrupt:
-                            Py_version_manager.py_print(" ")
-
-                elif self.arguments.args.volumes_commands == 'delete':
-                        try:
-                            volumes_operations.delete_volumes()
-                        except KeyboardInterrupt:
-                            Py_version_manager.py_print(" ")
-                                
-                elif self.arguments.args.volumes_commands == 'list':
-                        try:
-                            volumes_operations.list_volumes()
-                        except KeyboardInterrupt:
-                            Py_version_manager.py_print(" ")
+                operation = volumes_operations.caller(
+                    self.arguments.args.volumes_commands)
+                if operation:
+                    try:
+                        operation()
+                    except KeyboardInterrupt:
+                        Py_version_manager.py_print(" ")
+                    
 
                 else:
                     Py_version_manager.py_print("command not found")
                     if(Parsing_Errors):
                         Py_version_manager.py_print("Parsing Errors :")
                         Py_version_manager.py_print(*Parsing_Errors, sep="\n")
         # elif self.arguments.args.action == "attach_volume":
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/vpc/vpc.py` & `e2e_cli-0.9.9.9/e2e_cli/vpc/vpc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,90 +1,98 @@
 from prettytable import PrettyTable
 import json
 
 from e2e_cli.core.py_manager import Py_version_manager
 from e2e_cli.core.request_service import Request
 from e2e_cli.core.alias_service import get_user_cred
 from e2e_cli.core.helper_service import Checks
-from e2e_cli.core.constants import BASE_URL
+from e2e_cli.vpc import helpers
 
 
 class vpc_Crud:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
         if(get_user_cred(kwargs['alias'])):
             self.API_key=get_user_cred(kwargs['alias'])[1]
             self.Auth_Token=get_user_cred(kwargs['alias'])[0]
             self.possible=True
         else:
             self.possible=False
-        
+
+    def caller(self, method):
+        function_set = {"create": self.create_vpc,
+                        "delete": self.delete_vpc,
+                        "list": self.list_vpc,
+                        }
+        return function_set.get(method)   
+
 
     def create_vpc(self):
         Py_version_manager.py_print("Creating")
-        my_payload= json.dumps({
-                "network_size": 512,
-                "vpc_name": Checks.take_input(self.kwargs["inputs"], "vpc_name")
-            }) 
         API_key=self.API_key
         Auth_Token=self.Auth_Token
-        url =  BASE_URL+"myaccount/api/v1/vpc/?apikey="+API_key+"&location=Delhi"
+        helpers.create_vpc_helper(self.kwargs["inputs"])
+        my_payload= json.dumps({
+                "network_size": 512,
+                "vpc_name": self.kwargs["inputs"]["vpc_name"]
+            })
+        url =  f"myaccount/api/v1/vpc/?apikey={API_key}&location=Delhi"
         req="POST"
         status=Request(url, Auth_Token, my_payload, req).response.json()
-               
-        if Checks.status_result(status, req):
-            try:
-                x = PrettyTable()
-                x.field_names = ["ID", "Name"]
-                x.add_row([status['data']['vpc_id'], status['data']['name'] ])
-                Py_version_manager.py_print(x)
-            except Exception as e:
-                      Py_version_manager.py_print("Errors : ", e)
-                  
-        if('json' in self.kwargs["inputs"]):
-            Checks.show_json(status)    
+
+        Checks.show_json(status)        
+        # if Checks.status_result(status, req):
+        #     try:
+        #         x = PrettyTable()
+        #         x.field_names = ["ID", "Name"]
+        #         x.add_row([status['data']['vpc_id'], status['data']['name'] ])
+        #         Py_version_manager.py_print(x)
+        #     except Exception as e:
+        #               Py_version_manager.py_print("Errors : ", e)         
+        # if('json' in self.kwargs["inputs"]):
+        #     Checks.show_json(status)    
 
 
     def delete_vpc(self):
         my_payload={}
-        network_id=Checks.take_input(self.kwargs["inputs"], "network_id")
-        while(not Checks.is_int(network_id)):
-                network_id=Py_version_manager.py_input("Only integers allowed ")
+        network_id=self.kwargs["inputs"]["network_id"]
+        helpers.delete_vpc_helper(self.kwargs["inputs"])
         API_key=self.API_key
         Auth_Token=self.Auth_Token
-        url =  BASE_URL+"/myaccount/api/v1/vpc/"+ network_id +"/?apikey="+API_key
+        url =  f"myaccount/api/v1/vpc/{network_id}/?apikey={API_key}"
         req="DELETE"
         status=Request(url, Auth_Token, my_payload, req).response.json()
 
         if Checks.status_result(status,req):
                         Py_version_manager.py_print("vpc Successfully deleted")
                         Py_version_manager.py_print("use following command -> e2e_cli --alias vpc list to check if vpc has been deleted")
         
         Checks.show_json(status)
 
 
     def list_vpc(self):
         my_payload={}
         API_key= self.API_key  
         Auth_Token= self.Auth_Token 
-        url =  BASE_URL+"myaccount/api/v1/vpc/list/?apikey="+ API_key+"&location=Delhi"
+        url =  "myaccount/api/v1/vpc/list/?apikey="+ API_key+"&location=Delhi"
         req="GET"
         status=Request(url, Auth_Token, my_payload, req).response.json()
         
-        if Checks.status_result(status, req):
-                Py_version_manager.py_print("Your vpcs : ")
-                try:
-                    list=status['data']
-                    i=1
-                    x = PrettyTable()
-                    x.field_names = ["index", "network_id", "Name", "network_mask", "gateway_ip", "pool_size"]
-                    for element in list:
-                        x.add_row([i, element['network_id'], element['name'], element['network_mask'], element["gateway_ip"], element["pool_size"]])
-                        i = i+1
-                    Py_version_manager.py_print(x)
-                except Exception as e:
-                      Py_version_manager.py_print("Errors : ", e)
+        Checks.show_json(status)
+        # if Checks.status_result(status, req):
+        #         Py_version_manager.py_print("Your vpcs : ")
+        #         try:
+        #             list=status['data']
+        #             i=1
+        #             x = PrettyTable()
+        #             x.field_names = ["index", "network_id", "Name", "network_mask", "gateway_ip", "pool_size"]
+        #             for element in list:
+        #                 x.add_row([i, element['network_id'], element['name'], element['network_mask'], element["gateway_ip"], element["pool_size"]])
+        #                 i = i+1
+        #             Py_version_manager.py_print(x)
+        #         except Exception as e:
+        #               Py_version_manager.py_print("Errors : ", e)
 
-        if('json' in self.kwargs["inputs"]):
-            Checks.show_json(status)    
+        # if('json' in self.kwargs["inputs"]):
+        #     Checks.show_json(status)
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli/vpc/vpc_routing.py` & `e2e_cli-0.9.9.9/e2e_cli/cdn/cdn_routing.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 import subprocess
 
 from e2e_cli.core.py_manager import Py_version_manager
-from e2e_cli.vpc.vpc import vpc_Crud
+from e2e_cli.cdn.cdn_crud.cdn import CdnCrud
+from e2e_cli.cdn.cdn_actions.cdn_action import CdnActions
 
-class vpc_Routing:
+class cdn_Routing:
     def __init__(self, arguments):
         self.arguments = arguments
         
         
     def route(self, Parsing_Errors):
-        if (self.arguments.args.vpc_commands is None):
+        if (self.arguments.args.action is None) and (self.arguments.args.cdn_commands is None):
             if(Parsing_Errors):
                 Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
                 Py_version_manager.py_print("")
-            subprocess.call(['e2e_cli', 'vpc', '-h'])
+            subprocess.call(['e2e_cli', 'cdn', '-h'])
 
 
-        elif (self.arguments.args.vpc_commands is not None) and (self.arguments.args.action is not None):
-            Py_version_manager.py_print("Only one action at a time !!")
+        elif (self.arguments.args.cdn_commands is not None) and (self.arguments.args.action is not None):
+              Py_version_manager.py_print("Only one action at a time !!")
 
 
-        elif (self.arguments.args.vpc_commands is not None):
-            vpc_operations = vpc_Crud(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
-            if(vpc_operations.possible):  
-
-                if self.arguments.args.vpc_commands == 'create':
-                                try:
-                                    vpc_operations.create_vpc()
-                                except KeyboardInterrupt:
-                                    Py_version_manager.py_print(" ")
-
-                elif self.arguments.args.vpc_commands == 'delete':
-                    vpc_operations = vpc_Crud(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
-                    if(vpc_operations.possible):
-                                try:
-                                    vpc_operations.delete_vpc()
-                                except KeyboardInterrupt:
-                                    Py_version_manager.py_print(" ")
-                                
-                elif self.arguments.args.vpc_commands == 'list':
-                    vpc_operations = vpc_Crud(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
-                    if(vpc_operations.possible):
-                                try:
-                                    vpc_operations.list_vpc()
-                                except KeyboardInterrupt:
-                                    Py_version_manager.py_print(" ")
+        elif(self.arguments.args.cdn_commands is not None):
+            cdn_operations = CdnCrud(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
+            if(cdn_operations.possible):
+                operation = cdn_operations.caller(
+                    self.arguments.args.cdn_commands)
+                if operation:
+                    try:
+                        operation()
+                    except KeyboardInterrupt:
+                        Py_version_manager.py_print(" ")
+
+
+        elif(self.arguments.args.action is not None):
+            cdn_operations = CdnActions(alias=self.arguments.args.alias, inputs=self.arguments.inputs)
+            if(cdn_operations.possible):
+                operation = cdn_operations.caller(
+                    self.arguments.args.action)
+                if operation:
+                    try:
+                        operation()
+                    except KeyboardInterrupt:
+                        Py_version_manager.py_print(" ")
 
                 else:
                     Py_version_manager.py_print("command not found")
                     if(Parsing_Errors):
                         Py_version_manager.py_print("Parsing Errors :")
                         Py_version_manager.py_print(*Parsing_Errors, sep="\n")
+                
 
         else:
             Py_version_manager.py_print("command not found")
             if(Parsing_Errors):
                 Py_version_manager.py_print("Parsing Errors :")
                 Py_version_manager.py_print(*Parsing_Errors, sep="\n")
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli.egg-info/PKG-INFO` & `e2e_cli-0.9.9.9/e2e_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2e-cli
-Version: 0.9.9.8
+Version: 0.9.9.9
 Summary: This a E2E CLI tool for myAccount
 Home-page: UNKNOWN
 Author: Sajal&Aman@E2E_Networks_Ltd
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `e2e_cli-0.9.9.8/e2e_cli.egg-info/SOURCES.txt` & `e2e_cli-0.9.9.9/e2e_cli.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,29 +8,36 @@
 e2e_cli/man_display.py
 e2e_cli.egg-info/PKG-INFO
 e2e_cli.egg-info/SOURCES.txt
 e2e_cli.egg-info/dependency_links.txt
 e2e_cli.egg-info/entry_points.txt
 e2e_cli.egg-info/requires.txt
 e2e_cli.egg-info/top_level.txt
+e2e_cli/add_on_services/__init__.py
+e2e_cli/add_on_services/view_security_groups.py
 e2e_cli/auto_scaling/__init__.py
 e2e_cli/auto_scaling/auto_scaling.py
 e2e_cli/auto_scaling/autoscaling_routing.py
+e2e_cli/auto_scaling/helpers.py
 e2e_cli/bucket_store/__init__.py
 e2e_cli/bucket_store/bucket_routing.py
 e2e_cli/bucket_store/bucket_actions/__init__.py
 e2e_cli/bucket_store/bucket_actions/bucket_actions.py
+e2e_cli/bucket_store/bucket_actions/helpers.py
 e2e_cli/bucket_store/bucket_crud/__init__.py
 e2e_cli/bucket_store/bucket_crud/bucket_storage.py
+e2e_cli/bucket_store/bucket_crud/helpers.py
 e2e_cli/cdn/__init__.py
 e2e_cli/cdn/cdn_routing.py
 e2e_cli/cdn/cdn_actions/__init__.py
 e2e_cli/cdn/cdn_actions/cdn_action.py
+e2e_cli/cdn/cdn_actions/helpers.py
 e2e_cli/cdn/cdn_crud/__init__.py
 e2e_cli/cdn/cdn_crud/cdn.py
+e2e_cli/cdn/cdn_crud/helpers.py
 e2e_cli/config/__init__.py
 e2e_cli/config/config.py
 e2e_cli/config/config_routing.py
 e2e_cli/config/config_service.py
 e2e_cli/core/__init__.py
 e2e_cli/core/alias_service.py
 e2e_cli/core/constants.py
@@ -39,38 +46,45 @@
 e2e_cli/core/helper_service.py
 e2e_cli/core/py_manager.py
 e2e_cli/core/request_service.py
 e2e_cli/dbaas/__init__.py
 e2e_cli/dbaas/dbaas_routing.py
 e2e_cli/dbaas/dbaas_actions/__init__.py
 e2e_cli/dbaas/dbaas_actions/dbaas_action.py
+e2e_cli/dbaas/dbaas_actions/helpers.py
 e2e_cli/dbaas/dbaas_crud/__init__.py
 e2e_cli/dbaas/dbaas_crud/dbaas.py
 e2e_cli/dbaas/dbaas_crud/dbaas_services.py
 e2e_cli/docs/__init__.py
 e2e_cli/docs/e2e_cli.1
 e2e_cli/image/__init__.py
 e2e_cli/image/image_routing.py
 e2e_cli/image/image_crud/__init__.py
+e2e_cli/image/image_crud/helpers.py
 e2e_cli/image/image_crud/image.py
 e2e_cli/image/image_listing/__init__.py
 e2e_cli/image/image_listing/image_list.py
 e2e_cli/loadbalancer/__init__.py
 e2e_cli/loadbalancer/lb.py
 e2e_cli/loadbalancer/lb_routing.py
 e2e_cli/loadbalancer/lb_services.py
 e2e_cli/node/__init__.py
 e2e_cli/node/node_routing.py
 e2e_cli/node/node_actions/__init__.py
+e2e_cli/node/node_actions/helpers.py
 e2e_cli/node/node_actions/node_action.py
 e2e_cli/node/node_crud/__init__.py
+e2e_cli/node/node_crud/helpers.py
 e2e_cli/node/node_crud/node.py
 e2e_cli/node/node_crud/node_listing_service.py
 e2e_cli/volumes/__init__.py
 e2e_cli/volumes/volumes_routing.py
 e2e_cli/volumes/volumes_actions/__init__.py
 e2e_cli/volumes/volumes_actions/volumes_action.py
 e2e_cli/volumes/volumes_crud/__init__.py
+e2e_cli/volumes/volumes_crud/constants.py
+e2e_cli/volumes/volumes_crud/helpers.py
 e2e_cli/volumes/volumes_crud/volumes.py
 e2e_cli/vpc/__init__.py
+e2e_cli/vpc/helpers.py
 e2e_cli/vpc/vpc.py
 e2e_cli/vpc/vpc_routing.py
```

### Comparing `e2e_cli-0.9.9.8/setup.py` & `e2e_cli-0.9.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   from setuptools import setup, find_packages
 
 with open( (os.path.dirname(__file__)+"/e2e_cli/docs/PyPi_description.md") , 'r') as f:
       pypi_text=f.read()
 
 setup(
     name='e2e_cli',
-    version='0.9.9.8',
+    version='0.9.9.9',
     description="This a E2E CLI tool for myAccount",
     author="Sajal&Aman@E2E_Networks_Ltd",
     packages=find_packages(),
     install_requires=['prettytable', 'requests', 'setuptools', 'chardet'],
     
     long_description_content_type="text/markdown",
     long_description=pypi_text,
```

