# Comparing `tmp/pulumi_fastly-8.2.0a1687671288.tar.gz` & `tmp/pulumi_fastly-8.2.0a1688059197.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fastly-8.2.0a1687671288.tar", last modified: Sun Jun 25 05:48:19 2023, max compression
+gzip compressed data, was "pulumi_fastly-8.2.0a1688059197.tar", last modified: Thu Jun 29 17:24:26 2023, max compression
```

## Comparing `pulumi_fastly-8.2.0a1687671288.tar` & `pulumi_fastly-8.2.0a1688059197.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:48:19.796306 pulumi_fastly-8.2.0a1687671288/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-25 05:48:19.796306 pulumi_fastly-8.2.0a1687671288/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:48:19.796306 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   509608 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:48:19.796306 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/configstore.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/configstore_entries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_fastly_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_package_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_activation_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_configuration_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_platform_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_private_key_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_subscription_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_waf_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)   454051 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/service_acl_entries.py
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/service_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)    96684 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/service_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/service_dictionary_items.py
--rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/service_dynamic_snippet_content.py
--rw-r--r--   0 runner    (1001) docker     (123)   124679 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/service_vcl.py
--rw-r--r--   0 runner    (1001) docker     (123)    81770 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/service_waf_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/tls_mutual_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    34762 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/tls_subscription_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:48:19.796306 pulumi_fastly-8.2.0a1687671288/pulumi_fastly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/pulumi_fastly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 05:48:19.796306 pulumi_fastly-8.2.0a1687671288/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-25 05:48:19.000000 pulumi_fastly-8.2.0a1687671288/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:24:26.532278 pulumi_fastly-8.2.0a1688059197/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-29 17:24:26.532278 pulumi_fastly-8.2.0a1688059197/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:24:26.532278 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   509912 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:24:26.532278 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/configstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/configstore_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_fastly_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_package_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_activation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_configuration_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_platform_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_private_key_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_subscription_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_waf_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)   454355 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/service_acl_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/service_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96684 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/service_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/service_dictionary_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/service_dynamic_snippet_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124679 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/service_vcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81770 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/service_waf_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/tls_mutual_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35186 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/tls_subscription_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:24:26.532278 pulumi_fastly-8.2.0a1688059197/pulumi_fastly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/pulumi_fastly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 17:24:26.532278 pulumi_fastly-8.2.0a1688059197/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-29 17:24:26.000000 pulumi_fastly-8.2.0a1688059197/setup.py
```

### Comparing `pulumi_fastly-8.2.0a1687671288/PKG-INFO` & `pulumi_fastly-8.2.0a1688059197/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.2.0a1687671288
+Version: 8.2.0a1688059197
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi fastly
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_fastly-8.2.0a1687671288/README.md` & `pulumi_fastly-8.2.0a1688059197/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/__init__.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/_inputs.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -11345,14 +11345,17 @@
 
     @property
     @pulumi.getter(name="geoHeaders")
     def geo_headers(self) -> Optional[pulumi.Input[bool]]:
         """
         Injects Fastly-Geo-Country, Fastly-Geo-City, and Fastly-Geo-Region into the request headers
         """
