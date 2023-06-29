# Comparing `tmp/jaseci-1.4.1.1.tar.gz` & `tmp/jaseci-1.4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaseci-1.4.1.1.tar", last modified: Wed Jun 14 19:22:28 2023, max compression
+gzip compressed data, was "jaseci-1.4.1.2.tar", last modified: Thu Jun 29 13:58:11 2023, max compression
```

## Comparing `jaseci-1.4.1.1.tar` & `jaseci-1.4.1.2.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.274445 jaseci-1.4.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-14 19:22:28.274445 jaseci-1.4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.238444 jaseci-1.4.1.1/jaseci/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.238444 jaseci-1.4.1.1/jaseci/cli_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/cli_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/cli_tools/book_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/cli_tools/jsctl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.238444 jaseci-1.4.1.1/jaseci/cli_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/cli_tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21217 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/cli_tools/tests/test_jsctl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.238444 jaseci-1.4.1.1/jaseci/extens/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.242444 jaseci-1.4.1.1/jaseci/extens/act_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/jaseci.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/std.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/stripe.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.246444 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/std_test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_file_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_mail_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_net_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_std.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_std_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_webtool.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_zlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/webtool.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/act_lib/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.250444 jaseci-1.4.1.1/jaseci/extens/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/actions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/alias_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/architype_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/global_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/graph_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/jac_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/jsorc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/logger_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/master_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/object_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/prometheus_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/sentinel_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/super_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.254444 jaseci-1.4.1.1/jaseci/extens/api/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/test_architype_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/test_global_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/test_graph_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/test_logger_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/test_object_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/test_sentinel_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/tests/test_walker_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/walker_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/api/webhook_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.254444 jaseci-1.4.1.1/jaseci/extens/svc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/elastic_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/kube_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/mail_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/prome_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/redis_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/stripe_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/task_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/extens/svc/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.254444 jaseci-1.4.1.1/jaseci/jac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.258445 jaseci-1.4.1.1/jaseci/jac/interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/interpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/interpreter/architype_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    66659 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/interpreter/interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/interpreter/sentinel_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.258445 jaseci-1.4.1.1/jaseci/jac/interpreter/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/interpreter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/interpreter/tests/test_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/interpreter/walker_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.258445 jaseci-1.4.1.1/jaseci/jac/ir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/ast_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/jac_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.258445 jaseci-1.4.1.1/jaseci/jac/ir/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/passes/ast_prune_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/passes/codegen_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/passes/ir_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/passes/printer_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/passes/pt_prune_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/passes/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/ir/passes/stats_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jac.g4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.262445 jaseci-1.4.1.1/jaseci/jac/jac_parse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jac_parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34691 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jac_parse/jacLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    29031 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jac_parse/jacListener.py
--rw-r--r--   0 runner    (1001) docker     (123)   334026 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jac_parse/jacParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jac_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.262445 jaseci-1.4.1.1/jaseci/jac/jsci_vm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jsci_vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jsci_vm/disasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jsci_vm/inst_ptr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jsci_vm/machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jsci_vm/op_codes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.262445 jaseci-1.4.1.1/jaseci/jac/jsci_vm/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jsci_vm/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/jsci_vm/tests/test_codegen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.262445 jaseci-1.4.1.1/jaseci/jac/machine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/machine/jac_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/machine/jac_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/machine/machine_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.266445 jaseci-1.4.1.1/jaseci/jac/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/tests/book_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/tests/test_book.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jac/tests/test_lang_14.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.266445 jaseci-1.4.1.1/jaseci/jsorc/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/jsorc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/jsorc_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/jsorc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/live_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.266445 jaseci-1.4.1.1/jaseci/jsorc/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/manifests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/manifests/database.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   484138 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/manifests/elastic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37855 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/manifests/prometheus.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/manifests/redis.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/remote_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.266445 jaseci-1.4.1.1/jaseci/jsorc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/jsorc/tests/test_jsorc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.270445 jaseci-1.4.1.1/jaseci/prim/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/ability.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/architype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/element.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/master.py
--rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/obj_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/super_master.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/prim/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.274445 jaseci-1.4.1.1/jaseci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25194 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/jac_test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/jac_test_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/test_jac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    24345 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/test_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/tests/test_stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.274445 jaseci-1.4.1.1/jaseci/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.274445 jaseci-1.4.1.1/jaseci/utils/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/actions/actions_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/actions/actions_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/actions/actions_state.py
--rw-r--r--   0 runner    (1001) docker     (123)   119142 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/gprof2dot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/id_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/jaseci/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.238444 jaseci-1.4.1.1/jaseci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-14 19:22:28.000000 jaseci-1.4.1.1/jaseci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-14 19:22:28.000000 jaseci-1.4.1.1/jaseci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:22:28.000000 jaseci-1.4.1.1/jaseci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 19:22:28.000000 jaseci-1.4.1.1/jaseci.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-14 19:22:28.000000 jaseci-1.4.1.1/jaseci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 19:22:28.000000 jaseci-1.4.1.1/jaseci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 19:22:28.274445 jaseci-1.4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-14 19:22:11.000000 jaseci-1.4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.176623 jaseci-1.4.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-29 13:58:11.176623 jaseci-1.4.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.140623 jaseci-1.4.1.2/jaseci/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.140623 jaseci-1.4.1.2/jaseci/cli_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/cli_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/cli_tools/book_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/cli_tools/jsctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.140623 jaseci-1.4.1.2/jaseci/cli_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/cli_tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21217 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/cli_tools/tests/test_jsctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.140623 jaseci-1.4.1.2/jaseci/extens/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.144623 jaseci-1.4.1.2/jaseci/extens/act_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/jaseci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.148623 jaseci-1.4.1.2/jaseci/extens/act_lib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/tests/std_test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_mail_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_net_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_std_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_webtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_zlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/webtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/act_lib/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.152623 jaseci-1.4.1.2/jaseci/extens/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/actions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/alias_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/architype_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/global_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/graph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/jac_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/jsorc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/logger_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/master_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/object_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/prometheus_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/sentinel_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/super_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.152623 jaseci-1.4.1.2/jaseci/extens/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/tests/test_architype_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/tests/test_global_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/tests/test_graph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/tests/test_logger_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/tests/test_object_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/tests/test_sentinel_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/tests/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/tests/test_walker_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/walker_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/api/webhook_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.156623 jaseci-1.4.1.2/jaseci/extens/svc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/svc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/svc/elastic_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/svc/kube_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/svc/mail_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/svc/prome_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/svc/redis_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/svc/stripe_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/svc/task_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/extens/svc/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.156623 jaseci-1.4.1.2/jaseci/jac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.160623 jaseci-1.4.1.2/jaseci/jac/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/interpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/interpreter/architype_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66659 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/interpreter/interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/interpreter/sentinel_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.160623 jaseci-1.4.1.2/jaseci/jac/interpreter/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/interpreter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/interpreter/tests/test_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/interpreter/walker_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.160623 jaseci-1.4.1.2/jaseci/jac/ir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/ir/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/ir/ast_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/ir/jac_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.160623 jaseci-1.4.1.2/jaseci/jac/ir/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/ir/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/ir/passes/ast_prune_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/ir/passes/codegen_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/ir/passes/ir_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/ir/passes/printer_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/ir/passes/pt_prune_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/ir/passes/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/ir/passes/stats_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/jac.g4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.160623 jaseci-1.4.1.2/jaseci/jac/jac_parse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/jac_parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34691 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/jac_parse/jacLexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29031 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/jac_parse/jacListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)   334026 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/jac_parse/jacParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/jac_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.164623 jaseci-1.4.1.2/jaseci/jac/jsci_vm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/jsci_vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/jsci_vm/disasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/jsci_vm/inst_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/jsci_vm/machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/jsci_vm/op_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.164623 jaseci-1.4.1.2/jaseci/jac/jsci_vm/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/jsci_vm/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/jsci_vm/tests/test_codegen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.164623 jaseci-1.4.1.2/jaseci/jac/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/machine/jac_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/machine/jac_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/machine/machine_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.164623 jaseci-1.4.1.2/jaseci/jac/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/tests/book_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/tests/test_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jac/tests/test_lang_14.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.168623 jaseci-1.4.1.2/jaseci/jsorc/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jsorc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jsorc/jsorc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jsorc/jsorc_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jsorc/jsorc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jsorc/live_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.168623 jaseci-1.4.1.2/jaseci/jsorc/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jsorc/manifests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jsorc/manifests/database.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   484138 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jsorc/manifests/elastic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37855 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jsorc/manifests/prometheus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jsorc/manifests/redis.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jsorc/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jsorc/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jsorc/remote_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.168623 jaseci-1.4.1.2/jaseci/jsorc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jsorc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jsorc/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/jsorc/tests/test_jsorc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.172623 jaseci-1.4.1.2/jaseci/prim/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/prim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/prim/ability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/prim/architype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/prim/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/prim/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/prim/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/prim/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/prim/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/prim/obj_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/prim/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/prim/super_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/prim/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.172623 jaseci-1.4.1.2/jaseci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/tests/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25194 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/tests/jac_test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/tests/jac_test_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/tests/test_jac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24345 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/tests/test_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/tests/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/tests/test_stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.176623 jaseci-1.4.1.2/jaseci/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.176623 jaseci-1.4.1.2/jaseci/utils/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/utils/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/utils/actions/actions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/utils/actions/actions_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/utils/actions/actions_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119142 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/utils/gprof2dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/utils/id_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/utils/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/utils/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/jaseci/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:58:11.140623 jaseci-1.4.1.2/jaseci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-29 13:58:11.000000 jaseci-1.4.1.2/jaseci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-29 13:58:11.000000 jaseci-1.4.1.2/jaseci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:58:11.000000 jaseci-1.4.1.2/jaseci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-29 13:58:11.000000 jaseci-1.4.1.2/jaseci.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-29 13:58:11.000000 jaseci-1.4.1.2/jaseci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 13:58:11.000000 jaseci-1.4.1.2/jaseci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:58:11.176623 jaseci-1.4.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-29 13:57:47.000000 jaseci-1.4.1.2/setup.py
```

### Comparing `jaseci-1.4.1.1/LICENSE` & `jaseci-1.4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/__init__.py` & `jaseci-1.4.1.2/jaseci/__init__.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/cli_tools/book_tools.py` & `jaseci-1.4.1.2/jaseci/cli_tools/book_tools.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/cli_tools/jsctl.py` & `jaseci-1.4.1.2/jaseci/cli_tools/jsctl.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/cli_tools/tests/test_jsctl.py` & `jaseci-1.4.1.2/jaseci/cli_tools/tests/test_jsctl.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/date.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/date.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/elastic.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/elastic.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/file.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/file.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/jaseci.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/jaseci.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/net.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/net.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/rand.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/rand.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/regex.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/regex.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/request.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/request.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/std.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/std.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/stripe.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/stripe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,190 +1,237 @@
 """Built in actions for Jaseci"""
 import stripe as s
 
 from jaseci.jsorc.jsorc import JsOrc