+        warnings.warn("""'geo_headers' attribute has been deprecated and will be removed in the next major version release""", DeprecationWarning)
+        pulumi.log.warn("""geo_headers is deprecated: 'geo_headers' attribute has been deprecated and will be removed in the next major version release""")
+
         return pulumi.get(self, "geo_headers")
 
     @geo_headers.setter
     def geo_headers(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "geo_headers", value)
 
     @property
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/_utilities.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/config/vars.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/configstore.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/configstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/configstore_entries.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/configstore_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_datacenters.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_datacenters.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,9 +61,9 @@
     Use this data source to get the list of the [Fastly datacenters](https://developer.fastly.com/reference/api/utils/pops/).
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getDatacenters:getDatacenters', __args__, opts=opts, typ=GetDatacentersResult).value
 
     return AwaitableGetDatacentersResult(
-        id=__ret__.id,
-        pops=__ret__.pops)
+        id=pulumi.get(__ret__, 'id'),
+        pops=pulumi.get(__ret__, 'pops'))
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_dictionaries.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_dictionaries.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,18 +123,18 @@
     __args__ = dict()
     __args__['serviceId'] = service_id
     __args__['serviceVersion'] = service_version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getDictionaries:getDictionaries', __args__, opts=opts, typ=GetDictionariesResult).value
 
     return AwaitableGetDictionariesResult(
-        dictionaries=__ret__.dictionaries,
-        id=__ret__.id,
-        service_id=__ret__.service_id,
-        service_version=__ret__.service_version)
+        dictionaries=pulumi.get(__ret__, 'dictionaries'),
+        id=pulumi.get(__ret__, 'id'),
+        service_id=pulumi.get(__ret__, 'service_id'),
+        service_version=pulumi.get(__ret__, 'service_version'))
 
 
 @_utilities.lift_output_func(get_dictionaries)
 def get_dictionaries_output(service_id: Optional[pulumi.Input[str]] = None,
                             service_version: Optional[pulumi.Input[int]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDictionariesResult]:
     """
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_fastly_ip_ranges.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_fastly_ip_ranges.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,10 +91,10 @@
     [1]: https://docs.fastly.com/guides/securing-communications/accessing-fastlys-ip-ranges
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getFastlyIpRanges:getFastlyIpRanges', __args__, opts=opts, typ=GetFastlyIpRangesResult).value
 
     return AwaitableGetFastlyIpRangesResult(
-        cidr_blocks=__ret__.cidr_blocks,
-        id=__ret__.id,
-        ipv6_cidr_blocks=__ret__.ipv6_cidr_blocks)
+        cidr_blocks=pulumi.get(__ret__, 'cidr_blocks'),
+        id=pulumi.get(__ret__, 'id'),
+        ipv6_cidr_blocks=pulumi.get(__ret__, 'ipv6_cidr_blocks'))
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_package_hash.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_package_hash.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,18 +107,18 @@
     __args__ = dict()
     __args__['content'] = content
     __args__['filename'] = filename
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getPackageHash:getPackageHash', __args__, opts=opts, typ=GetPackageHashResult).value
 
     return AwaitableGetPackageHashResult(
-        content=__ret__.content,
-        filename=__ret__.filename,
-        hash=__ret__.hash,
-        id=__ret__.id)
+        content=pulumi.get(__ret__, 'content'),
+        filename=pulumi.get(__ret__, 'filename'),
+        hash=pulumi.get(__ret__, 'hash'),
+        id=pulumi.get(__ret__, 'id'))
 
 
 @_utilities.lift_output_func(get_package_hash)
 def get_package_hash_output(content: Optional[pulumi.Input[Optional[str]]] = None,
                             filename: Optional[pulumi.Input[Optional[str]]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPackageHashResult]:
     """
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_services.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_services.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,10 +73,10 @@
     Use this data source to get the list of the [Fastly services](https://developer.fastly.com/reference/api/services/service/).
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getServices:getServices', __args__, opts=opts, typ=GetServicesResult).value
 
     return AwaitableGetServicesResult(
-        details=__ret__.details,
-        id=__ret__.id,
-        ids=__ret__.ids)
+        details=pulumi.get(__ret__, 'details'),
+        id=pulumi.get(__ret__, 'id'),
+        ids=pulumi.get(__ret__, 'ids'))
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_activation.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_activation.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,19 +126,19 @@
     __args__['configurationId'] = configuration_id
     __args__['domain'] = domain
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsActivation:getTlsActivation', __args__, opts=opts, typ=GetTlsActivationResult).value
 
     return AwaitableGetTlsActivationResult(
-        certificate_id=__ret__.certificate_id,
-        configuration_id=__ret__.configuration_id,
-        created_at=__ret__.created_at,
-        domain=__ret__.domain,
-        id=__ret__.id)
+        certificate_id=pulumi.get(__ret__, 'certificate_id'),
+        configuration_id=pulumi.get(__ret__, 'configuration_id'),
+        created_at=pulumi.get(__ret__, 'created_at'),
+        domain=pulumi.get(__ret__, 'domain'),
+        id=pulumi.get(__ret__, 'id'))
 
 
 @_utilities.lift_output_func(get_tls_activation)
 def get_tls_activation_output(certificate_id: Optional[pulumi.Input[Optional[str]]] = None,
                               configuration_id: Optional[pulumi.Input[Optional[str]]] = None,
                               domain: Optional[pulumi.Input[Optional[str]]] = None,
                               id: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_activation_ids.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_activation_ids.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,17 +89,17 @@
     """
     __args__ = dict()
     __args__['certificateId'] = certificate_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsActivationIds:getTlsActivationIds', __args__, opts=opts, typ=GetTlsActivationIdsResult).value
 
     return AwaitableGetTlsActivationIdsResult(
-        certificate_id=__ret__.certificate_id,
-        id=__ret__.id,
-        ids=__ret__.ids)
+        certificate_id=pulumi.get(__ret__, 'certificate_id'),
+        id=pulumi.get(__ret__, 'id'),
+        ids=pulumi.get(__ret__, 'ids'))
 
 
 @_utilities.lift_output_func(get_tls_activation_ids)
 def get_tls_activation_ids_output(certificate_id: Optional[pulumi.Input[Optional[str]]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTlsActivationIdsResult]:
     """
     Use this data source to get the list of TLS Activation identifiers in Fastly.
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_certificate.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_certificate.py`

 * *Files 11% similar despite different names*

```diff
@@ -189,24 +189,24 @@
     __args__['issuedTo'] = issued_to
     __args__['issuer'] = issuer
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsCertificate:getTlsCertificate', __args__, opts=opts, typ=GetTlsCertificateResult).value
 
     return AwaitableGetTlsCertificateResult(
-        created_at=__ret__.created_at,
-        domains=__ret__.domains,
-        id=__ret__.id,
-        issued_to=__ret__.issued_to,
-        issuer=__ret__.issuer,
-        name=__ret__.name,
-        replace=__ret__.replace,
-        serial_number=__ret__.serial_number,
-        signature_algorithm=__ret__.signature_algorithm,
-        updated_at=__ret__.updated_at)
+        created_at=pulumi.get(__ret__, 'created_at'),
+        domains=pulumi.get(__ret__, 'domains'),
+        id=pulumi.get(__ret__, 'id'),
+        issued_to=pulumi.get(__ret__, 'issued_to'),
+        issuer=pulumi.get(__ret__, 'issuer'),
+        name=pulumi.get(__ret__, 'name'),
+        replace=pulumi.get(__ret__, 'replace'),
+        serial_number=pulumi.get(__ret__, 'serial_number'),
+        signature_algorithm=pulumi.get(__ret__, 'signature_algorithm'),
+        updated_at=pulumi.get(__ret__, 'updated_at'))
 
 
 @_utilities.lift_output_func(get_tls_certificate)
 def get_tls_certificate_output(domains: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                                id: Optional[pulumi.Input[Optional[str]]] = None,
                                issued_to: Optional[pulumi.Input[Optional[str]]] = None,
                                issuer: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_certificate_ids.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_certificate_ids.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,9 +71,9 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsCertificateIds:getTlsCertificateIds', __args__, opts=opts, typ=GetTlsCertificateIdsResult).value
 
     return AwaitableGetTlsCertificateIdsResult(
-        id=__ret__.id,
-        ids=__ret__.ids)
+        id=pulumi.get(__ret__, 'id'),
+        ids=pulumi.get(__ret__, 'ids'))
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_configuration.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -183,23 +183,23 @@
     __args__['name'] = name
     __args__['tlsProtocols'] = tls_protocols
     __args__['tlsService'] = tls_service
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsConfiguration:getTlsConfiguration', __args__, opts=opts, typ=GetTlsConfigurationResult).value
 
     return AwaitableGetTlsConfigurationResult(
-        created_at=__ret__.created_at,
-        default=__ret__.default,
-        dns_records=__ret__.dns_records,
-        http_protocols=__ret__.http_protocols,
-        id=__ret__.id,
-        name=__ret__.name,
-        tls_protocols=__ret__.tls_protocols,
-        tls_service=__ret__.tls_service,
-        updated_at=__ret__.updated_at)
+        created_at=pulumi.get(__ret__, 'created_at'),
+        default=pulumi.get(__ret__, 'default'),
+        dns_records=pulumi.get(__ret__, 'dns_records'),
+        http_protocols=pulumi.get(__ret__, 'http_protocols'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        tls_protocols=pulumi.get(__ret__, 'tls_protocols'),
+        tls_service=pulumi.get(__ret__, 'tls_service'),
+        updated_at=pulumi.get(__ret__, 'updated_at'))
 
 
 @_utilities.lift_output_func(get_tls_configuration)
 def get_tls_configuration_output(default: Optional[pulumi.Input[Optional[bool]]] = None,
                                  http_protocols: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                                  id: Optional[pulumi.Input[Optional[str]]] = None,
                                  name: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_configuration_ids.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_configuration_ids.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,9 +71,9 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsConfigurationIds:getTlsConfigurationIds', __args__, opts=opts, typ=GetTlsConfigurationIdsResult).value
 
     return AwaitableGetTlsConfigurationIdsResult(
-        id=__ret__.id,
-        ids=__ret__.ids)
+        id=pulumi.get(__ret__, 'id'),
+        ids=pulumi.get(__ret__, 'ids'))
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_domain.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_domain.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,19 +111,19 @@
     """
     __args__ = dict()
     __args__['domain'] = domain
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsDomain:getTlsDomain', __args__, opts=opts, typ=GetTlsDomainResult).value
 
     return AwaitableGetTlsDomainResult(
-        domain=__ret__.domain,
-        id=__ret__.id,
-        tls_activation_ids=__ret__.tls_activation_ids,
-        tls_certificate_ids=__ret__.tls_certificate_ids,
-        tls_subscription_ids=__ret__.tls_subscription_ids)
+        domain=pulumi.get(__ret__, 'domain'),
+        id=pulumi.get(__ret__, 'id'),
+        tls_activation_ids=pulumi.get(__ret__, 'tls_activation_ids'),
+        tls_certificate_ids=pulumi.get(__ret__, 'tls_certificate_ids'),
+        tls_subscription_ids=pulumi.get(__ret__, 'tls_subscription_ids'))
 
 
 @_utilities.lift_output_func(get_tls_domain)
 def get_tls_domain_output(domain: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTlsDomainResult]:
     """
     Use this data source to get the IDs of activations, certificates and subscriptions associated with a domain.
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_platform_certificate.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_platform_certificate.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,22 +156,22 @@
     __args__ = dict()
     __args__['domains'] = domains
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsPlatformCertificate:getTlsPlatformCertificate', __args__, opts=opts, typ=GetTlsPlatformCertificateResult).value
 
     return AwaitableGetTlsPlatformCertificateResult(
-        configuration_id=__ret__.configuration_id,
-        created_at=__ret__.created_at,
-        domains=__ret__.domains,
-        id=__ret__.id,
-        not_after=__ret__.not_after,
-        not_before=__ret__.not_before,
-        replace=__ret__.replace,
-        updated_at=__ret__.updated_at)
+        configuration_id=pulumi.get(__ret__, 'configuration_id'),
+        created_at=pulumi.get(__ret__, 'created_at'),
+        domains=pulumi.get(__ret__, 'domains'),
+        id=pulumi.get(__ret__, 'id'),
+        not_after=pulumi.get(__ret__, 'not_after'),
+        not_before=pulumi.get(__ret__, 'not_before'),
+        replace=pulumi.get(__ret__, 'replace'),
+        updated_at=pulumi.get(__ret__, 'updated_at'))
 
 
 @_utilities.lift_output_func(get_tls_platform_certificate)
 def get_tls_platform_certificate_output(domains: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                                         id: Optional[pulumi.Input[Optional[str]]] = None,
                                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTlsPlatformCertificateResult]:
     """
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_platform_certificate_ids.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_platform_certificate_ids.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,9 +70,9 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsPlatformCertificateIds:getTlsPlatformCertificateIds', __args__, opts=opts, typ=GetTlsPlatformCertificateIdsResult).value
 
     return AwaitableGetTlsPlatformCertificateIdsResult(
-        id=__ret__.id,
-        ids=__ret__.ids)
+        id=pulumi.get(__ret__, 'id'),
+        ids=pulumi.get(__ret__, 'ids'))
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_private_key.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_private_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,21 +158,21 @@
     __args__['keyType'] = key_type
     __args__['name'] = name
     __args__['publicKeySha1'] = public_key_sha1
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsPrivateKey:getTlsPrivateKey', __args__, opts=opts, typ=GetTlsPrivateKeyResult).value
 
     return AwaitableGetTlsPrivateKeyResult(
-        created_at=__ret__.created_at,
-        id=__ret__.id,
-        key_length=__ret__.key_length,
-        key_type=__ret__.key_type,
-        name=__ret__.name,
-        public_key_sha1=__ret__.public_key_sha1,
-        replace=__ret__.replace)
+        created_at=pulumi.get(__ret__, 'created_at'),
+        id=pulumi.get(__ret__, 'id'),
+        key_length=pulumi.get(__ret__, 'key_length'),
+        key_type=pulumi.get(__ret__, 'key_type'),
+        name=pulumi.get(__ret__, 'name'),
+        public_key_sha1=pulumi.get(__ret__, 'public_key_sha1'),
+        replace=pulumi.get(__ret__, 'replace'))
 
 
 @_utilities.lift_output_func(get_tls_private_key)
 def get_tls_private_key_output(created_at: Optional[pulumi.Input[Optional[str]]] = None,
                                id: Optional[pulumi.Input[Optional[str]]] = None,
                                key_length: Optional[pulumi.Input[Optional[int]]] = None,
                                key_type: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_private_key_ids.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_private_key_ids.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,9 +70,9 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsPrivateKeyIds:getTlsPrivateKeyIds', __args__, opts=opts, typ=GetTlsPrivateKeyIdsResult).value
 
     return AwaitableGetTlsPrivateKeyIdsResult(
-        id=__ret__.id,
-        ids=__ret__.ids)
+        id=pulumi.get(__ret__, 'id'),
+        ids=pulumi.get(__ret__, 'ids'))
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_subscription.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_subscription.py`

 * *Files 12% similar despite different names*

```diff
@@ -156,22 +156,22 @@
     __args__['configurationId'] = configuration_id
     __args__['domains'] = domains
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsSubscription:getTlsSubscription', __args__, opts=opts, typ=GetTlsSubscriptionResult).value
 
     return AwaitableGetTlsSubscriptionResult(
-        certificate_authority=__ret__.certificate_authority,
-        common_name=__ret__.common_name,
-        configuration_id=__ret__.configuration_id,
-        created_at=__ret__.created_at,
-        domains=__ret__.domains,
-        id=__ret__.id,
-        state=__ret__.state,
-        updated_at=__ret__.updated_at)
+        certificate_authority=pulumi.get(__ret__, 'certificate_authority'),
+        common_name=pulumi.get(__ret__, 'common_name'),
+        configuration_id=pulumi.get(__ret__, 'configuration_id'),
+        created_at=pulumi.get(__ret__, 'created_at'),
+        domains=pulumi.get(__ret__, 'domains'),
+        id=pulumi.get(__ret__, 'id'),
+        state=pulumi.get(__ret__, 'state'),
+        updated_at=pulumi.get(__ret__, 'updated_at'))
 
 
 @_utilities.lift_output_func(get_tls_subscription)
 def get_tls_subscription_output(certificate_authority: Optional[pulumi.Input[Optional[str]]] = None,
                                 configuration_id: Optional[pulumi.Input[Optional[str]]] = None,
                                 domains: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                                 id: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_tls_subscription_ids.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_tls_subscription_ids.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,9 +71,9 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsSubscriptionIds:getTlsSubscriptionIds', __args__, opts=opts, typ=GetTlsSubscriptionIdsResult).value
 
     return AwaitableGetTlsSubscriptionIdsResult(
-        id=__ret__.id,
-        ids=__ret__.ids)
+        id=pulumi.get(__ret__, 'id'),
+        ids=pulumi.get(__ret__, 'ids'))
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/get_waf_rules.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/get_waf_rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,20 +123,20 @@
     __args__['modsecRuleIds'] = modsec_rule_ids
     __args__['publishers'] = publishers
     __args__['tags'] = tags
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getWafRules:getWafRules', __args__, opts=opts, typ=GetWafRulesResult).value
 
     return AwaitableGetWafRulesResult(
-        exclude_modsec_rule_ids=__ret__.exclude_modsec_rule_ids,
-        id=__ret__.id,
-        modsec_rule_ids=__ret__.modsec_rule_ids,
-        publishers=__ret__.publishers,
-        rules=__ret__.rules,
-        tags=__ret__.tags)
+        exclude_modsec_rule_ids=pulumi.get(__ret__, 'exclude_modsec_rule_ids'),
+        id=pulumi.get(__ret__, 'id'),
+        modsec_rule_ids=pulumi.get(__ret__, 'modsec_rule_ids'),
+        publishers=pulumi.get(__ret__, 'publishers'),
+        rules=pulumi.get(__ret__, 'rules'),
+        tags=pulumi.get(__ret__, 'tags'))
 
 
 @_utilities.lift_output_func(get_waf_rules)
 def get_waf_rules_output(exclude_modsec_rule_ids: Optional[pulumi.Input[Optional[Sequence[int]]]] = None,
                          modsec_rule_ids: Optional[pulumi.Input[Optional[Sequence[int]]]] = None,
                          publishers: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                          tags: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/kvstore.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/kvstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/outputs.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10228,14 +10228,17 @@
 
     @property
     @pulumi.getter(name="geoHeaders")
     def geo_headers(self) -> Optional[bool]:
         """
         Injects Fastly-Geo-Country, Fastly-Geo-City, and Fastly-Geo-Region into the request headers
         """
+        warnings.warn("""'geo_headers' attribute has been deprecated and will be removed in the next major version release""", DeprecationWarning)
+        pulumi.log.warn("""geo_headers is deprecated: 'geo_headers' attribute has been deprecated and will be removed in the next major version release""")
+
         return pulumi.get(self, "geo_headers")
 
     @property
     @pulumi.getter(name="hashKeys")
     def hash_keys(self) -> Optional[str]:
         """
         Comma separated list of varnish request object fields that should be in the hash key
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/provider.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/service_acl_entries.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/service_acl_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/service_authorization.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/service_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/service_compute.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/service_compute.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/service_dictionary_items.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/service_dictionary_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/service_dynamic_snippet_content.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/service_dynamic_snippet_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/service_vcl.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/service_vcl.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/service_waf_configuration.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/service_waf_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/tls_activation.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/tls_certificate.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/tls_mutual_authentication.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/tls_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/tls_platform_certificate.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/tls_private_key.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/tls_subscription.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/tls_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,14 +283,17 @@
 
     @property
     @pulumi.getter(name="managedDnsChallenge")
     def managed_dns_challenge(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         The details required to configure DNS to respond to ACME DNS challenge in order to verify domain ownership.
         """
+        warnings.warn("""Use 'managed_dns_challenges' attribute instead""", DeprecationWarning)
+        pulumi.log.warn("""managed_dns_challenge is deprecated: Use 'managed_dns_challenges' attribute instead""")
+
         return pulumi.get(self, "managed_dns_challenge")
 
     @managed_dns_challenge.setter
     def managed_dns_challenge(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "managed_dns_challenge", value)
 
     @property
@@ -589,14 +592,17 @@
 
     @property
     @pulumi.getter(name="managedDnsChallenge")
     def managed_dns_challenge(self) -> pulumi.Output[Mapping[str, str]]:
         """
         The details required to configure DNS to respond to ACME DNS challenge in order to verify domain ownership.
         """
+        warnings.warn("""Use 'managed_dns_challenges' attribute instead""", DeprecationWarning)
+        pulumi.log.warn("""managed_dns_challenge is deprecated: Use 'managed_dns_challenges' attribute instead""")
+
         return pulumi.get(self, "managed_dns_challenge")
 
     @property
     @pulumi.getter(name="managedDnsChallenges")
     def managed_dns_challenges(self) -> pulumi.Output[Sequence['outputs.TlsSubscriptionManagedDnsChallenge']]:
         """
         A list of options for configuring DNS to respond to ACME DNS challenge in order to verify domain ownership.
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/tls_subscription_validation.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/tls_subscription_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly/user.py` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly.egg-info/PKG-INFO` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-fastly
-Version: 8.2.0a1687671288
+Version: 8.2.0a1688059197
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi fastly
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_fastly-8.2.0a1687671288/pulumi_fastly.egg-info/SOURCES.txt` & `pulumi_fastly-8.2.0a1688059197/pulumi_fastly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687671288/setup.py` & `pulumi_fastly-8.2.0a1688059197/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "8.2.0a1687671288"
-PLUGIN_VERSION = "8.2.0-alpha.1687671288+e8028a4e"
+VERSION = "8.2.0a1688059197"
+PLUGIN_VERSION = "8.2.0-alpha.1688059197+d3d8d176"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'fastly', PLUGIN_VERSION])
         except OSError as error:
```