+from jaseci.utils.utils import logger
 from jaseci.extens.svc.stripe_svc import StripeService
 from datetime import datetime
 from jaseci.jsorc.live_actions import jaseci_action
 
 
 def stripe() -> s:
-    return JsOrc.svc("stripe", StripeService).poke()
+    _stripe = JsOrc.svc("stripe", StripeService)
+    if _stripe.is_running():
+        return _stripe.app
+    else:
+        logger.info(
+            "Stripe service is not running! Fallback to direct stripe call with required api key params."
+        )
+        return s
 
 
 @jaseci_action()
-def create_product(name: str, description: str, **kwargs):
+def product_create(name: str, **kwargs):
     """create product"""
 
-    return stripe().Product.create(name=name, description=description, **kwargs)
+    return stripe().Product.create(name=name, **kwargs)
 
 
 @jaseci_action()
-def create_product_price(
-    productId: str,
-    amount: int,
+def price_create(
+    product: str,
+    unit_amount: int,
     currency: str,
-    recurring: dict = {},
     **kwargs,
 ):
-    """modify product price"""
+    """create product price"""
 
     return stripe().Price.create(
-        product=productId,
-        unit_amount=amount,
-        currency=currency,
-        **recurring if recurring else {},
-        **kwargs,
+        product=product, unit_amount=unit_amount, currency=currency, **kwargs
     )
 
 
 @jaseci_action()
-def product_list(detailed: bool = False, **kwargs):
+def product_list(**kwargs):
     """retrieve all producs"""
 
-    return stripe().Product.list(**{"active": True} if detailed else {}, **kwargs)
+    return stripe().Product.list(**kwargs)
 
 
 @jaseci_action()
-def create_customer(
-    email: str,
-    name: str,
-    address: dict = {},
-    **kwargs,
-):
+def customer_create(**kwargs):
     """create customer"""
 
-    return stripe().Customer.create(email=email, name=name, address=address, **kwargs)
+    return stripe().Customer.create(**kwargs)
 
 
 @jaseci_action()
-def get_customer(customer_id: str, **kwargs):
-    """retrieve customer information"""
+def customer_modify(customer_id: str, **kwargs):
+    """update customer"""
 
-    return stripe().Customer.retrieve(id=customer_id, **kwargs)
+    return stripe().Customer.modify(customer_id, **kwargs)
 
 
 @jaseci_action()
-def attach_payment_method(payment_method_id: str, customer_id: str, **kwargs):
-    """attach payment method to customer"""
+def customer_retrieve(customer_id: str, **kwargs):
+    """retrieve customer information"""
 
-    paymentMethods = get_payment_methods(customer_id)
+    return stripe().Customer.retrieve(customer_id, **kwargs)
 
-    paymentMethod = stripe().PaymentMethod.attach(
-        payment_method=payment_method_id, customer=customer_id, **kwargs
-    )
 
-    is_default = True
-    if paymentMethods.get("data"):
-        update_default_payment_method(customer_id, payment_method_id)
-        is_default = False
-
-    paymentMethod["is_default"] = is_default
+@jaseci_action()
+def payment_method_attach(payment_method_id: str, customer_id: str, **kwargs):
+    """retrieve customer list of invoices"""
 
-    return paymentMethod
+    return stripe().PaymentMethod.attach(
+        payment_method_id, customer=customer_id, **kwargs
+    )
 
 
 @jaseci_action()
-def detach_payment_method(payment_method_id: str, **kwargs):
+def payment_method_detach(payment_method_id: str, **kwargs):
     """detach payment method from customer"""
 
-    return stripe().PaymentMethod.detach(payment_method=payment_method_id, **kwargs)
+    return stripe().PaymentMethod.detach(payment_method_id, **kwargs)
 
 
 @jaseci_action()
-def get_payment_methods(customer_id: str, **kwargs):
+def payment_method_list(**kwargs):
     """get customer list of payment methods"""
 
-    return stripe().PaymentMethod.list(customer=customer_id, type="card", **kwargs)
+    return stripe().PaymentMethod.list(**kwargs)
 
 
 @jaseci_action()
-def update_default_payment_method(customer_id: str, payment_method_id: str, **kwargs):
-    """update default payment method of customer"""
+def invoice_create(**kwargs):
+    """create customer invoice"""
 
-    return stripe().Customer.modify(
-        sid=customer_id,
-        invoice_settings={"default_payment_method": payment_method_id},
-        **kwargs,
-    )
+    return stripe().Invoice.create(**kwargs)
 
 
 @jaseci_action()
-def create_invoice(customer_id: str, **kwargs):
-    """create customer invoice"""
+def invoice_list(**kwargs):
+    """retrieve customer list of invoices"""
 
-    return stripe().Invoice.create(customer=customer_id, **kwargs)
+    return stripe().Invoice.list(**kwargs)
 
 
 @jaseci_action()
-def get_invoice_list(
-    customer_id: str,
-    subscription_id: str,
-    starting_after: str = "",
-    limit: int = 10,
-    **kwargs,
+def payment_intent_list(**kwargs):
+    """get customer payment intents"""
+
+    return stripe().PaymentIntent.list(**kwargs)
+
+
+@jaseci_action()
+def payment_intent_create(amount: int, currency: str, **kwargs):
+    """Create customer payment"""
+
+    return stripe().PaymentIntent.create(amount=amount, currency=currency, **kwargs)
+
+
+@jaseci_action()
+def subscription_create(customer: str, items: list, **kwargs):
+    """create subcriptions"""
+
+    return stripe().Subscription.create(customer=customer, items=items, **kwargs)
+
+
+@jaseci_action()
+def subscription_modify(subscription_id: str, **kwargs):
+    """modify subcriptions"""
+
+    return stripe().Subscription.modify(subscription_id, **kwargs)
+
+
+@jaseci_action()
+def subscription_list(**kwargs):
+    """list all customer's subcriptions"""
+
+    return stripe().Subscription.list(**kwargs)
+
+
+@jaseci_action()
+def subscription_retrieve(subscription_id: str, **kwargs):
+    """retrieve customer subcription details"""
+
+    return stripe().Subscription.retrieve(subscription_id, **kwargs)
+
+
+@jaseci_action()
+def payment_method_create(type: str, **kwargs):
+    """create payment method"""
+
+    return stripe().PaymentMethod.create(type=type, **kwargs)
+
+
+@jaseci_action()
+def subscription_delete(subscription_id: str, **kwargs):
+    """cancel customer subscription"""
+
+    return stripe().Subscription.delete(subscription_id, **kwargs)
+
+
+@jaseci_action()
+def invoice_retrieve(invoice_id: str, **kwargs):
+    """get invoice information"""
+
+    return stripe().Invoice.retrieve(invoice_id, **kwargs)
+
+
+@jaseci_action()
+def subscription_item_create_usage_record(
+    subscription_item_id: str, quantity: int, **kwargs
 ):
-    """retrieve customer list of invoices"""
+    """Create usage record"""
 
-    return stripe().Invoice.list(
-        customer=customer_id,
-        limit=limit,
-        subscription=subscription_id,
-        **{"starting_after": starting_after} if starting_after else {},
-        **kwargs,
+    return stripe().SubscriptionItem.create_usage_record(
+        subscription_item_id, quantity=quantity, timestamp=datetime.now(), **kwargs
     )
 
 
 @jaseci_action()
-def get_payment_intents(
-    customer_id: str, starting_after: str = "", limit: int = 10, **kwargs
-):
-    """get customer payment intents"""
+def checkout_session_create(success_url: str, mode: str, **kwargs):
+    return stripe().checkout.Session.create(
+        success_url=success_url,
+        mode=mode,
+        **kwargs,
+    )
+
 
-    return stripe().PaymentIntent.list(
-        customer=customer_id,
-        limit=limit,
-        **{"starting_after": starting_after} if starting_after else {},
+@jaseci_action()
+def billing_portal_session_create(customer: str, **kwargs):
+    return stripe().billing_portal.Session.create(
+        customer=customer,
         **kwargs,
     )
 
 
+#################################################
+#            WITH PRE CUSTOM PROCESS            #
+#################################################
+
+
 @jaseci_action()
-def create_payment_intents(
-    customer_id: str,
-    amount: int,
-    currency: str,
-    payment_method_types: list = ["card"],
-    **kwargs,
-):
-    """Create customer payment"""
+def update_default_payment_method(customer_id: str, payment_method_id: str, **kwargs):
+    """update default payment method of customer"""
 
-    return stripe().PaymentIntent.create(
-        customer=customer_id,
-        amount=amount,
-        currency=currency,
-        payment_method_types=payment_method_types,
+    return customer_modify(
+        customer_id,
+        invoice_settings={"default_payment_method": payment_method_id},
         **kwargs,
     )
 
 
 @jaseci_action()
-def get_customer_subscription(customer_id: str, **kwargs):
-    """retrieve customer subcription list"""
+def attach_payment_method(payment_method_id: str, customer_id: str, **kwargs):
+    """attach payment method to customer"""
 
-    return stripe().Subscription.list(customer=customer_id, **kwargs)
+    paymentMethods = payment_method_list(customer=customer_id)
 
+    paymentMethod = payment_method_attach(payment_method_id, customer_id, **kwargs)
 
-@jaseci_action()
-def create_payment_method(card_type: str, card: dict, billing_details: dict, **kwargs):
-    """create payment method"""
+    is_default = True
+    if paymentMethods.get("data"):
+        update_default_payment_method(customer_id, payment_method_id)
+        is_default = False
 
-    return stripe().PaymentMethod.create(
-        type=card_type, card=card, billing_details=billing_details, **kwargs
-    )
+    paymentMethod["is_default"] = is_default
+
+    return paymentMethod
 
 
 @jaseci_action()
 def create_trial_subscription(
     customer_id: str,
     items: list,
     payment_method_id: str = "",
@@ -196,17 +243,17 @@
     if payment_method_id != "":
         # attach payment method to customer
         attach_payment_method(payment_method_id, customer_id)
 
         # set card to default payment method
         update_default_payment_method(customer_id, payment_method_id)
 
-    return stripe().Subscription.create(
-        customer=customer_id,
-        items=items,
+    return subscription_create(
+        customer_id,
+        items,
         trial_period_days=trial_period_days,
         **kwargs,
     )
 
 
 @jaseci_action()
 def create_subscription(
@@ -220,77 +267,39 @@
     if payment_method_id != "":
         # attach payment method to customer
         attach_payment_method(payment_method_id, customer_id)
 
         # set card to default payment method
         update_default_payment_method(customer_id, payment_method_id)
 
-    return stripe().Subscription.create(customer=customer_id, items=items, **kwargs)
-
-
-@jaseci_action()
-def cancel_subscription(subscription_id: str, **kwargs):
-    """cancel customer subscription"""
-
-    return stripe().Subscription.delete(sid=subscription_id, **kwargs)
-
-
-@jaseci_action()
-def get_subscription(subscription_id: str, **kwargs):
-    """retrieve customer subcription details"""
-
-    return stripe().Subscription.retrieve(id=subscription_id, **kwargs)
+    return subscription_create(customer_id, items, **kwargs)
 
 
 @jaseci_action()
 def update_subscription_item(
     subscription_id: str, subscription_item_id: str, price_id: str, **kwargs
 ):
     """update subcription details"""
 
-    return stripe().Subscription.modify(
-        sid=subscription_id,
+    return subscription_modify(
+        subscription_id,
         cancel_at_period_end=False,
         items=[
             {
                 "id": subscription_item_id,
                 "price": price_id,
             },
         ],
         **kwargs,
     )
 
 
-@jaseci_action()
-def get_invoice(invoice_id: str, **kwargs):
-    """get invoice information"""
-
-    return stripe().Invoice.retrieve(id=invoice_id, **kwargs)
-
-
-@jaseci_action()
-def create_usage_report(subscription_item_id: str, quantity: int, **kwargs):
-    """Create usage record"""
-
-    return stripe().SubscriptionItem.create_usage_record(
-        id=subscription_item_id, quantity=quantity, timestamp=datetime.now(), **kwargs
-    )
-
-
-@jaseci_action()
-def create_checkout_session(
-    success_url: str, cancel_url: str, line_items: list, mode: str, **kwargs
-):
-    return stripe().checkout.Session.create(
-        success_url=success_url,
-        cancel_url=cancel_url,
-        line_items=line_items,
-        mode=mode,
-        **kwargs,
-    )
+#################################################
+#            EXECUTE CUSTOM PROCESS             #
+#################################################
 
 
 @jaseci_action()
 def exec(api: str, *args, **kwargs):
     apis = api.split(".")
 
     if not apis:
```

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/std_test_code.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/tests/std_test_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_date.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_elastic.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_elastic.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_file_lib.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_file_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_mail_lib.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_mail_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_net_lib.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_net_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_regex.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_std.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_std.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_std_lib.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_std_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_url.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_vector.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_webtool.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_webtool.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/tests/test_zlib.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/tests/test_zlib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/url.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/url.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/vector.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/vector.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/webtool.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/webtool.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/act_lib/zip.py` & `jaseci-1.4.1.2/jaseci/extens/act_lib/zip.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/actions_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/actions_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/alias_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/alias_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/architype_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/architype_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/config_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/config_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/global_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/global_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/graph_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/graph_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/interface.py` & `jaseci-1.4.1.2/jaseci/extens/api/interface.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/jac_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/jac_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/jsorc_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/jsorc_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/logger_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/logger_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/master_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/master_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/object_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/object_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/prometheus_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/prometheus_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/queue_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/queue_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/sentinel_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/sentinel_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/super_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/super_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/tests/test_architype_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/tests/test_architype_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/tests/test_global_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/tests/test_global_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/tests/test_graph_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/tests/test_graph_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/tests/test_logger_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/tests/test_logger_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/tests/test_object_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/tests/test_object_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/tests/test_sentinel_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/tests/test_sentinel_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/tests/test_user_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/tests/test_user_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/tests/test_walker_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/tests/test_walker_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/user_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/user_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     def user_create(
         self,
         name: str,
         password: str = "",
         global_init: str = "",
         global_init_ctx: dict = {},
         other_fields: dict = {},
+        send_email: bool = False,
     ):
         """
         Create a new user (master object)
 
         This API is used to create users and optionally set them up with a graph and
         related initialization. In the context of
         JSCTL, any name is sufficient and no additional information is required.
@@ -56,15 +57,15 @@
         :param global_init_ctx: Context to preload for the initialization walker
         :param other_fields: This parameter is used for additional fields required for
             overloaded interfaces. This parameter is not used in JSCTL, but is used
             by Jaseci server for the additional parameters of password, is_activated,
             and is_superuser.
         """
         ret = {}
-        mast = self.user_creator(name, password, other_fields)
+        mast = self.user_creator(name, password, other_fields, send_email)
         if type(mast) is dict:  # in case of upstream error
             return mast
         ret["user"] = mast.serialize()
         self.seek_committer(mast)
         if len(global_init):
             ret["global_init"] = self.user_global_init(
                 mast, global_init, global_init_ctx
@@ -98,15 +99,17 @@
         """
         ret = {}
         ret["success"] = self.user_destroyer(self.name)
         if not ret["success"]:
             ret["status_code"] = 400
         return ret
 
-    def user_creator(self, name, password: str = "", other_fields: dict = {}):
+    def user_creator(
+        self, name, password: str = "", other_fields: dict = {}, send_email=True
+    ):
         """
         Abstraction for user creation for elegant overriding
         """
 
         return JsOrc.master(h=self._h, name=name)
 
     def superuser_creator(self, name, password: str = "", other_fields: dict = {}):
```

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/walker_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/walker_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/api/webhook_api.py` & `jaseci-1.4.1.2/jaseci/extens/api/webhook_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,31 +31,39 @@
 
             if customer_id:
                 customer = stripe.Customer.retrieve(id=customer_id)
                 metadata = customer.get("metadata")
             else:
                 metadata = payload_obj.get("metadata")
 
-            master_id = metadata.get("master_id")
+            master_id = metadata.get("master")
             master = self._h.get_obj(master_id, master_id)
 
             node_id = metadata.get("node")
             if not node_id:
                 node_id = master.active_gph_id
-
             node = self._h.get_obj(master_id, node_id)
 
-            global_snt_id = self._h.get_glob("GLOB_SENTINEL")
-            global_snt = self._h.get_obj(master_id, global_snt_id)
+            sentinel_id = (
+                metadata.get("sentinel")
+                or master.active_snt_id
+                or self._h.get_glob("GLOB_SENTINEL")
+            )
+            sentinel = self._h.get_obj(
+                master_id,
+                self._h.get_glob("GLOB_SENTINEL")
+                if sentinel_id == "global"
+                else sentinel_id,
+            )
 
             payload = {"event": req_body}
             self.seek_committer(master)
 
             wlk = stripe_service.get_walker(req_body["type"])
 
             return master.walker_run(
-                name=wlk, nd=node, ctx=payload, _req_ctx=_req_ctx, snt=global_snt
+                name=wlk, nd=node, ctx=payload, _req_ctx=_req_ctx, snt=sentinel
             )
         else:
             raise HTTPException(
                 status_code=400, detail=str(type + " webhook is not yet supported")
             )
```

### Comparing `jaseci-1.4.1.1/jaseci/extens/svc/elastic_svc.py` & `jaseci-1.4.1.2/jaseci/extens/svc/elastic_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/svc/kube_svc.py` & `jaseci-1.4.1.2/jaseci/extens/svc/kube_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/svc/mail_svc.py` & `jaseci-1.4.1.2/jaseci/extens/svc/mail_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/svc/prome_svc.py` & `jaseci-1.4.1.2/jaseci/extens/svc/prome_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/svc/redis_svc.py` & `jaseci-1.4.1.2/jaseci/extens/svc/redis_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/svc/stripe_svc.py` & `jaseci-1.4.1.2/jaseci/extens/svc/stripe_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/svc/task_svc.py` & `jaseci-1.4.1.2/jaseci/extens/svc/task_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/extens/svc/tasks.py` & `jaseci-1.4.1.2/jaseci/extens/svc/tasks.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/interpreter/architype_interp.py` & `jaseci-1.4.1.2/jaseci/jac/interpreter/architype_interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/interpreter/interp.py` & `jaseci-1.4.1.2/jaseci/jac/interpreter/interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/interpreter/sentinel_interp.py` & `jaseci-1.4.1.2/jaseci/jac/interpreter/sentinel_interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/interpreter/tests/test_interp.py` & `jaseci-1.4.1.2/jaseci/jac/interpreter/tests/test_interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/interpreter/walker_interp.py` & `jaseci-1.4.1.2/jaseci/jac/interpreter/walker_interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/ir/ast.py` & `jaseci-1.4.1.2/jaseci/jac/ir/ast.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/ir/ast_builder.py` & `jaseci-1.4.1.2/jaseci/jac/ir/ast_builder.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/ir/jac_code.py` & `jaseci-1.4.1.2/jaseci/jac/ir/jac_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/ir/passes/codegen_pass.py` & `jaseci-1.4.1.2/jaseci/jac/ir/passes/codegen_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/ir/passes/ir_pass.py` & `jaseci-1.4.1.2/jaseci/jac/ir/passes/ir_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/ir/passes/printer_pass.py` & `jaseci-1.4.1.2/jaseci/jac/ir/passes/printer_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/ir/passes/pt_prune_pass.py` & `jaseci-1.4.1.2/jaseci/jac/ir/passes/pt_prune_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/ir/passes/schedule.py` & `jaseci-1.4.1.2/jaseci/jac/ir/passes/schedule.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/jac.g4` & `jaseci-1.4.1.2/jaseci/jac/jac.g4`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/jac_parse/jacLexer.py` & `jaseci-1.4.1.2/jaseci/jac/jac_parse/jacLexer.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/jac_parse/jacListener.py` & `jaseci-1.4.1.2/jaseci/jac/jac_parse/jacListener.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/jac_parse/jacParser.py` & `jaseci-1.4.1.2/jaseci/jac/jac_parse/jacParser.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/jac_set.py` & `jaseci-1.4.1.2/jaseci/jac/jac_set.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/jsci_vm/disasm.py` & `jaseci-1.4.1.2/jaseci/jac/jsci_vm/disasm.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/jsci_vm/inst_ptr.py` & `jaseci-1.4.1.2/jaseci/jac/jsci_vm/inst_ptr.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/jsci_vm/machine.py` & `jaseci-1.4.1.2/jaseci/jac/jsci_vm/machine.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/jsci_vm/op_codes.py` & `jaseci-1.4.1.2/jaseci/jac/jsci_vm/op_codes.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/jsci_vm/tests/test_codegen.py` & `jaseci-1.4.1.2/jaseci/jac/jsci_vm/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/machine/jac_scope.py` & `jaseci-1.4.1.2/jaseci/jac/machine/jac_scope.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/machine/jac_value.py` & `jaseci-1.4.1.2/jaseci/jac/machine/jac_value.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/machine/machine_state.py` & `jaseci-1.4.1.2/jaseci/jac/machine/machine_state.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/tests/book_code.py` & `jaseci-1.4.1.2/jaseci/jac/tests/book_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/tests/test_book.py` & `jaseci-1.4.1.2/jaseci/jac/tests/test_book.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jac/tests/test_lang_14.py` & `jaseci-1.4.1.2/jaseci/jac/tests/test_lang_14.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jsorc/jsorc.py` & `jaseci-1.4.1.2/jaseci/jsorc/jsorc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jsorc/jsorc_settings.py` & `jaseci-1.4.1.2/jaseci/jsorc/jsorc_settings.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jsorc/jsorc_utils.py` & `jaseci-1.4.1.2/jaseci/jsorc/jsorc_utils.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jsorc/live_actions.py` & `jaseci-1.4.1.2/jaseci/jsorc/live_actions.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jsorc/manifests/database.yaml` & `jaseci-1.4.1.2/jaseci/jsorc/manifests/database.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jsorc/manifests/elastic.yaml` & `jaseci-1.4.1.2/jaseci/jsorc/manifests/elastic.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jsorc/manifests/prometheus.yaml` & `jaseci-1.4.1.2/jaseci/jsorc/manifests/prometheus.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jsorc/manifests/redis.yaml` & `jaseci-1.4.1.2/jaseci/jsorc/manifests/redis.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jsorc/memory.py` & `jaseci-1.4.1.2/jaseci/jsorc/memory.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jsorc/redis.py` & `jaseci-1.4.1.2/jaseci/jsorc/redis.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jsorc/remote_actions.py` & `jaseci-1.4.1.2/jaseci/jsorc/remote_actions.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jsorc/tests/test_actions.py` & `jaseci-1.4.1.2/jaseci/jsorc/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/jsorc/tests/test_jsorc.py` & `jaseci-1.4.1.2/jaseci/jsorc/tests/test_jsorc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/prim/ability.py` & `jaseci-1.4.1.2/jaseci/prim/ability.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/prim/architype.py` & `jaseci-1.4.1.2/jaseci/prim/architype.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/prim/edge.py` & `jaseci-1.4.1.2/jaseci/prim/edge.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/prim/element.py` & `jaseci-1.4.1.2/jaseci/prim/element.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/prim/graph.py` & `jaseci-1.4.1.2/jaseci/prim/graph.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/prim/master.py` & `jaseci-1.4.1.2/jaseci/prim/master.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/prim/node.py` & `jaseci-1.4.1.2/jaseci/prim/node.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/prim/obj_mixins.py` & `jaseci-1.4.1.2/jaseci/prim/obj_mixins.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/prim/sentinel.py` & `jaseci-1.4.1.2/jaseci/prim/sentinel.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/prim/super_master.py` & `jaseci-1.4.1.2/jaseci/prim/super_master.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/prim/walker.py` & `jaseci-1.4.1.2/jaseci/prim/walker.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/tests/infer.py` & `jaseci-1.4.1.2/jaseci/tests/infer.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/tests/jac_test_code.py` & `jaseci-1.4.1.2/jaseci/tests/jac_test_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/tests/jac_test_progs.py` & `jaseci-1.4.1.2/jaseci/tests/jac_test_progs.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/tests/test_core.py` & `jaseci-1.4.1.2/jaseci/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/tests/test_jac.py` & `jaseci-1.4.1.2/jaseci/tests/test_jac.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/tests/test_node.py` & `jaseci-1.4.1.2/jaseci/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/tests/test_progs.py` & `jaseci-1.4.1.2/jaseci/tests/test_progs.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/tests/test_stack.py` & `jaseci-1.4.1.2/jaseci/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/tests/test_stripe.py` & `jaseci-1.4.1.2/jaseci/tests/test_stripe.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,29 +39,30 @@
         stripe.Subscription.create = Mock()
         stripe.Subscription.delete = Mock()
         stripe.Subscription.retrieve = Mock()
         stripe.Subscription.modify = Mock()
         stripe.Invoice.retrieve = Mock()
         stripe.SubscriptionItem.create_usage_record = Mock()
         stripe.checkout.Session.create = Mock()
+        stripe.billing_portal.Session.create = Mock()
 
     @classmethod
     def tearDownClass(cls):
         super(StripeTests, cls).tearDownClass()
 
     @jac_testcase("stripe.jac", "create_product")
     def test_stripe_create_product(self, ret):
         stripe.Product.create.assert_called_once_with(
             name="product1", description="new product"
         )
 
     @jac_testcase("stripe.jac", "create_product_price")
     def test_stripe_create_product_price(self, ret):
         stripe.Price.create.assert_called_once_with(
-            product="product1", unit_amount=12, currency="usd"
+            product="product1", unit_amount=12, currency="usd", recurring={}
         )
 
     @jac_testcase("stripe.jac", "product_list")
     def test_stripe_product_list(self, ret):
         stripe.Product.list.assert_called_once_with(active=True)
 
     @jac_testcase("stripe.jac", "create_customer")
@@ -70,80 +71,71 @@
             email="test12@gmail.com",
             name="stripe customer",
             address={"billing_address": "123 metro manila"},
         )
 
     @jac_testcase("stripe.jac", "get_customer")
     def test_stripe_get_customer(self, ret):
-        stripe.Customer.retrieve.assert_called_once_with(id="cus_NBsqL1C1GrrHYM")
+        stripe.Customer.retrieve.assert_called_once_with("cus_NBsqL1C1GrrHYM")
 
     @jac_testcase("stripe.jac", "attach_payment_method")
     def test_stripe_attach_payment_method(self, ret):
-        stripe.PaymentMethod.list.assert_called_once_with(
-            customer="cus_NBsqL1C1GrrHYM", type="card"
-        )
+        stripe.PaymentMethod.list.assert_called_once_with(customer="cus_NBsqL1C1GrrHYM")
 
         stripe.PaymentMethod.attach.assert_called_once_with(
-            payment_method="pm_1MN1iN2xToAoV8chTjvX94hm", customer="cus_NBsqL1C1GrrHYM"
+            "pm_1MN1iN2xToAoV8chTjvX94hm", customer="cus_NBsqL1C1GrrHYM"
         )
 
     @jac_testcase("stripe.jac", "detach_payment_method")
     def test_stripe_detach_payment_method(self, ret):
         stripe.PaymentMethod.detach.assert_called_once_with(
-            payment_method="pm_1MN1iN2xToAoV8chTjvX94hm"
+            "pm_1MN1iN2xToAoV8chTjvX94hm"
         )
 
     @jac_testcase("stripe.jac", "get_payment_methods")
     def test_stripe_get_payment_methods(self, ret):
-        stripe.PaymentMethod.list.assert_called_with(
-            customer="cus_NBsqL1C1GrrHYM", type="card"
-        )
+        stripe.PaymentMethod.list.assert_called_with(customer="cus_NBsqL1C1GrrHYM")
 
     @jac_testcase("stripe.jac", "update_default_payment_method")
     def test_stripe_update_default_payment_method(self, ret):
         stripe.Customer.modify.assert_called_with(
-            sid="cus_NBsqL1C1GrrHYM",
+            "cus_NBsqL1C1GrrHYM",
             invoice_settings={"default_payment_method": "pm_1MN1iN2xToAoV8chTjvX94hm"},
         )
 
     @jac_testcase("stripe.jac", "create_invoice")
     def test_stripe_create_invoice(self, ret):
         stripe.Customer.modify.assert_called_once_with(
-            sid="cus_NBsqL1C1GrrHYM",
+            "cus_NBsqL1C1GrrHYM",
             invoice_settings={"default_payment_method": "pm_1MN1iN2xToAoV8chTjvX94hm"},
         )
 
     @jac_testcase("stripe.jac", "get_invoice_list")
     def test_stripe_get_invoice_list(self, ret):
         stripe.Invoice.list.assert_called_once_with(
             customer="cus_NBsqL1C1GrrHYM",
-            limit=10,
             subscription="sub_1MTgMQCZO78n7fsZqu1dk6nD",
         )
 
     @jac_testcase("stripe.jac", "get_payment_intents")
     def test_stripe_get_payment_intents(self, ret):
-        stripe.PaymentIntent.list.assert_called_once_with(
-            customer="cus_NBsqL1C1GrrHYM", limit=10
-        )
+        stripe.PaymentIntent.list.assert_called_once_with(customer="cus_NBsqL1C1GrrHYM")
 
     @jac_testcase("stripe.jac", "create_payment_intents")
     def test_stripe_create_payment_intents(self, ret):
         stripe.PaymentIntent.create.assert_called_once_with(
-            customer="cus_NBsqL1C1GrrHYM",
             amount=12,
             currency="usd",
+            customer="cus_NBsqL1C1GrrHYM",
             payment_method_types=["card"],
         )
 
     @jac_testcase("stripe.jac", "get_customer_subscription")
     def test_stripe_get_customer_subscription(self, ret):
-        stripe.Subscription.list.assert_called_once_with(
-            customer="sub_1MTgMQCZO78n7fsZqu1dk6nD"
-        )
+        stripe.Subscription.list.assert_called_once_with(customer="customer_id")
 
     @jac_testcase("stripe.jac", "create_payment_method")
     def test_stripe_create_payment_method(self, ret):
         stripe.PaymentMethod.create.assert_called_once_with(
             type="card",
             card={
                 "number": "4242424242424242",
@@ -168,47 +160,51 @@
             customer="cus_NBsqL1C1GrrHYM",
             items=[{"price": "price_1MR9T6CZO78n7fsZmNdIJplr"}],
         )
 
     @jac_testcase("stripe.jac", "cancel_subscription")
     def test_stripe_cancel_subscription(self, ret):
         stripe.Subscription.delete.assert_called_once_with(
-            sid="sub_1MTgMQCZO78n7fsZqu1dk6nD"
+            "sub_1MTgMQCZO78n7fsZqu1dk6nD"
         )
 
     @jac_testcase("stripe.jac", "get_subscription")
     def test_stripe_get_subscription(self, ret):
         stripe.Subscription.retrieve.assert_called_once_with(
-            id="sub_1MTgMQCZO78n7fsZqu1dk6nD"
+            "sub_1MTgMQCZO78n7fsZqu1dk6nD"
         )
 
     @jac_testcase("stripe.jac", "update_subscription_item")
     def test_stripe_update_subscription_item(self, ret):
         stripe.Subscription.modify.assert_called_once_with(
-            sid="sub_1MTgMQCZO78n7fsZqu1dk6nD",
+            "sub_1MTgMQCZO78n7fsZqu1dk6nD",
             cancel_at_period_end=False,
             items=[
                 {
                     "id": "su_1MTgMQCZO78n7fsZqu1dk6nD",
                     "price": "price_1MTgMQCZO78n7fsZqu1dk6nD",
                 }
             ],
         )
 
     @jac_testcase("stripe.jac", "get_invoice")
     def test_stripe_get_invoice(self, ret):
-        stripe.Invoice.retrieve.assert_called_once_with(
-            id="inv_1MTgMQCZO78n7fsZqu1dk6nD"
-        )
+        stripe.Invoice.retrieve.assert_called_once_with("inv_1MTgMQCZO78n7fsZqu1dk6nD")
 
     @jac_testcase("stripe.jac", "create_usage_report")
     def test_stripe_create_usage_report(self, ret):
         stripe.SubscriptionItem.create_usage_record.assert_called()
 
     @jac_testcase("stripe.jac", "create_checkout_session")
     def test_stripe_create_checkout_session(self, ret):
         stripe.checkout.Session.create.assert_called_once_with(
             success_url="https://example.com/success",
-            cancel_url="https://example.com/cancel",
-            line_items=[{"price": "price_H5ggYwtDq4fbrJ", "quantity": 12}],
             mode="payment",
+            line_items=[{"price": "price_H5ggYwtDq4fbrJ", "quantity": 12}],
+            cancel_url="https://example.com/cancel",
+        )
+
+    @jac_testcase("stripe.jac", "create_billing_portal_session")
+    def test_stripe_create_billing_portal_session(self, ret):
+        stripe.billing_portal.Session.create.assert_called_once_with(
+            customer="cus_O7ECcoZCZFwinb", return_url="https://example.com/account"
         )
```

### Comparing `jaseci-1.4.1.1/jaseci/utils/actions/actions_manager.py` & `jaseci-1.4.1.2/jaseci/utils/actions/actions_manager.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/utils/actions/actions_optimizer.py` & `jaseci-1.4.1.2/jaseci/utils/actions/actions_optimizer.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/utils/actions/actions_state.py` & `jaseci-1.4.1.2/jaseci/utils/actions/actions_state.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/utils/gprof2dot.py` & `jaseci-1.4.1.2/jaseci/utils/gprof2dot.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/utils/id_list.py` & `jaseci-1.4.1.2/jaseci/utils/id_list.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/utils/json_handler.py` & `jaseci-1.4.1.2/jaseci/utils/json_handler.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/utils/log_utils.py` & `jaseci-1.4.1.2/jaseci/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/utils/test_core.py` & `jaseci-1.4.1.2/jaseci/utils/test_core.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci/utils/utils.py` & `jaseci-1.4.1.2/jaseci/utils/utils.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/jaseci.egg-info/SOURCES.txt` & `jaseci-1.4.1.2/jaseci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.1/setup.py` & `jaseci-1.4.1.2/setup.py`

 * *Files identical despite different names*

