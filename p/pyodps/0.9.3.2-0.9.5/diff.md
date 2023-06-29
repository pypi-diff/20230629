# Comparing `tmp/pyodps-0.9.3.2.tar.gz` & `tmp/pyodps-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyodps-0.9.3.2.tar", last modified: Sat Aug 22 08:26:00 2020, max compression
+gzip compressed data, was "dist\pyodps-0.9.5.tar", last modified: Sun Sep  6 13:27:26 2020, max compression
```

## Comparing `pyodps-0.9.3.2.tar` & `pyodps-0.9.5.tar`

### file list

```diff
@@ -1,426 +1,431 @@
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/cupid/
--rw-rw-rw-   0        0        0     1597 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/config.py
--rw-rw-rw-   0        0        0     1864 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/errors.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/cupid/io/
--rw-rw-rw-   0        0        0     1833 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/io/kvstore.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/cupid/io/table/
--rw-rw-rw-   0        0        0    16260 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/io/table/core.py
--rw-rw-rw-   0        0        0     4701 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/io/table/pd.py
--rw-rw-rw-   0        0        0     6941 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/io/table/record.py
--rw-rw-rw-   0        0        0      827 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/io/table/__init__.py
--rw-rw-rw-   0        0        0      713 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/io/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/cupid/proto/
--rw-rw-rw-   0        0        0    91635 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/proto/cupidtaskparam_pb2.py
--rw-rw-rw-   0        0        0     5164 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/proto/cupid_process_service_pb2.py
--rw-rw-rw-   0        0        0    28609 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/proto/cupid_subprocess_service_pb2.py
--rw-rw-rw-   0        0        0    48395 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/proto/cupid_task_service_pb2.py
--rw-rw-rw-   0        0        0     7228 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/proto/kv_store_service_pb2.py
--rw-rw-rw-   0        0        0        0 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/proto/__init__.py
--rw-rw-rw-   0        0        0     8243 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/rpc.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/cupid/runtime/
--rw-rw-rw-   0        0        0    17571 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/runtime/ctypes_libs.py
--rw-rw-rw-   0        0        0     3403 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/runtime/runtime.py
--rw-rw-rw-   0        0        0     2976 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/runtime/runtime_test.py
--rw-rw-rw-   0        0        0      642 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/runtime/__init__.py
--rw-rw-rw-   0        0        0     8520 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/session.py
--rw-rw-rw-   0        0        0     1283 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/utils.py
--rw-rw-rw-   0        0        0      649 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/_version.py
--rw-rw-rw-   0        0        0      746 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/cupid/__init__.py
--rw-rw-rw-   0        0        0      272 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/misc/
--rw-rw-rw-   0        0        0     7735 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/misc/stdint.h
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/
--rw-rw-rw-   0        0        0    10889 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/accounts.py
--rw-rw-rw-   0        0        0     7499 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/compat.py
--rw-rw-rw-   0        0        0    16637 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/config.py
--rw-rw-rw-   0        0        0    30359 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/console.py
--rw-rw-rw-   0        0        0    73475 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/core.py
--rw-rw-rw-   0        0        0     2363 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/counters.py
--rw-rw-rw-   0        0        0     6042 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/crc.py
--rw-rw-rw-   0        0        0     8097 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/dag.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/df/
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/df/backends/
--rw-rw-rw-   0        0        0    12085 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/analyzer.py
--rw-rw-rw-   0        0        0     1191 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/context.py
--rw-rw-rw-   0        0        0    29761 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/core.py
--rw-rw-rw-   0        0        0    11910 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/engine.py
--rw-rw-rw-   0        0        0      779 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/errors.py
--rw-rw-rw-   0        0        0    48828 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/formatter.py
--rw-rw-rw-   0        0        0    14930 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/frame.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/df/backends/odpssql/
--rw-rw-rw-   0        0        0    24015 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/odpssql/analyzer.py
--rw-rw-rw-   0        0        0    28343 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/odpssql/codegen.py
--rw-rw-rw-   0        0        0    57464 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/odpssql/compiler.py
--rw-rw-rw-   0        0        0     8944 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/odpssql/context.py
--rw-rw-rw-   0        0        0    24116 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/odpssql/engine.py
--rw-rw-rw-   0        0        0      822 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/odpssql/models.py
--rw-rw-rw-   0        0        0     7224 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/odpssql/rewriter.py
--rw-rw-rw-   0        0        0    11804 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/odpssql/tunnel.py
--rw-rw-rw-   0        0        0     4775 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/odpssql/types.py
--rw-rw-rw-   0        0        0      646 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/odpssql/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/df/backends/optimize/
--rw-rw-rw-   0        0        0     9366 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/optimize/columnpruning.py
--rw-rw-rw-   0        0        0     9396 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/optimize/core.py
--rw-rw-rw-   0        0        0    10129 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/optimize/predicatepushdown.py
--rw-rw-rw-   0        0        0     2494 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/optimize/utils.py
--rw-rw-rw-   0        0        0      673 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/optimize/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/df/backends/pd/
--rw-rw-rw-   0        0        0     3983 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/pd/analyzer.py
--rw-rw-rw-   0        0        0    63303 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/pd/compiler.py
--rw-rw-rw-   0        0        0    13552 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/pd/engine.py
--rw-rw-rw-   0        0        0     4587 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/pd/types.py
--rw-rw-rw-   0        0        0      646 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/pd/__init__.py
--rw-rw-rw-   0        0        0     6657 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/rewriter.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/df/backends/seahawks/
--rw-rw-rw-   0        0        0     3304 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/seahawks/compiler.py
--rw-rw-rw-   0        0        0     1487 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/seahawks/engine.py
--rw-rw-rw-   0        0        0     1286 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/seahawks/ext.py
--rw-rw-rw-   0        0        0     1019 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/seahawks/models.py
--rw-rw-rw-   0        0        0      642 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/seahawks/__init__.py
--rw-rw-rw-   0        0        0     5839 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/selecter.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/df/backends/sqlalchemy/
--rw-rw-rw-   0        0        0     7190 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/sqlalchemy/analyzer.py
--rw-rw-rw-   0        0        0    26354 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/sqlalchemy/compiler.py
--rw-rw-rw-   0        0        0    15020 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/sqlalchemy/engine.py
--rw-rw-rw-   0        0        0     2760 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/sqlalchemy/ext.py
--rw-rw-rw-   0        0        0     2673 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/sqlalchemy/rewriter.py
--rw-rw-rw-   0        0        0     3114 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/sqlalchemy/types.py
--rw-rw-rw-   0        0        0      792 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/sqlalchemy/utils.py
--rw-rw-rw-   0        0        0      642 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/sqlalchemy/__init__.py
--rw-rw-rw-   0        0        0     9948 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/utils.py
--rw-rw-rw-   0        0        0      646 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/backends/__init__.py
--rw-rw-rw-   0        0        0     7241 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/core.py
--rw-rw-rw-   0        0        0     5173 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/delay.py
--rw-rw-rw-   0        0        0      693 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/engines.py
--rw-rw-rw-   0        0        0     5513 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/examples.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/df/expr/
--rw-rw-rw-   0        0        0     9398 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/arithmetic.py
--rw-rw-rw-   0        0        0    61752 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/collections.py
--rw-rw-rw-   0        0        0     9218 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/composites.py
--rw-rw-rw-   0        0        0    18231 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/core.py
--rw-rw-rw-   0        0        0     6715 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/datetimes.py
--rw-rw-rw-   0        0        0     5629 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/dynamic.py
--rw-rw-rw-   0        0        0    21946 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/element.py
--rw-rw-rw-   0        0        0      689 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/errors.py
--rw-rw-rw-   0        0        0    71743 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/expressions.py
--rw-rw-rw-   0        0        0     9855 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/formatter.py
--rw-rw-rw-   0        0        0    19952 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/groupby.py
--rw-rw-rw-   0        0        0     5659 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/math.py
--rw-rw-rw-   0        0        0    42056 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/merge.py
--rw-rw-rw-   0        0        0     6622 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/query.py
--rw-rw-rw-   0        0        0    22431 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/reduction.py
--rw-rw-rw-   0        0        0    21739 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/strings.py
--rw-rw-rw-   0        0        0     7211 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/utils.py
--rw-rw-rw-   0        0        0    19696 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/window.py
--rw-rw-rw-   0        0        0      645 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/expr/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/df/tools/
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/df/tools/lib/
--rw-rw-rw-   0        0        0     5576 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/tools/lib/bloomfilter.py
--rw-rw-rw-   0        0        0     4064 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/tools/lib/hll.py
--rw-rw-rw-   0        0        0      712 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/tools/lib/__init__.py
--rw-rw-rw-   0        0        0     3829 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/tools/libtools.py
--rw-rw-rw-   0        0        0     7358 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/tools/plotting.py
--rw-rw-rw-   0        0        0      694 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/tools/__init__.py
--rw-rw-rw-   0        0        0     9186 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/types.py
--rw-rw-rw-   0        0        0     7377 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/ui.py
--rw-rw-rw-   0        0        0     4910 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/utils.py
--rw-rw-rw-   0        0        0     2094 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/df/__init__.py
--rw-rw-rw-   0        0        0      831 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/distcache.py
--rw-rw-rw-   0        0        0     6723 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/errors.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/examples/
--rw-rw-rw-   0        0        0    21960 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/examples/tables.py
--rw-rw-rw-   0        0        0      640 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/examples/__init__.py
--rw-rw-rw-   0        0        0     6991 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/inter.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ipython/
--rw-rw-rw-   0        0        0     5994 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ipython/completer.py
--rw-rw-rw-   0        0        0    10592 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ipython/magics.py
--rw-rw-rw-   0        0        0      855 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ipython/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/lib/
--rw-rw-rw-   0        0        0    76818 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/cloudpickle.py
--rw-rw-rw-   0        0        0    29895 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/enum.py
--rw-rw-rw-   0        0        0     6012 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/ext_types.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/lib/futures/
--rw-rw-rw-   0        0        0    14877 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/futures/process.py
--rw-rw-rw-   0        0        0     4641 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/futures/thread.py
--rw-rw-rw-   0        0        0    21102 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/futures/_base.py
--rw-rw-rw-   0        0        0      833 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/futures/__init__.py
--rw-rw-rw-   0        0        0    13303 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/importer.py
--rw-rw-rw-   0        0        0     5166 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/lib_utils.py
--rw-rw-rw-   0        0        0    31062 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/six.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/lib/tzlocal/
--rw-rw-rw-   0        0        0     5641 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/tzlocal/unix.py
--rw-rw-rw-   0        0        0     1375 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/tzlocal/utils.py
--rw-rw-rw-   0        0        0     3252 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/tzlocal/win32.py
--rw-rw-rw-   0        0        0    31191 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/tzlocal/windows_tz.py
--rw-rw-rw-   0        0        0      154 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/tzlocal/__init__.py
--rw-rw-rw-   0        0        0     1995 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/xnamedtuple.py
--rw-rw-rw-   0        0        0      646 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/mars_extension/
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/mars_extension/actors/
--rw-rw-rw-   0        0        0     2259 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/actors/prochelper.py
--rw-rw-rw-   0        0        0     1092 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/actors/__init__.py
--rw-rw-rw-   0        0        0    12576 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/core.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/mars_extension/dataframe/
--rw-rw-rw-   0        0        0    15636 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/dataframe/datasource.py
--rw-rw-rw-   0        0        0    12993 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/dataframe/datastore.py
--rw-rw-rw-   0        0        0      924 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/dataframe/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/mars_extension/deploy/
--rw-rw-rw-   0        0        0     9225 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/deploy/client.py
--rw-rw-rw-   0        0        0     3459 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/deploy/notebook.py
--rw-rw-rw-   0        0        0     3118 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/deploy/scheduler.py
--rw-rw-rw-   0        0        0     1225 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/deploy/utils.py
--rw-rw-rw-   0        0        0     2501 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/deploy/web.py
--rw-rw-rw-   0        0        0     2726 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/deploy/worker.py
--rw-rw-rw-   0        0        0      641 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/deploy/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/mars_extension/io/
--rw-rw-rw-   0        0        0     1021 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/io/core.py
--rw-rw-rw-   0        0        0     1383 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/io/local.py
--rw-rw-rw-   0        0        0     3689 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/io/oss.py
--rw-rw-rw-   0        0        0      667 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/io/__init__.py
--rw-rw-rw-   0        0        0    15935 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/oss.py
--rw-rw-rw-   0        0        0     6184 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/run_script.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/mars_extension/tensor/
--rw-rw-rw-   0        0        0     5868 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/tensor/datasource.py
--rw-rw-rw-   0        0        0     6338 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/tensor/datastore.py
--rw-rw-rw-   0        0        0     1054 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/tensor/__init__.py
--rw-rw-rw-   0        0        0     1642 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/mars_extension/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/algolib/
--rw-rw-rw-   0        0        0    14247 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/algolib/base_algo.py
--rw-rw-rw-   0        0        0    20167 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/algolib/loader.py
--rw-rw-rw-   0        0        0    14512 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/algolib/objects.py
--rw-rw-rw-   0        0        0      820 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/algolib/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/classifiers/
--rw-rw-rw-   0        0        0     1599 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/classifiers/_customize.py
--rw-rw-rw-   0        0        0      746 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/classifiers/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/clustering/
--rw-rw-rw-   0        0        0      943 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/clustering/_customize.py
--rw-rw-rw-   0        0        0      746 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/clustering/__init__.py
--rw-rw-rw-   0        0        0     3344 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/cross_validation.py
--rw-rw-rw-   0        0        0    25754 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/engine.py
--rw-rw-rw-   0        0        0     1143 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/enums.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/expr/
--rw-rw-rw-   0        0        0     9685 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/expr/core.py
--rw-rw-rw-   0        0        0     9945 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/expr/exporters.py
--rw-rw-rw-   0        0        0    23452 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/expr/mixin.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/expr/models/
--rw-rw-rw-   0        0        0    14779 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/expr/models/base.py
--rw-rw-rw-   0        0        0    19325 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/expr/models/pmml.py
--rw-rw-rw-   0        0        0      724 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/expr/models/__init__.py
--rw-rw-rw-   0        0        0    10486 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/expr/op.py
--rw-rw-rw-   0        0        0     3565 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/expr/specialized.py
--rw-rw-rw-   0        0        0      831 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/expr/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/feature/
--rw-rw-rw-   0        0        0     2418 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/feature/_customize.py
--rw-rw-rw-   0        0        0      788 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/feature/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/metrics/
--rw-rw-rw-   0        0        0    24088 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/metrics/classification.py
--rw-rw-rw-   0        0        0     1998 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/metrics/clustering.py
--rw-rw-rw-   0        0        0     8118 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/metrics/regression.py
--rw-rw-rw-   0        0        0     3357 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/metrics/scorer.py
--rw-rw-rw-   0        0        0     3253 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/metrics/utils.py
--rw-rw-rw-   0        0        0     7354 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/metrics/_customize.py
--rw-rw-rw-   0        0        0     1022 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/metrics/__init__.py
--rw-rw-rw-   0        0        0     5067 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/models.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/network/
--rw-rw-rw-   0        0        0     2719 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/network/_customize.py
--rw-rw-rw-   0        0        0      830 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/network/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/pipeline/
--rw-rw-rw-   0        0        0    15706 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/pipeline/core.py
--rw-rw-rw-   0        0        0     2767 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/pipeline/steps.py
--rw-rw-rw-   0        0        0      749 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/pipeline/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/preprocess/
--rw-rw-rw-   0        0        0     5275 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/preprocess/_customize.py
--rw-rw-rw-   0        0        0     1070 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/preprocess/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/recommend/
--rw-rw-rw-   0        0        0     2227 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/recommend/_customize.py
--rw-rw-rw-   0        0        0      835 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/recommend/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/regression/
--rw-rw-rw-   0        0        0      792 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/regression/__init__.py
--rw-rw-rw-   0        0        0     6764 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/runners.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/statistics/
--rw-rw-rw-   0        0        0     5002 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/statistics/_customize.py
--rw-rw-rw-   0        0        0      792 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/statistics/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/tensor/
--rw-rw-rw-   0        0        0      788 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/tensor/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/text/
--rw-rw-rw-   0        0        0     2302 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/text/_customize.py
--rw-rw-rw-   0        0        0      824 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/text/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ml/timeseries/
--rw-rw-rw-   0        0        0     1404 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/timeseries/_customize.py
--rw-rw-rw-   0        0        0      836 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/timeseries/__init__.py
--rw-rw-rw-   0        0        0     7390 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/utils.py
--rw-rw-rw-   0        0        0      913 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ml/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/models/
--rw-rw-rw-   0        0        0     4566 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/cache.py
--rw-rw-rw-   0        0        0     6195 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/core.py
--rw-rw-rw-   0        0        0     3597 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/function.py
--rw-rw-rw-   0        0        0     3397 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/functions.py
--rw-rw-rw-   0        0        0    33750 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/instance.py
--rw-rw-rw-   0        0        0     8349 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/instances.py
--rw-rw-rw-   0        0        0     1869 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/job.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/models/ml/
--rw-rw-rw-   0        0        0     3469 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/ml/offlinemodel.py
--rw-rw-rw-   0        0        0     2851 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/ml/offlinemodels.py
--rw-rw-rw-   0        0        0      723 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/ml/__init__.py
--rw-rw-rw-   0        0        0     7179 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/partition.py
--rw-rw-rw-   0        0        0     4842 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/partitions.py
--rw-rw-rw-   0        0        0     8161 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/project.py
--rw-rw-rw-   0        0        0     2527 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/projects.py
--rw-rw-rw-   0        0        0     1085 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/record.py
--rw-rw-rw-   0        0        0    23961 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/resource.py
--rw-rw-rw-   0        0        0     4686 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/resources.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/models/security/
--rw-rw-rw-   0        0        0     2890 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/security/config.py
--rw-rw-rw-   0        0        0     4209 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/security/roles.py
--rw-rw-rw-   0        0        0     3774 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/security/users.py
--rw-rw-rw-   0        0        0      750 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/security/__init__.py
--rw-rw-rw-   0        0        0    10724 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/session.py
--rw-rw-rw-   0        0        0    31366 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/table.py
--rw-rw-rw-   0        0        0     4224 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/tables.py
--rw-rw-rw-   0        0        0     8443 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/tasks.py
--rw-rw-rw-   0        0        0     5848 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/volumes.py
--rw-rw-rw-   0        0        0    16894 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/volume_fs.py
--rw-rw-rw-   0        0        0    13769 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/volume_parted.py
--rw-rw-rw-   0        0        0     3101 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/worker.py
--rw-rw-rw-   0        0        0     1636 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/xflow.py
--rw-rw-rw-   0        0        0     7632 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/xflows.py
--rw-rw-rw-   0        0        0     1355 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/models/__init__.py
--rw-rw-rw-   0        0        0     9368 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/readers.py
--rw-rw-rw-   0        0        0     6566 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/rest.py
--rw-rw-rw-   0        0        0    27234 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/serializers.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/src/
--rw-rw-rw-   0        0        0     9838 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/src/crc32.c
--rw-rw-rw-   0        0        0      788 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/src/crc32c_c.pxd
--rw-rw-rw-   0        0        0     1074 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/src/crc32c_c.pyx
--rw-rw-rw-   0        0        0     1372 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/src/types_c.pxd
--rw-rw-rw-   0        0        0    12404 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/src/types_c.pyx
--rw-rw-rw-   0        0        0      642 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/src/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/static/
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/static/algorithms/
--rw-rw-rw-   0        0        0    38559 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/algorithms/classifier.xml
--rw-rw-rw-   0        0        0     5165 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/algorithms/clustering.xml
--rw-rw-rw-   0        0        0    12368 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/algorithms/feature.xml
--rw-rw-rw-   0        0        0    14356 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/algorithms/metrics.xml
--rw-rw-rw-   0        0        0    41742 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/algorithms/network.xml
--rw-rw-rw-   0        0        0    16822 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/algorithms/preprocess.xml
--rw-rw-rw-   0        0        0     4621 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/algorithms/recommend.xml
--rw-rw-rw-   0        0        0    15269 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/algorithms/regression.xml
--rw-rw-rw-   0        0        0    16361 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/algorithms/statistics.xml
--rw-rw-rw-   0        0        0    38115 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/algorithms/text.xml
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/static/data/
--rw-rw-rw-   0        0        0    83713 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/data/dow_jones.txt
--rw-rw-rw-   0        0        0    76466 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/data/ionosphere.txt
--rw-rw-rw-   0        0        0     4549 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/data/iris.txt
--rw-rw-rw-   0        0        0   141059 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/data/splited_words.txt
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/static/ui/
--rw-rw-rw-   0        0        0     3427 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/Gruntfile.js
--rw-rw-rw-   0        0        0      497 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/package.json
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/static/ui/src/
--rw-rw-rw-   0        0        0      538 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/chosen-sprite.png
--rw-rw-rw-   0        0        0      738 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/chosen-sprite@2x.png
--rw-rw-rw-   0        0        0    11073 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/chosen.css
--rw-rw-rw-   0        0        0    44916 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/chosen.js
--rw-rw-rw-   0        0        0     8269 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/common.js
--rw-rw-rw-   0        0        0    49879 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/df-view.js
--rw-rw-rw-   0        0        0   332760 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/echarts.min.js
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/static/ui/src/fonts/
--rw-rw-rw-   0        0        0     1122 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/fonts/custom-font.css
--rw-rw-rw-   0        0        0     1520 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/fonts/custom-font.eot
--rw-rw-rw-   0        0        0     2665 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/fonts/custom-font.svg
--rw-rw-rw-   0        0        0     1340 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/fonts/custom-font.ttf
--rw-rw-rw-   0        0        0     1416 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/fonts/custom-font.woff
--rw-rw-rw-   0        0        0     9063 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/html-notify.js
--rw-rw-rw-   0        0        0     2031 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/ml-retry.js
--rw-rw-rw-   0        0        0    13294 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/progress.js
--rw-rw-rw-   0        0        0     2502 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/styles.css
--rw-rw-rw-   0        0        0    14015 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/src/westeros.js
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/static/ui/target/
--rw-rw-rw-   0        0        0      538 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/target/chosen-sprite.png
--rw-rw-rw-   0        0        0      738 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/target/chosen-sprite@2x.png
--rw-rw-rw-   0        0        0    10764 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/target/chosen.css
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/static/ui/target/fonts/
--rw-rw-rw-   0        0        0      486 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/target/fonts/custom-font.css
--rw-rw-rw-   0        0        0     1520 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/target/fonts/custom-font.eot
--rw-rw-rw-   0        0        0     2665 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/target/fonts/custom-font.svg
--rw-rw-rw-   0        0        0     1340 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/target/fonts/custom-font.ttf
--rw-rw-rw-   0        0        0     1416 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/target/fonts/custom-font.woff
--rw-rw-rw-   0        0        0   406870 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/target/main.js
--rw-rw-rw-   0        0        0     1416 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/static/ui/target/styles.css
--rw-rw-rw-   0        0        0    14528 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tempobj.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/tunnel/
--rw-rw-rw-   0        0        0     2822 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/base.py
--rw-rw-rw-   0        0        0     2016 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/checksum.py
--rw-rw-rw-   0        0        0     1535 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/checksum_c.pxd
--rw-rw-rw-   0        0        0     3003 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/checksum_c.pyx
--rw-rw-rw-   0        0        0     1451 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/errors.py
--rw-rw-rw-   0        0        0     8087 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/instancetunnel.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/tunnel/io/
--rw-rw-rw-   0        0        0     8520 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/io/reader.py
--rw-rw-rw-   0        0        0     2425 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/io/reader_c.pxd
--rw-rw-rw-   0        0        0    14991 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/io/reader_c.pyx
--rw-rw-rw-   0        0        0    10791 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/io/stream.py
--rw-rw-rw-   0        0        0    17506 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/io/writer.py
--rw-rw-rw-   0        0        0     2308 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/io/writer_c.pxd
--rw-rw-rw-   0        0        0    12444 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/io/writer_c.pyx
--rw-rw-rw-   0        0        0      643 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/io/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/tunnel/pb/
--rw-rw-rw-   0        0        0     4231 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pb/decoder.py
--rw-rw-rw-   0        0        0     1316 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pb/decoder_c.pxd
--rw-rw-rw-   0        0        0     2938 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pb/decoder_c.pyx
--rw-rw-rw-   0        0        0     4896 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pb/encoder.py
--rw-rw-rw-   0        0        0     1231 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pb/encoder_c.pxd
--rw-rw-rw-   0        0        0     2166 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pb/encoder_c.pyx
--rw-rw-rw-   0        0        0      974 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pb/errors.py
--rw-rw-rw-   0        0        0     5169 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pb/input_stream.py
--rw-rw-rw-   0        0        0     4446 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pb/output_stream.py
--rw-rw-rw-   0        0        0     1099 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pb/util_c.pxd
--rw-rw-rw-   0        0        0     5343 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pb/util_c.pyx
--rw-rw-rw-   0        0        0     6820 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pb/wire_format.py
--rw-rw-rw-   0        0        0      623 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pb/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/tunnel/pdio/
--rw-rw-rw-   0        0        0     1766 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pdio/block_decoder_c.pxd
--rw-rw-rw-   0        0        0     6487 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pdio/block_decoder_c.pyx
--rw-rw-rw-   0        0        0     1706 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pdio/block_encoder_c.pxd
--rw-rw-rw-   0        0        0     6711 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pdio/block_encoder_c.pyx
--rw-rw-rw-   0        0        0      756 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pdio/errno.py
--rw-rw-rw-   0        0        0     2149 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pdio/pdreader_c.pxd
--rw-rw-rw-   0        0        0    15022 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pdio/pdreader_c.pyx
--rw-rw-rw-   0        0        0     2417 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pdio/pdwriter.py
--rw-rw-rw-   0        0        0     2487 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pdio/pdwriter_c.pxd
--rw-rw-rw-   0        0        0    17060 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pdio/pdwriter_c.pyx
--rw-rw-rw-   0        0        0      895 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pdio/util_c.pxd
--rw-rw-rw-   0        0        0      845 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/pdio/__init__.py
--rw-rw-rw-   0        0        0    22595 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/tabletunnel.py
--rw-rw-rw-   0        0        0    25078 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/volumetunnel.py
--rw-rw-rw-   0        0        0      783 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/wireconstants.py
--rw-rw-rw-   0        0        0     1154 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/tunnel/__init__.py
--rw-rw-rw-   0        0        0    46989 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/types.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/udf/
--rw-rw-rw-   0        0        0     1607 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/udf/runtime.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/udf/tools/
--rw-rw-rw-   0        0        0     7839 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/udf/tools/runners.py
--rw-rw-rw-   0        0        0     1709 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/udf/tools/utils.py
--rw-rw-rw-   0        0        0      600 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/udf/tools/__init__.py
--rw-rw-rw-   0        0        0      683 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/udf/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/odps/ui/
--rw-rw-rw-   0        0        0     2602 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ui/common.py
--rw-rw-rw-   0        0        0    11031 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ui/progress.py
--rw-rw-rw-   0        0        0      763 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/ui/__init__.py
--rw-rw-rw-   0        0        0    24165 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/utils.py
--rw-rw-rw-   0        0        0      852 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/_version.py
--rw-rw-rw-   0        0        0     1287 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/odps/__init__.py
--rw-rw-rw-   0        0        0     8254 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/pyodps.egg-info/
--rw-rw-rw-   0        0        0        1 2020-08-22 08:25:59.000000 pyodps-0.9.3.2/pyodps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     8254 2020-08-22 08:25:59.000000 pyodps-0.9.3.2/pyodps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      143 2020-08-22 08:25:59.000000 pyodps-0.9.3.2/pyodps.egg-info/requires.txt
--rw-rw-rw-   0        0        0     9967 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/pyodps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2020-08-22 08:25:59.000000 pyodps-0.9.3.2/pyodps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5409 2020-08-22 08:25:15.000000 pyodps-0.9.3.2/README.rst
--rw-rw-rw-   0        0        0       15 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/requirements.txt
-drwxrwxrwx   0        0        0        0 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/scripts/
--rw-rw-rw-   0        0        0     1553 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/scripts/pyou
--rw-rw-rw-   0        0        0       42 2020-08-22 08:26:00.000000 pyodps-0.9.3.2/setup.cfg
--rw-rw-rw-   0        0        0    11932 2020-08-22 08:25:16.000000 pyodps-0.9.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/cupid/
+-rw-rw-rw-   0        0        0     1644 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/config.py
+-rw-rw-rw-   0        0        0     1884 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/errors.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/cupid/io/
+-rw-rw-rw-   0        0        0     1833 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/io/kvstore.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/cupid/io/table/
+-rw-rw-rw-   0        0        0    16260 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/io/table/core.py
+-rw-rw-rw-   0        0        0     4701 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/io/table/pd.py
+-rw-rw-rw-   0        0        0     6941 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/io/table/record.py
+-rw-rw-rw-   0        0        0      827 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/io/table/__init__.py
+-rw-rw-rw-   0        0        0      713 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/io/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/cupid/proto/
+-rw-rw-rw-   0        0        0    91635 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/proto/cupidtaskparam_pb2.py
+-rw-rw-rw-   0        0        0     5164 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/proto/cupid_process_service_pb2.py
+-rw-rw-rw-   0        0        0    28609 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/proto/cupid_subprocess_service_pb2.py
+-rw-rw-rw-   0        0        0    48395 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/proto/cupid_task_service_pb2.py
+-rw-rw-rw-   0        0        0     7228 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/proto/kv_store_service_pb2.py
+-rw-rw-rw-   0        0        0        0 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/proto/__init__.py
+-rw-rw-rw-   0        0        0     8243 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/rpc.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/cupid/runtime/
+-rw-rw-rw-   0        0        0    17571 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/runtime/ctypes_libs.py
+-rw-rw-rw-   0        0        0     3540 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/runtime/runtime.py
+-rw-rw-rw-   0        0        0     2976 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/runtime/runtime_test.py
+-rw-rw-rw-   0        0        0      642 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/runtime/__init__.py
+-rw-rw-rw-   0        0        0     6867 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/session.py
+-rw-rw-rw-   0        0        0     1625 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/utils.py
+-rw-rw-rw-   0        0        0      649 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/_version.py
+-rw-rw-rw-   0        0        0      746 2020-09-06 13:26:52.000000 pyodps-0.9.5/cupid/__init__.py
+-rw-rw-rw-   0        0        0      272 2020-09-06 13:26:52.000000 pyodps-0.9.5/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/misc/
+-rw-rw-rw-   0        0        0     7735 2020-09-06 13:26:52.000000 pyodps-0.9.5/misc/stdint.h
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/
+-rw-rw-rw-   0        0        0    10889 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/accounts.py
+-rw-rw-rw-   0        0        0     7625 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/compat.py
+-rw-rw-rw-   0        0        0    16637 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/config.py
+-rw-rw-rw-   0        0        0    30359 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/console.py
+-rw-rw-rw-   0        0        0    73452 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/core.py
+-rw-rw-rw-   0        0        0     2363 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/counters.py
+-rw-rw-rw-   0        0        0     6042 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/crc.py
+-rw-rw-rw-   0        0        0     8074 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/dag.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/df/
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/df/backends/
+-rw-rw-rw-   0        0        0    12085 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/analyzer.py
+-rw-rw-rw-   0        0        0     1191 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/context.py
+-rw-rw-rw-   0        0        0    29738 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/core.py
+-rw-rw-rw-   0        0        0    11910 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/engine.py
+-rw-rw-rw-   0        0        0      779 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/errors.py
+-rw-rw-rw-   0        0        0    48805 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/formatter.py
+-rw-rw-rw-   0        0        0    14930 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/frame.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/df/backends/odpssql/
+-rw-rw-rw-   0        0        0    24015 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/odpssql/analyzer.py
+-rw-rw-rw-   0        0        0    28343 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/odpssql/codegen.py
+-rw-rw-rw-   0        0        0    57464 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/odpssql/compiler.py
+-rw-rw-rw-   0        0        0     8944 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/odpssql/context.py
+-rw-rw-rw-   0        0        0    24116 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/odpssql/engine.py
+-rw-rw-rw-   0        0        0      822 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/odpssql/models.py
+-rw-rw-rw-   0        0        0     7224 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/odpssql/rewriter.py
+-rw-rw-rw-   0        0        0    11804 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/odpssql/tunnel.py
+-rw-rw-rw-   0        0        0     4775 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/odpssql/types.py
+-rw-rw-rw-   0        0        0      646 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/odpssql/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/df/backends/optimize/
+-rw-rw-rw-   0        0        0     9366 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/optimize/columnpruning.py
+-rw-rw-rw-   0        0        0     9396 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/optimize/core.py
+-rw-rw-rw-   0        0        0    10129 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/optimize/predicatepushdown.py
+-rw-rw-rw-   0        0        0     2494 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/optimize/utils.py
+-rw-rw-rw-   0        0        0      673 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/optimize/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/df/backends/pd/
+-rw-rw-rw-   0        0        0     3983 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/pd/analyzer.py
+-rw-rw-rw-   0        0        0    63303 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/pd/compiler.py
+-rw-rw-rw-   0        0        0    13552 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/pd/engine.py
+-rw-rw-rw-   0        0        0     4587 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/pd/types.py
+-rw-rw-rw-   0        0        0      646 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/pd/__init__.py
+-rw-rw-rw-   0        0        0     6657 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/rewriter.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/df/backends/seahawks/
+-rw-rw-rw-   0        0        0     3304 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/seahawks/compiler.py
+-rw-rw-rw-   0        0        0     1487 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/seahawks/engine.py
+-rw-rw-rw-   0        0        0     1286 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/seahawks/ext.py
+-rw-rw-rw-   0        0        0     1019 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/seahawks/models.py
+-rw-rw-rw-   0        0        0      642 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/seahawks/__init__.py
+-rw-rw-rw-   0        0        0     5839 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/selecter.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/df/backends/sqlalchemy/
+-rw-rw-rw-   0        0        0     7190 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/sqlalchemy/analyzer.py
+-rw-rw-rw-   0        0        0    26354 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/sqlalchemy/compiler.py
+-rw-rw-rw-   0        0        0    15020 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/sqlalchemy/engine.py
+-rw-rw-rw-   0        0        0     2760 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/sqlalchemy/ext.py
+-rw-rw-rw-   0        0        0     2673 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/sqlalchemy/rewriter.py
+-rw-rw-rw-   0        0        0     3114 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/sqlalchemy/types.py
+-rw-rw-rw-   0        0        0      792 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/sqlalchemy/utils.py
+-rw-rw-rw-   0        0        0      642 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/sqlalchemy/__init__.py
+-rw-rw-rw-   0        0        0     9948 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/utils.py
+-rw-rw-rw-   0        0        0      646 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/backends/__init__.py
+-rw-rw-rw-   0        0        0     7241 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/core.py
+-rw-rw-rw-   0        0        0     5173 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/delay.py
+-rw-rw-rw-   0        0        0      693 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/engines.py
+-rw-rw-rw-   0        0        0     5513 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/examples.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/df/expr/
+-rw-rw-rw-   0        0        0     9398 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/arithmetic.py
+-rw-rw-rw-   0        0        0    61752 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/collections.py
+-rw-rw-rw-   0        0        0     9218 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/composites.py
+-rw-rw-rw-   0        0        0    18231 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/core.py
+-rw-rw-rw-   0        0        0     6715 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/datetimes.py
+-rw-rw-rw-   0        0        0     5629 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/dynamic.py
+-rw-rw-rw-   0        0        0    21946 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/element.py
+-rw-rw-rw-   0        0        0      689 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/errors.py
+-rw-rw-rw-   0        0        0    71743 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/expressions.py
+-rw-rw-rw-   0        0        0     9855 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/formatter.py
+-rw-rw-rw-   0        0        0    19952 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/groupby.py
+-rw-rw-rw-   0        0        0     5659 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/math.py
+-rw-rw-rw-   0        0        0    42056 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/merge.py
+-rw-rw-rw-   0        0        0     6622 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/query.py
+-rw-rw-rw-   0        0        0    22431 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/reduction.py
+-rw-rw-rw-   0        0        0    21739 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/strings.py
+-rw-rw-rw-   0        0        0     7211 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/utils.py
+-rw-rw-rw-   0        0        0    19696 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/window.py
+-rw-rw-rw-   0        0        0      645 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/expr/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/df/tools/
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/df/tools/lib/
+-rw-rw-rw-   0        0        0     5576 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/tools/lib/bloomfilter.py
+-rw-rw-rw-   0        0        0     4064 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/tools/lib/hll.py
+-rw-rw-rw-   0        0        0      712 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/tools/lib/__init__.py
+-rw-rw-rw-   0        0        0     3829 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/tools/libtools.py
+-rw-rw-rw-   0        0        0     7358 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/tools/plotting.py
+-rw-rw-rw-   0        0        0      694 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/tools/__init__.py
+-rw-rw-rw-   0        0        0     9186 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/types.py
+-rw-rw-rw-   0        0        0     7377 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/ui.py
+-rw-rw-rw-   0        0        0     4910 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/utils.py
+-rw-rw-rw-   0        0        0     2094 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/df/__init__.py
+-rw-rw-rw-   0        0        0      831 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/distcache.py
+-rw-rw-rw-   0        0        0     6723 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/errors.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/examples/
+-rw-rw-rw-   0        0        0    21960 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/examples/tables.py
+-rw-rw-rw-   0        0        0      640 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/examples/__init__.py
+-rw-rw-rw-   0        0        0     6991 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/inter.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ipython/
+-rw-rw-rw-   0        0        0     5994 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ipython/completer.py
+-rw-rw-rw-   0        0        0    10592 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ipython/magics.py
+-rw-rw-rw-   0        0        0      855 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ipython/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/lib/
+-rw-rw-rw-   0        0        0    76818 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/cloudpickle.py
+-rw-rw-rw-   0        0        0    29895 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/enum.py
+-rw-rw-rw-   0        0        0     6012 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/ext_types.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/lib/futures/
+-rw-rw-rw-   0        0        0    14877 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/futures/process.py
+-rw-rw-rw-   0        0        0     4641 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/futures/thread.py
+-rw-rw-rw-   0        0        0    21102 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/futures/_base.py
+-rw-rw-rw-   0        0        0      833 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/futures/__init__.py
+-rw-rw-rw-   0        0        0    13303 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/importer.py
+-rw-rw-rw-   0        0        0     5166 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/lib_utils.py
+-rw-rw-rw-   0        0        0    31062 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/six.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/lib/tzlocal/
+-rw-rw-rw-   0        0        0     5641 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/tzlocal/unix.py
+-rw-rw-rw-   0        0        0     1375 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/tzlocal/utils.py
+-rw-rw-rw-   0        0        0     3252 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/tzlocal/win32.py
+-rw-rw-rw-   0        0        0    31191 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/tzlocal/windows_tz.py
+-rw-rw-rw-   0        0        0      154 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/tzlocal/__init__.py
+-rw-rw-rw-   0        0        0     1995 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/xnamedtuple.py
+-rw-rw-rw-   0        0        0      646 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/mars_extension/
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/mars_extension/actors/
+-rw-rw-rw-   0        0        0     3145 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/actors/session.py
+-rw-rw-rw-   0        0        0      643 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/actors/__init__.py
+-rw-rw-rw-   0        0        0    15684 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/core.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/mars_extension/dataframe/
+-rw-rw-rw-   0        0        0    17581 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/dataframe/datasource.py
+-rw-rw-rw-   0        0        0    12988 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/dataframe/datastore.py
+-rw-rw-rw-   0        0        0      924 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/dataframe/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/mars_extension/deploy/
+-rw-rw-rw-   0        0        0    10598 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/deploy/app.py
+-rw-rw-rw-   0        0        0     9621 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/deploy/client.py
+-rw-rw-rw-   0        0        0     5139 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/deploy/core.py
+-rw-rw-rw-   0        0        0     3499 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/deploy/notebook.py
+-rw-rw-rw-   0        0        0     1339 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/deploy/scheduler.py
+-rw-rw-rw-   0        0        0     1225 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/deploy/utils.py
+-rw-rw-rw-   0        0        0     1873 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/deploy/web.py
+-rw-rw-rw-   0        0        0      953 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/deploy/worker.py
+-rw-rw-rw-   0        0        0      642 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/deploy/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/mars_extension/io/
+-rw-rw-rw-   0        0        0     1021 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/io/core.py
+-rw-rw-rw-   0        0        0     1383 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/io/local.py
+-rw-rw-rw-   0        0        0     3689 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/io/oss.py
+-rw-rw-rw-   0        0        0      667 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/io/__init__.py
+-rw-rw-rw-   0        0        0    15935 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/oss.py
+-rw-rw-rw-   0        0        0     6179 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/run_script.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/mars_extension/tensor/
+-rw-rw-rw-   0        0        0     5868 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/tensor/datasource.py
+-rw-rw-rw-   0        0        0     6338 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/tensor/datastore.py
+-rw-rw-rw-   0        0        0     1054 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/tensor/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/mars_extension/web/
+-rw-rw-rw-   0        0        0     1116 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/web/apihandlers.py
+-rw-rw-rw-   0        0        0      707 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/web/__init__.py
+-rw-rw-rw-   0        0        0     1570 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/mars_extension/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/algolib/
+-rw-rw-rw-   0        0        0    14247 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/algolib/base_algo.py
+-rw-rw-rw-   0        0        0    20144 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/algolib/loader.py
+-rw-rw-rw-   0        0        0    14512 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/algolib/objects.py
+-rw-rw-rw-   0        0        0      820 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/algolib/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/classifiers/
+-rw-rw-rw-   0        0        0     1599 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/classifiers/_customize.py
+-rw-rw-rw-   0        0        0      746 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/classifiers/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/clustering/
+-rw-rw-rw-   0        0        0      943 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/clustering/_customize.py
+-rw-rw-rw-   0        0        0      746 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/clustering/__init__.py
+-rw-rw-rw-   0        0        0     3344 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/cross_validation.py
+-rw-rw-rw-   0        0        0    25754 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/engine.py
+-rw-rw-rw-   0        0        0     1143 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/enums.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/expr/
+-rw-rw-rw-   0        0        0     9685 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/expr/core.py
+-rw-rw-rw-   0        0        0     9945 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/expr/exporters.py
+-rw-rw-rw-   0        0        0    23452 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/expr/mixin.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/expr/models/
+-rw-rw-rw-   0        0        0    14779 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/expr/models/base.py
+-rw-rw-rw-   0        0        0    19325 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/expr/models/pmml.py
+-rw-rw-rw-   0        0        0      724 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/expr/models/__init__.py
+-rw-rw-rw-   0        0        0    10486 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/expr/op.py
+-rw-rw-rw-   0        0        0     3565 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/expr/specialized.py
+-rw-rw-rw-   0        0        0      831 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/expr/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/feature/
+-rw-rw-rw-   0        0        0     2418 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/feature/_customize.py
+-rw-rw-rw-   0        0        0      788 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/feature/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/metrics/
+-rw-rw-rw-   0        0        0    24088 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/metrics/classification.py
+-rw-rw-rw-   0        0        0     1998 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/metrics/clustering.py
+-rw-rw-rw-   0        0        0     8118 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/metrics/regression.py
+-rw-rw-rw-   0        0        0     3357 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/metrics/scorer.py
+-rw-rw-rw-   0        0        0     3253 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/metrics/utils.py
+-rw-rw-rw-   0        0        0     7354 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/metrics/_customize.py
+-rw-rw-rw-   0        0        0     1022 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/metrics/__init__.py
+-rw-rw-rw-   0        0        0     5067 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/models.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/network/
+-rw-rw-rw-   0        0        0     2719 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/network/_customize.py
+-rw-rw-rw-   0        0        0      830 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/network/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/pipeline/
+-rw-rw-rw-   0        0        0    15707 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/pipeline/core.py
+-rw-rw-rw-   0        0        0     2767 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/pipeline/steps.py
+-rw-rw-rw-   0        0        0      749 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/pipeline/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/preprocess/
+-rw-rw-rw-   0        0        0     5252 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/preprocess/_customize.py
+-rw-rw-rw-   0        0        0     1070 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/preprocess/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/recommend/
+-rw-rw-rw-   0        0        0     2227 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/recommend/_customize.py
+-rw-rw-rw-   0        0        0      835 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/recommend/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/regression/
+-rw-rw-rw-   0        0        0      792 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/regression/__init__.py
+-rw-rw-rw-   0        0        0     6764 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/runners.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/statistics/
+-rw-rw-rw-   0        0        0     5002 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/statistics/_customize.py
+-rw-rw-rw-   0        0        0      792 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/statistics/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/tensor/
+-rw-rw-rw-   0        0        0      788 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/tensor/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/text/
+-rw-rw-rw-   0        0        0     2302 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/text/_customize.py
+-rw-rw-rw-   0        0        0      824 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/text/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ml/timeseries/
+-rw-rw-rw-   0        0        0     1404 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/timeseries/_customize.py
+-rw-rw-rw-   0        0        0      836 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/timeseries/__init__.py
+-rw-rw-rw-   0        0        0     7390 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/utils.py
+-rw-rw-rw-   0        0        0      913 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ml/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/models/
+-rw-rw-rw-   0        0        0     4566 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/cache.py
+-rw-rw-rw-   0        0        0     6195 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/core.py
+-rw-rw-rw-   0        0        0     3597 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/function.py
+-rw-rw-rw-   0        0        0     3397 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/functions.py
+-rw-rw-rw-   0        0        0    33750 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/instance.py
+-rw-rw-rw-   0        0        0     8349 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/instances.py
+-rw-rw-rw-   0        0        0     1869 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/job.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/models/ml/
+-rw-rw-rw-   0        0        0     3469 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/ml/offlinemodel.py
+-rw-rw-rw-   0        0        0     2851 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/ml/offlinemodels.py
+-rw-rw-rw-   0        0        0      723 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/ml/__init__.py
+-rw-rw-rw-   0        0        0     7179 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/partition.py
+-rw-rw-rw-   0        0        0     4842 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/partitions.py
+-rw-rw-rw-   0        0        0     8161 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/project.py
+-rw-rw-rw-   0        0        0     2527 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/projects.py
+-rw-rw-rw-   0        0        0     1085 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/record.py
+-rw-rw-rw-   0        0        0    23961 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/resource.py
+-rw-rw-rw-   0        0        0     4686 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/resources.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/models/security/
+-rw-rw-rw-   0        0        0     2890 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/security/config.py
+-rw-rw-rw-   0        0        0     4209 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/security/roles.py
+-rw-rw-rw-   0        0        0     3774 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/security/users.py
+-rw-rw-rw-   0        0        0      750 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/security/__init__.py
+-rw-rw-rw-   0        0        0    10817 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/session.py
+-rw-rw-rw-   0        0        0    31463 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/table.py
+-rw-rw-rw-   0        0        0     4224 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/tables.py
+-rw-rw-rw-   0        0        0     8443 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/tasks.py
+-rw-rw-rw-   0        0        0     5848 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/volumes.py
+-rw-rw-rw-   0        0        0    16894 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/volume_fs.py
+-rw-rw-rw-   0        0        0    13769 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/volume_parted.py
+-rw-rw-rw-   0        0        0     3101 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/worker.py
+-rw-rw-rw-   0        0        0     1636 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/xflow.py
+-rw-rw-rw-   0        0        0     7632 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/xflows.py
+-rw-rw-rw-   0        0        0     1355 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/models/__init__.py
+-rw-rw-rw-   0        0        0     9368 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/readers.py
+-rw-rw-rw-   0        0        0     6566 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/rest.py
+-rw-rw-rw-   0        0        0    27234 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/serializers.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/src/
+-rw-rw-rw-   0        0        0     9838 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/src/crc32.c
+-rw-rw-rw-   0        0        0      788 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/src/crc32c_c.pxd
+-rw-rw-rw-   0        0        0     1074 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/src/crc32c_c.pyx
+-rw-rw-rw-   0        0        0     1372 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/src/types_c.pxd
+-rw-rw-rw-   0        0        0    12404 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/src/types_c.pyx
+-rw-rw-rw-   0        0        0      642 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/src/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/static/
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/static/algorithms/
+-rw-rw-rw-   0        0        0    38559 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/algorithms/classifier.xml
+-rw-rw-rw-   0        0        0     5165 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/algorithms/clustering.xml
+-rw-rw-rw-   0        0        0    12368 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/algorithms/feature.xml
+-rw-rw-rw-   0        0        0    14356 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/algorithms/metrics.xml
+-rw-rw-rw-   0        0        0    41742 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/algorithms/network.xml
+-rw-rw-rw-   0        0        0    16822 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/algorithms/preprocess.xml
+-rw-rw-rw-   0        0        0     4621 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/algorithms/recommend.xml
+-rw-rw-rw-   0        0        0    15269 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/algorithms/regression.xml
+-rw-rw-rw-   0        0        0    16361 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/algorithms/statistics.xml
+-rw-rw-rw-   0        0        0    38115 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/algorithms/text.xml
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/static/data/
+-rw-rw-rw-   0        0        0    83713 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/data/dow_jones.txt
+-rw-rw-rw-   0        0        0    76466 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/data/ionosphere.txt
+-rw-rw-rw-   0        0        0     4549 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/data/iris.txt
+-rw-rw-rw-   0        0        0   141059 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/data/splited_words.txt
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/static/ui/
+-rw-rw-rw-   0        0        0     3427 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/Gruntfile.js
+-rw-rw-rw-   0        0        0      497 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/package.json
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/static/ui/src/
+-rw-rw-rw-   0        0        0      538 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/chosen-sprite.png
+-rw-rw-rw-   0        0        0      738 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/chosen-sprite@2x.png
+-rw-rw-rw-   0        0        0    11073 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/chosen.css
+-rw-rw-rw-   0        0        0    44916 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/chosen.js
+-rw-rw-rw-   0        0        0     8269 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/common.js
+-rw-rw-rw-   0        0        0    49879 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/df-view.js
+-rw-rw-rw-   0        0        0   332760 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/echarts.min.js
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/static/ui/src/fonts/
+-rw-rw-rw-   0        0        0     1122 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/fonts/custom-font.css
+-rw-rw-rw-   0        0        0     1520 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/fonts/custom-font.eot
+-rw-rw-rw-   0        0        0     2665 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/fonts/custom-font.svg
+-rw-rw-rw-   0        0        0     1340 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/fonts/custom-font.ttf
+-rw-rw-rw-   0        0        0     1416 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/fonts/custom-font.woff
+-rw-rw-rw-   0        0        0     9063 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/html-notify.js
+-rw-rw-rw-   0        0        0     2031 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/ml-retry.js
+-rw-rw-rw-   0        0        0    13294 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/progress.js
+-rw-rw-rw-   0        0        0     2502 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/styles.css
+-rw-rw-rw-   0        0        0    14015 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/src/westeros.js
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/static/ui/target/
+-rw-rw-rw-   0        0        0      538 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/target/chosen-sprite.png
+-rw-rw-rw-   0        0        0      738 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/target/chosen-sprite@2x.png
+-rw-rw-rw-   0        0        0    10764 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/target/chosen.css
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/static/ui/target/fonts/
+-rw-rw-rw-   0        0        0      486 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/target/fonts/custom-font.css
+-rw-rw-rw-   0        0        0     1520 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/target/fonts/custom-font.eot
+-rw-rw-rw-   0        0        0     2665 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/target/fonts/custom-font.svg
+-rw-rw-rw-   0        0        0     1340 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/target/fonts/custom-font.ttf
+-rw-rw-rw-   0        0        0     1416 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/target/fonts/custom-font.woff
+-rw-rw-rw-   0        0        0   406870 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/target/main.js
+-rw-rw-rw-   0        0        0     1416 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/static/ui/target/styles.css
+-rw-rw-rw-   0        0        0    14528 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tempobj.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/tunnel/
+-rw-rw-rw-   0        0        0     2822 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/base.py
+-rw-rw-rw-   0        0        0     2016 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/checksum.py
+-rw-rw-rw-   0        0        0     1535 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/checksum_c.pxd
+-rw-rw-rw-   0        0        0     3003 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/checksum_c.pyx
+-rw-rw-rw-   0        0        0     1451 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/errors.py
+-rw-rw-rw-   0        0        0     9106 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/instancetunnel.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/tunnel/io/
+-rw-rw-rw-   0        0        0     8520 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/io/reader.py
+-rw-rw-rw-   0        0        0     2425 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/io/reader_c.pxd
+-rw-rw-rw-   0        0        0    14991 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/io/reader_c.pyx
+-rw-rw-rw-   0        0        0    10791 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/io/stream.py
+-rw-rw-rw-   0        0        0    17506 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/io/writer.py
+-rw-rw-rw-   0        0        0     2308 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/io/writer_c.pxd
+-rw-rw-rw-   0        0        0    12444 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/io/writer_c.pyx
+-rw-rw-rw-   0        0        0      643 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/io/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/tunnel/pb/
+-rw-rw-rw-   0        0        0     4231 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pb/decoder.py
+-rw-rw-rw-   0        0        0     1316 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pb/decoder_c.pxd
+-rw-rw-rw-   0        0        0     2938 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pb/decoder_c.pyx
+-rw-rw-rw-   0        0        0     4896 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pb/encoder.py
+-rw-rw-rw-   0        0        0     1231 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pb/encoder_c.pxd
+-rw-rw-rw-   0        0        0     2166 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pb/encoder_c.pyx
+-rw-rw-rw-   0        0        0      974 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pb/errors.py
+-rw-rw-rw-   0        0        0     5169 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pb/input_stream.py
+-rw-rw-rw-   0        0        0     4446 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pb/output_stream.py
+-rw-rw-rw-   0        0        0     1099 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pb/util_c.pxd
+-rw-rw-rw-   0        0        0     5343 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pb/util_c.pyx
+-rw-rw-rw-   0        0        0     6820 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pb/wire_format.py
+-rw-rw-rw-   0        0        0      623 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pb/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/tunnel/pdio/
+-rw-rw-rw-   0        0        0     1766 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pdio/block_decoder_c.pxd
+-rw-rw-rw-   0        0        0     6487 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pdio/block_decoder_c.pyx
+-rw-rw-rw-   0        0        0     1706 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pdio/block_encoder_c.pxd
+-rw-rw-rw-   0        0        0     6711 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pdio/block_encoder_c.pyx
+-rw-rw-rw-   0        0        0      756 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pdio/errno.py
+-rw-rw-rw-   0        0        0     2149 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pdio/pdreader_c.pxd
+-rw-rw-rw-   0        0        0    15022 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pdio/pdreader_c.pyx
+-rw-rw-rw-   0        0        0     2417 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pdio/pdwriter.py
+-rw-rw-rw-   0        0        0     2487 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pdio/pdwriter_c.pxd
+-rw-rw-rw-   0        0        0    17060 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pdio/pdwriter_c.pyx
+-rw-rw-rw-   0        0        0      895 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pdio/util_c.pxd
+-rw-rw-rw-   0        0        0      845 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/pdio/__init__.py
+-rw-rw-rw-   0        0        0    22595 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/tabletunnel.py
+-rw-rw-rw-   0        0        0    25078 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/volumetunnel.py
+-rw-rw-rw-   0        0        0      783 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/wireconstants.py
+-rw-rw-rw-   0        0        0     1154 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/tunnel/__init__.py
+-rw-rw-rw-   0        0        0    46989 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/types.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/udf/
+-rw-rw-rw-   0        0        0     1607 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/udf/runtime.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/udf/tools/
+-rw-rw-rw-   0        0        0     7839 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/udf/tools/runners.py
+-rw-rw-rw-   0        0        0     1709 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/udf/tools/utils.py
+-rw-rw-rw-   0        0        0      600 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/udf/tools/__init__.py
+-rw-rw-rw-   0        0        0      683 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/udf/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/odps/ui/
+-rw-rw-rw-   0        0        0     2602 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ui/common.py
+-rw-rw-rw-   0        0        0    11031 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ui/progress.py
+-rw-rw-rw-   0        0        0      763 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/ui/__init__.py
+-rw-rw-rw-   0        0        0    24165 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/utils.py
+-rw-rw-rw-   0        0        0      849 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/_version.py
+-rw-rw-rw-   0        0        0     1287 2020-09-06 13:26:52.000000 pyodps-0.9.5/odps/__init__.py
+-rw-rw-rw-   0        0        0     8252 2020-09-06 13:27:26.000000 pyodps-0.9.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/pyodps.egg-info/
+-rw-rw-rw-   0        0        0        1 2020-09-06 13:27:26.000000 pyodps-0.9.5/pyodps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     8252 2020-09-06 13:27:26.000000 pyodps-0.9.5/pyodps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2020-09-06 13:27:26.000000 pyodps-0.9.5/pyodps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0    10108 2020-09-06 13:27:26.000000 pyodps-0.9.5/pyodps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       11 2020-09-06 13:27:26.000000 pyodps-0.9.5/pyodps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5409 2020-09-06 13:26:52.000000 pyodps-0.9.5/README.rst
+-rw-rw-rw-   0        0        0       15 2020-09-06 13:26:52.000000 pyodps-0.9.5/requirements.txt
+drwxrwxrwx   0        0        0        0 2020-09-06 13:27:26.000000 pyodps-0.9.5/scripts/
+-rw-rw-rw-   0        0        0     1553 2020-09-06 13:26:52.000000 pyodps-0.9.5/scripts/pyou
+-rw-rw-rw-   0        0        0       42 2020-09-06 13:27:26.000000 pyodps-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0    11932 2020-09-06 13:26:52.000000 pyodps-0.9.5/setup.py
```

### Comparing `pyodps-0.9.3.2/cupid/config.py` & `pyodps-0.9.5/cupid/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 options.register_option('cupid.running_engine_type', None)
 options.register_option('cupid.job_duration_hours', 25920)
 options.register_option('cupid.channel_init_timeout_seconds', 120)
 options.register_option('cupid.kube.master_mode', 'cupid')
 options.register_option('cupid.runtime.endpoint', 'http://service.cn.maxcompute.aliyun-inc.com/api')
 
 # mars app config
-options.register_option('cupid.mars_image', 'mars-app:0.9.3rc')
+options.register_option('cupid.image_prefix', None)
+options.register_option('cupid.image_version', '0.9.4rc3')
```

### Comparing `pyodps-0.9.3.2/cupid/errors.py` & `pyodps-0.9.5/cupid/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,23 +28,23 @@
 class CupidUserError(CupidError):
     pass
 
 
 class CupidCppError(CupidError):
     cpp_error_type = None
 
-    def __new__(cls, err_type, err_msg):
+    def __new__(cls, err_type=None, err_msg=None):
         if cls is not CupidCppError:
             return CupidError.__new__(cls)
         if err_type in _cpp_errors:
             return CupidError.__new__(_cpp_errors[err_type])
         else:
             return CupidError.__new__(cls)
 
-    def __init__(self, err_type, err_msg):
+    def __init__(self, err_type=None, err_msg=None):
         self._err_type = err_type
         self._err_msg = err_msg
 
     def __str__(self):
         return '%s: %s' % (self._err_type, self._err_msg)
```

### Comparing `pyodps-0.9.3.2/cupid/io/kvstore.py` & `pyodps-0.9.5/cupid/io/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/cupid/io/table/core.py` & `pyodps-0.9.5/cupid/io/table/core.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/cupid/io/table/pd.py` & `pyodps-0.9.5/cupid/io/table/pd.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/cupid/io/table/record.py` & `pyodps-0.9.5/cupid/io/table/record.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/cupid/io/table/__init__.py` & `pyodps-0.9.5/cupid/io/table/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/cupid/io/__init__.py` & `pyodps-0.9.5/cupid/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/cupid/proto/cupidtaskparam_pb2.py` & `pyodps-0.9.5/cupid/proto/cupidtaskparam_pb2.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/cupid/proto/cupid_process_service_pb2.py` & `pyodps-0.9.5/cupid/proto/cupid_process_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/cupid/proto/cupid_subprocess_service_pb2.py` & `pyodps-0.9.5/cupid/proto/cupid_subprocess_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/cupid/proto/cupid_task_service_pb2.py` & `pyodps-0.9.5/cupid/proto/cupid_task_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/cupid/proto/kv_store_service_pb2.py` & `pyodps-0.9.5/cupid/proto/kv_store_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/cupid/rpc.py` & `pyodps-0.9.5/cupid/rpc.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/cupid/runtime/ctypes_libs.py` & `pyodps-0.9.5/cupid/runtime/ctypes_libs.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/cupid/runtime/runtime.py` & `pyodps-0.9.5/cupid/runtime/runtime.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,34 +10,36 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import logging
+import os
 
 from ..utils import get_environ
 from ..proto import cupid_process_service_pb2 as process_pb
 from ..rpc import CupidRpcController, SandboxRpcChannel
 
 logger = logging.getLogger(__name__)
-context_holder = [None]
+_pid_to_context = dict()
 
 
 def context():
     try:
         from .ctypes_libs import Subprocess_Container_Init, Subprocess_StartFDReceiver
     except ImportError:
         return
 
-    if not context_holder[0]:
+    pid = os.getpid()
+    if pid not in _pid_to_context:
         Subprocess_Container_Init()
         Subprocess_StartFDReceiver()
-        context_holder[0] = RuntimeContext()
-    return context_holder[0]
+        _pid_to_context[pid] = RuntimeContext()
+    return _pid_to_context[pid]
 
 
 class RuntimeContext(object):
     def __init__(self):
         from .ctypes_libs import ChannelConf, ChannelSlaveClient
         # init channels
         server_read_pipe_num = int(get_environ('serverReadPipeNum', 2))
@@ -53,14 +55,18 @@
         logger.info("serverReadPipeNum: %d, serverWritePipeNum: %d, clientReadPipeNum: %d, "
                     "clientWritePipeNum: %d, cpuCores: %d" %
                     (server_read_pipe_num, server_write_pipe_num, client_read_pipe_num,
                      client_write_pipe_num, cpu_cores))
         self._channel_client = ChannelSlaveClient(client_write_pipe_num, client_read_pipe_num, 'slave_client')
         self._channel_client.start()
 
+    @staticmethod
+    def is_context_ready():
+        return os.getpid() in _pid_to_context
+
     @property
     def channel_client(self):
         return self._channel_client
 
     def register_application(self, app_name, address):
         return self.channel_client.sync_call('report_app_address', json.dumps(
             dict(name=app_name, address=address)
```

### Comparing `pyodps-0.9.3.2/cupid/runtime/runtime_test.py` & `pyodps-0.9.5/cupid/runtime/runtime_test.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/cupid/runtime/__init__.py` & `pyodps-0.9.5/cupid/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/cupid/session.py` & `pyodps-0.9.5/cupid/session.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,64 +23,14 @@
 from .utils import get_environ
 
 logger = logging.getLogger(__name__)
 
 _CUPID_CONF_PREFIXES = 'odps cupid'.split()
 
 
-def _build_mars_config(app_config):
-    options.cupid.application_type = 'mars'
-
-    mars_config = dict()
-
-    resources = app_config['resources']
-    module_path = app_config['module_path']
-    resources_config = ','.join(resources)
-    module_path_config = ','.join(module_path)
-    mars_image = app_config.get('mars_image', None)
-
-    mars_config['odps.cupid.resources'] = resources_config
-    notebook = app_config.get('notebook', None)
-    cmd = '/opt/conda/bin/python /srv/server.py ' \
-          '--scheduler-num {} ' \
-          '--scheduler-cpu {} ' \
-          '--scheduler-mem {} ' \
-          '--worker-num {} ' \
-          '--worker-cpu {} ' \
-          '--worker-mem {} ' \
-          '--disk-num {} ' \
-          '--cache-mem {} ' \
-          '--module-path {} '.format(
-        app_config['scheduler_num'],
-        app_config['scheduler_cpu'],
-        app_config['scheduler_mem'],
-        app_config['worker_num'],
-        app_config['worker_cpu'],
-        app_config['worker_mem'],
-        app_config['disk_num'],
-        app_config['cache_mem'],
-        module_path_config
-    )
-    if mars_image:
-        cmd = cmd + '--mars-image {} '.format(mars_image)
-    if notebook:
-        cmd = cmd + '--with-nootbook '
-    mars_config['odps.cupid.kube.appmaster.cmd'] = cmd
-    mars_config['odps.cupid.kube.appmaster.image'] = app_config.get('mars_app_image', None) or \
-                                                     options.cupid.mars_image
-    return mars_config
-
-
-def _build_app_config(app_name, app_config):
-    if app_name == 'mars':
-        return _build_mars_config(app_config)
-    else:
-        return dict()
-
-
 class CupidSession(object):
     def __init__(self, odps=None, project=None):
         from .runtime import context
         from odps import ODPS
 
         self._context = context()
 
@@ -91,16 +41,14 @@
         self.project = project if project is not None else self.odps.project
 
         self.lookup_name = get_environ('META_LOOKUP_NAME', '')
         self.running = False
         self.save_id = None
         self.job_running_event = threading.Event()
 
-        self._kube_app_name = None
-        self._kube_app_config = None
         self._kube_url = None
 
     def check_running(self, timeout=None):
         timeout = timeout or options.cupid.wait_am_start_time
         if not self.running:
             self.job_running_event.wait(timeout)
         return self.running
@@ -149,47 +97,47 @@
         return channel.wait_cupid_instance(inst)
 
     def get_proxied_url(self, instance, app_name, expired_in_hours=None):
         expired_in_hours = expired_in_hours or 30 * 24
         return 'http://%s.%s' % (self.get_proxy_token(instance, app_name, expired_in_hours),
                                  options.cupid.proxy_endpoint)
 
-    def start_kubernetes(self, async_=False, priority=None, running_cluster=None, **kw):
+    def start_kubernetes(self, async_=False, priority=None, running_cluster=None,
+                         proxy_endpoint=None, major_task_version=None,
+                         app_command=None, app_image=None, resources=None, **kw):
         priority = priority or options.priority
         if priority is None and options.get_priority is not None:
             priority = options.get_priority(self.odps)
         menginetype = options.cupid.running_engine_type
 
-        self._kube_app_name = kw.get('app_name', None)
-        self._kube_app_config = kw.get('app_config', None)
-
-        proxy_endpoint = self._kube_app_config.pop('proxy_endpoint', None)
         if proxy_endpoint is not None:
             options.cupid.proxy_endpoint = proxy_endpoint
-
-        major_task_version = self._kube_app_config.pop('major_task_version', None)
         if major_task_version is not None:
             options.cupid.major_task_version = major_task_version
 
-        async_ = kw.get('async', async_)
-        runtime_endpoint = kw.get('runtime_endpoint', None)
+        async_ = kw.pop('async', async_)
+        runtime_endpoint = kw.pop('runtime_endpoint', None)
         task_operator = task_param_pb.CupidTaskOperator(moperator='startam', menginetype=menginetype)
-        task_name = kw.get('task_name')
+        task_name = kw.pop('task_name', None)
+
+        if len(kw) > 0:
+            raise ValueError('Got unexpected arguments: {}'.format(list(kw.keys())[0]))
 
         kub_conf = {
             'odps.cupid.kube.master.mode': options.cupid.kube.master_mode,
             'odps.cupid.master.type': options.cupid.master_type,
             'odps.cupid.engine.running.type': menginetype,
             'odps.cupid.job.capability.duration.hours': options.cupid.job_duration_hours,
             'odps.cupid.channel.init.timeout.seconds': options.cupid.channel_init_timeout_seconds,
             'odps.moye.runtime.type': options.cupid.application_type,
-            'odps.runtime.end.point': runtime_endpoint or options.cupid.runtime.endpoint
+            'odps.runtime.end.point': runtime_endpoint or options.cupid.runtime.endpoint,
+            'odps.cupid.resources': ','.join(resources or []),
+            'odps.cupid.kube.appmaster.cmd': app_command,
+            'odps.cupid.kube.appmaster.image': app_image
         }
-        app_conf = _build_app_config(self._kube_app_name, self._kube_app_config)
-        kub_conf.update(app_conf)
         if running_cluster:
             kub_conf['odps.cupid.task.running.cluster'] = running_cluster
         task_param = task_param_pb.CupidTaskParam(
             jobconf=self.job_conf(conf=kub_conf),
             mcupidtaskoperator=task_operator,
         )
         channel = CupidTaskServiceRpcChannel(self)
```

### Comparing `pyodps-0.9.3.2/cupid/_version.py` & `pyodps-0.9.5/cupid/_version.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/cupid/__init__.py` & `pyodps-0.9.5/cupid/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/misc/stdint.h` & `pyodps-0.9.5/misc/stdint.h`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/accounts.py` & `pyodps-0.9.5/odps/accounts.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/compat.py` & `pyodps-0.9.5/odps/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,18 @@
     import xml.etree.cElementTree as ElementTree
 except ImportError:
     import xml.etree.ElementTree as ElementTree
 try:
     ElementTreeParseError = getattr(ElementTree, 'ParseError')
 except AttributeError:
     ElementTreeParseError = getattr(ElementTree, 'XMLParserError')
+try:
+    from collections.abc import Iterable
+except ImportError:
+    from collections import Iterable
 from unicodedata import east_asian_width
 
 from .lib import six
 
 PY26 = six.PY2 and sys.version_info[1] == 6
 PY27 = six.PY2 and sys.version_info[1] == 7
 LESS_PY26 = sys.version_info[:2] < (2, 6)
@@ -266,8 +270,9 @@
 
     utc = FixedOffset(0, 'UTC')
 
 
 __all__ = ['sys', 'builtins', 'logging.config', 'unittest', 'OrderedDict', 'dictconfig', 'suppress',
            'reduce', 'reload_module', 'Queue', 'Empty', 'ElementTree', 'ElementTreeParseError',
            'urlretrieve', 'pickle', 'urlencode', 'urlparse', 'unquote', 'quote', 'quote_plus', 'parse_qsl',
-           'Enum', 'ConfigParser', 'decimal', 'Decimal', 'DECIMAL_TYPES', 'FixedOffset', 'utc', 'Monthdelta']
+           'Enum', 'ConfigParser', 'decimal', 'Decimal', 'DECIMAL_TYPES', 'FixedOffset', 'utc', 'Monthdelta',
+           'Iterable']
```

### Comparing `pyodps-0.9.3.2/odps/config.py` & `pyodps-0.9.5/odps/config.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/console.py` & `pyodps-0.9.5/odps/console.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/core.py` & `pyodps-0.9.5/odps/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,21 @@
 
 import os
 import json
 import re
 import time
 import random
 import warnings
-from collections import Iterable
 
 from .rest import RestClient
 from .config import options
 from .errors import NoSuchObject
 from .tempobj import clean_stored_objects
 from .utils import split_quoted
-from .compat import six
+from .compat import six, Iterable
 from . import models, accounts, errors, utils
 
 
 DEFAULT_ENDPOINT = 'http://service.odps.aliyun.com/api'
 LOG_VIEW_HOST_DEFAULT = 'http://logview.odps.aliyun.com'
 
 DROP_TABLE_REGEX = re.compile(r'^\s*drop\s+table\s*(|if\s+exists)\s+(?P<table_name>[^\s;]+)', re.I)
```

### Comparing `pyodps-0.9.3.2/odps/counters.py` & `pyodps-0.9.5/odps/counters.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/crc.py` & `pyodps-0.9.5/odps/crc.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/dag.py` & `pyodps-0.9.5/odps/dag.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import itertools
-from collections import Iterable
 from copy import deepcopy
 
-from .compat import Queue, six
+from .compat import Queue, six, Iterable
 
 
 class DAGValidationError(Exception):
     pass
 
 
 class DAG(object):
```

### Comparing `pyodps-0.9.3.2/odps/df/backends/analyzer.py` & `pyodps-0.9.5/odps/df/backends/analyzer.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/context.py` & `pyodps-0.9.5/odps/df/backends/context.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/core.py` & `pyodps-0.9.5/odps/df/backends/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,24 +12,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import absolute_import
 
-from collections import Iterable
 import itertools
 import time
 import types
 import os
 import sys
 import threading
 from operator import itemgetter
 
-from ...compat import six, Enum
+from ...compat import six, Enum, Iterable
 from ...models import Resource
 from ...config import options
 from ...dag import DAG
 from ...utils import init_progress_ui
 from ...ui.progress import create_instance_group
 from ...compat import futures
 from ...types import PartitionSpec
```

### Comparing `pyodps-0.9.3.2/odps/df/backends/engine.py` & `pyodps-0.9.5/odps/df/backends/engine.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/errors.py` & `pyodps-0.9.5/odps/df/backends/errors.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/formatter.py` & `pyodps-0.9.5/odps/df/backends/formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,20 +12,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from distutils.version import LooseVersion
 import itertools
-from collections import Iterable
 import cgi
 
 from ...config import options
 from ... import compat
-from ...compat import u, izip
+from ...compat import u, izip, Iterable
 from ...console import get_terminal_size
 from ...utils import to_text, to_str, indent, require_package
 from ...models import Table
 from ..types import *
 from ..expr.expressions import CollectionExpr, Scalar
 from ..utils import is_source_collection, traverse_until_source
```

### Comparing `pyodps-0.9.3.2/odps/df/backends/frame.py` & `pyodps-0.9.5/odps/df/backends/frame.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/odpssql/analyzer.py` & `pyodps-0.9.5/odps/df/backends/odpssql/analyzer.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/odpssql/codegen.py` & `pyodps-0.9.5/odps/df/backends/odpssql/codegen.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/odpssql/compiler.py` & `pyodps-0.9.5/odps/df/backends/odpssql/compiler.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/odpssql/context.py` & `pyodps-0.9.5/odps/df/backends/odpssql/context.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/odpssql/engine.py` & `pyodps-0.9.5/odps/df/backends/odpssql/engine.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/odpssql/models.py` & `pyodps-0.9.5/odps/df/backends/odpssql/models.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/odpssql/rewriter.py` & `pyodps-0.9.5/odps/df/backends/odpssql/rewriter.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/odpssql/tunnel.py` & `pyodps-0.9.5/odps/df/backends/odpssql/tunnel.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/odpssql/types.py` & `pyodps-0.9.5/odps/df/backends/odpssql/types.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/odpssql/__init__.py` & `pyodps-0.9.5/odps/df/backends/odpssql/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/optimize/columnpruning.py` & `pyodps-0.9.5/odps/df/backends/optimize/columnpruning.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/optimize/core.py` & `pyodps-0.9.5/odps/df/backends/optimize/core.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/optimize/predicatepushdown.py` & `pyodps-0.9.5/odps/df/backends/optimize/predicatepushdown.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/optimize/utils.py` & `pyodps-0.9.5/odps/df/backends/optimize/utils.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/optimize/__init__.py` & `pyodps-0.9.5/odps/df/backends/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/pd/analyzer.py` & `pyodps-0.9.5/odps/df/backends/pd/analyzer.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/pd/compiler.py` & `pyodps-0.9.5/odps/df/backends/pd/compiler.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/pd/engine.py` & `pyodps-0.9.5/odps/df/backends/pd/engine.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/pd/types.py` & `pyodps-0.9.5/odps/df/backends/pd/types.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/pd/__init__.py` & `pyodps-0.9.5/odps/df/backends/pd/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/rewriter.py` & `pyodps-0.9.5/odps/df/backends/rewriter.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/seahawks/compiler.py` & `pyodps-0.9.5/odps/df/backends/seahawks/compiler.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/seahawks/engine.py` & `pyodps-0.9.5/odps/df/backends/seahawks/engine.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/seahawks/ext.py` & `pyodps-0.9.5/odps/df/backends/seahawks/ext.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/seahawks/models.py` & `pyodps-0.9.5/odps/df/backends/seahawks/models.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/seahawks/__init__.py` & `pyodps-0.9.5/odps/df/backends/seahawks/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/selecter.py` & `pyodps-0.9.5/odps/df/backends/selecter.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/sqlalchemy/analyzer.py` & `pyodps-0.9.5/odps/df/backends/sqlalchemy/analyzer.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/sqlalchemy/compiler.py` & `pyodps-0.9.5/odps/df/backends/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/sqlalchemy/engine.py` & `pyodps-0.9.5/odps/df/backends/sqlalchemy/engine.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/sqlalchemy/ext.py` & `pyodps-0.9.5/odps/df/backends/sqlalchemy/ext.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/sqlalchemy/rewriter.py` & `pyodps-0.9.5/odps/df/backends/sqlalchemy/rewriter.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/sqlalchemy/types.py` & `pyodps-0.9.5/odps/df/backends/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/sqlalchemy/utils.py` & `pyodps-0.9.5/odps/df/backends/sqlalchemy/utils.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/sqlalchemy/__init__.py` & `pyodps-0.9.5/odps/df/backends/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/utils.py` & `pyodps-0.9.5/odps/df/backends/utils.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/backends/__init__.py` & `pyodps-0.9.5/odps/df/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/core.py` & `pyodps-0.9.5/odps/df/core.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/delay.py` & `pyodps-0.9.5/odps/df/delay.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/engines.py` & `pyodps-0.9.5/odps/df/engines.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/examples.py` & `pyodps-0.9.5/odps/df/examples.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/arithmetic.py` & `pyodps-0.9.5/odps/df/expr/arithmetic.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/collections.py` & `pyodps-0.9.5/odps/df/expr/collections.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/composites.py` & `pyodps-0.9.5/odps/df/expr/composites.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/core.py` & `pyodps-0.9.5/odps/df/expr/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import absolute_import
 
 import itertools
 import weakref
-from collections import deque, defaultdict, Iterable
+from collections import deque, defaultdict
 
 from ... import compat
-from ...compat import six
+from ...compat import six, Iterable
 from ...dag import DAG, Queue
 from . import utils
 
 
 class NodeMetaclass(type):
     def __new__(mcs, name, bases, kv):
         mixin_slots = []
```

### Comparing `pyodps-0.9.3.2/odps/df/expr/datetimes.py` & `pyodps-0.9.5/odps/df/expr/datetimes.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/dynamic.py` & `pyodps-0.9.5/odps/df/expr/dynamic.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/element.py` & `pyodps-0.9.5/odps/df/expr/element.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/errors.py` & `pyodps-0.9.5/odps/df/expr/errors.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/expressions.py` & `pyodps-0.9.5/odps/df/expr/expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import absolute_import
 import inspect
 import operator
-from collections import defaultdict, Iterable
+from collections import defaultdict
 import functools
 import sys
 
 from .core import Node, NodeMetaclass
 from .errors import ExpressionError
 from .utils import get_attrs, is_called_by_inspector, highest_precedence_data_type, new_id, \
     is_changed, get_proxied_expr
 from .. import types
-from ...compat import reduce, isvalidattr, dir2, OrderedDict, lkeys, six, futures
+from ...compat import reduce, isvalidattr, dir2, OrderedDict, lkeys, six, futures, Iterable
 from ...config import options
 from ...errors import NoSuchObject, DependencyNotInstalledError
 from ...utils import TEMP_TABLE_PREFIX, to_binary, deprecated, survey
 from ...models import Schema
 
 
 class ReprWrapper(object):
```

### Comparing `pyodps-0.9.3.2/odps/df/expr/formatter.py` & `pyodps-0.9.5/odps/df/expr/formatter.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/groupby.py` & `pyodps-0.9.5/odps/df/expr/groupby.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/math.py` & `pyodps-0.9.5/odps/df/expr/math.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/merge.py` & `pyodps-0.9.5/odps/df/expr/merge.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/query.py` & `pyodps-0.9.5/odps/df/expr/query.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/reduction.py` & `pyodps-0.9.5/odps/df/expr/reduction.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/strings.py` & `pyodps-0.9.5/odps/df/expr/strings.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/utils.py` & `pyodps-0.9.5/odps/df/expr/utils.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/window.py` & `pyodps-0.9.5/odps/df/expr/window.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/expr/__init__.py` & `pyodps-0.9.5/odps/df/expr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/tools/lib/bloomfilter.py` & `pyodps-0.9.5/odps/df/tools/lib/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/tools/lib/hll.py` & `pyodps-0.9.5/odps/df/tools/lib/hll.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/tools/lib/__init__.py` & `pyodps-0.9.5/odps/df/tools/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/tools/libtools.py` & `pyodps-0.9.5/odps/df/tools/libtools.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/tools/plotting.py` & `pyodps-0.9.5/odps/df/tools/plotting.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/tools/__init__.py` & `pyodps-0.9.5/odps/df/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/types.py` & `pyodps-0.9.5/odps/df/types.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/ui.py` & `pyodps-0.9.5/odps/df/ui.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/utils.py` & `pyodps-0.9.5/odps/df/utils.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/df/__init__.py` & `pyodps-0.9.5/odps/df/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/distcache.py` & `pyodps-0.9.5/odps/distcache.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/errors.py` & `pyodps-0.9.5/odps/errors.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/examples/tables.py` & `pyodps-0.9.5/odps/examples/tables.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/examples/__init__.py` & `pyodps-0.9.5/odps/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/inter.py` & `pyodps-0.9.5/odps/inter.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ipython/completer.py` & `pyodps-0.9.5/odps/ipython/completer.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ipython/magics.py` & `pyodps-0.9.5/odps/ipython/magics.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ipython/__init__.py` & `pyodps-0.9.5/odps/ipython/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/lib/cloudpickle.py` & `pyodps-0.9.5/odps/lib/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/lib/enum.py` & `pyodps-0.9.5/odps/lib/enum.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/lib/ext_types.py` & `pyodps-0.9.5/odps/lib/ext_types.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/lib/futures/process.py` & `pyodps-0.9.5/odps/lib/futures/process.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/lib/futures/thread.py` & `pyodps-0.9.5/odps/lib/futures/thread.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/lib/futures/_base.py` & `pyodps-0.9.5/odps/lib/futures/_base.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/lib/futures/__init__.py` & `pyodps-0.9.5/odps/lib/futures/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/lib/importer.py` & `pyodps-0.9.5/odps/lib/importer.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/lib/lib_utils.py` & `pyodps-0.9.5/odps/lib/lib_utils.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/lib/six.py` & `pyodps-0.9.5/odps/lib/six.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/lib/tzlocal/unix.py` & `pyodps-0.9.5/odps/lib/tzlocal/unix.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/lib/tzlocal/utils.py` & `pyodps-0.9.5/odps/lib/tzlocal/utils.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/lib/tzlocal/win32.py` & `pyodps-0.9.5/odps/lib/tzlocal/win32.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/lib/tzlocal/windows_tz.py` & `pyodps-0.9.5/odps/lib/tzlocal/windows_tz.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/lib/xnamedtuple.py` & `pyodps-0.9.5/odps/lib/xnamedtuple.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/lib/__init__.py` & `pyodps-0.9.5/odps/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/mars_extension/actors/__init__.py` & `pyodps-0.9.5/odps/mars_extension/deploy/scheduler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,41 @@
-#!/usr/bin/env python
+# !/usr/bin/env python
 # -*- coding: utf-8 -*-
-# Copyright 1999-2018 Alibaba Group Holding Ltd.
+# Copyright 1999-2017 Alibaba Group Holding Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import json
+import logging
+import os
 
-def _install():
-    try:
-        from .prochelper import WorkerProcessHelperActor, CupidWorkerProcessHelperActor, \
-            CupidStatusActor, StatusActor
+from mars.deploy.kubernetes.scheduler import K8SSchedulerApplication
+
+from .core import CupidServiceMixin
+
+logger = logging.getLogger(__name__)
+
+
+class CupidSchedulerApplication(CupidServiceMixin, K8SSchedulerApplication):
+    def __init__(self, *args, **kwargs):
         from mars.actors import register_actor_implementation
+        from mars.scheduler import SessionManagerActor
+        from odps.mars_extension.actors import CupidSessionManagerActor
+
+        register_actor_implementation(SessionManagerActor, CupidSessionManagerActor)
+        super().__init__(*args, **kwargs)
 
-        register_actor_implementation(WorkerProcessHelperActor, CupidWorkerProcessHelperActor)
-        register_actor_implementation(StatusActor, CupidStatusActor)
-    except ImportError:
-        pass
 
+main = CupidSchedulerApplication()
 
-_install()
-del _install
+if __name__ == '__main__':
+    main()
```

### Comparing `pyodps-0.9.3.2/odps/mars_extension/core.py` & `pyodps-0.9.5/odps/mars_extension/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from ..df import types as pd_types
 from ..df.backends.odpssql.types import df_type_to_odps_type
 from ..models import Schema
 from ..types import PartitionSpec
 from ..utils import to_binary, write_log
 
 
-logger = logging.getLogger('mars.worker')
+logger = logging.getLogger(__name__)
 
 
 def _check_internal(endpoint):
     from . import INTERNAL_PATTERN
 
     if INTERNAL_PATTERN and re.search(INTERNAL_PATTERN, endpoint) is not None:
         try:
@@ -69,41 +69,50 @@
         if task_name is not None:
             if not return_task_name:
                 yield instance
             else:
                 yield task_name, instance
 
 
-def create_mars_cluster(odps, worker_num=1, worker_cpu=8, worker_mem=32, cache_mem=None, disk_num=1,
-                        min_worker_num=None, resources=None, module_path=None, scheduler_num=1,
-                        notebook=None, instance_id=None, name='default', if_exists='reuse',
-                        project=None, **kw):
+def create_mars_cluster(odps, worker_num=1, worker_cpu=8, worker_mem=32, cache_mem=None,
+                        min_worker_num=None, disk_num=1, disk_size=100,
+                        scheduler_num=1, scheduler_cpu=None, scheduler_mem=None,
+                        web_num=1, web_cpu=None, web_mem=None, with_notebook=False,
+                        notebook_cpu=None, notebook_mem=None, timeout=None,
+                        extra_modules=None, resources=None, instance_id=None, name='default',
+                        if_exists='reuse', project=None, **kw):
     """
+    Create a Mars cluster and a Mars session as default session,
+    then all tasks will be submitted to cluster.
+
     :param worker_num: mars cluster worker's number
     :param worker_cpu: number of cpu cores on each mars worker
     :param worker_mem: memory size on each mars worker
     :param cache_mem: cache memory size on each mars worker
     :param disk_num: number of mounted disk
     :param min_worker_num: return if cluster worker's number reach to min_worker
     :param resources: resources name
-    :param module_path: user defined module path
+    :param extra_modules: user defined module path
     :param scheduler_num: the number of schedulers, default is 0
-    :param notebook: whether launch jupyter notebook, defaullt is False
+    :param with_notebook: whether launch jupyter notebook, defaullt is False
     :param instance_id: existing mars cluster's instance id
     :param name: cluster name, 'default' will be default name
     :param if_exists: 'reuse', 'raise' or 'ignore',
                       if 'reuse', will reuse the first created cluster with the same name,
                       if not created, create a new one;
                       if 'raise', will fail if cluster with same name created already;
                       if 'ignore', will always create a new cluster
     :param project: project name
     :return: class: `MarsClient`
     """
     from .deploy.client import MarsCupidClient
 
+    if kw.get('proxy_endpoint', None) is not None:
+        cupid_options.cupid.proxy_endpoint = kw['proxy_endpoint']
+
     if if_exists not in ('reuse', 'raise', 'ignore'):
         raise ValueError('`if_exists` should be "reuse", "raise", or "ignore"')
 
     task_name = 'MARS_TASK_{}'.format(hashlib.md5(to_binary(name)).hexdigest())
 
     _check_internal(odps.endpoint)
     if instance_id is not None:
@@ -128,31 +137,77 @@
                     raise ValueError('Cluster("{}") exists'.format(name))
 
         if client is None:
             # not create before, just create a new one
             client = MarsCupidClient(odps, project=project)
     else:
         client = MarsCupidClient(odps, project=project)
-    return client.submit(worker_num, worker_cpu, worker_mem, disk_num=disk_num, min_worker_num=min_worker_num,
-                         cache_mem=cache_mem, resources=resources, module_path=module_path, create_session=True,
-                         scheduler_num=scheduler_num, notebook=notebook, task_name=task_name, **kw)
+
+    worker_mem = int(worker_mem * 1024 ** 3)
+    cache_mem = int(cache_mem * 1024 ** 3) if cache_mem else None
+    disk_size = int(disk_size * 1024 ** 3)
+    scheduler_mem = int(scheduler_mem * 1024 ** 3) if scheduler_mem else None
+    web_mem = int(web_mem * 1024 ** 3) if web_mem else None
+    notebook_mem = int(notebook_mem * 1024 ** 3) if web_mem else None
+
+    kw = dict(worker_num=worker_num, worker_cpu=worker_cpu, worker_mem=worker_mem,
+              worker_cache_mem=cache_mem, min_worker_num=min_worker_num,
+              worker_disk_num=disk_num, worker_disk_size=disk_size,
+              scheduler_num=scheduler_num, scheduler_cpu=scheduler_cpu,
+              scheduler_mem=scheduler_mem, web_num=web_num, web_cpu=web_cpu,
+              web_mem=web_mem, with_notebook=with_notebook, notebook_cpu=notebook_cpu,
+              notebook_mem=notebook_mem, timeout=timeout, extra_modules=extra_modules,
+              resources=resources, task_name=task_name, **kw)
+    kw = dict((k, v) for k, v in kw.items() if v is not None)
+    return client.submit(**kw)
 
 
 def to_mars_dataframe(odps, table_name, shape=None, partition=None, chunk_bytes=None,
                       sparse=False, columns=None, add_offset=False, calc_nrows=True,
                       use_arrow_dtype=False, cupid_internal_endpoint=None):
+    """
+    Read table to Mars DataFrame.
+
+    :param table_name: table name
+    :param shape: table shape. A tuple like (1000, 3) which means table count is 1000 and schema length is 3.
+    :param partition: partition spec.
+    :param chunk_bytes: Bytes to read for each chunk. Default value is '16M'.
+    :param sparse: if read as sparse DataFrame.
+    :param columns: selected columns.
+    :param add_offset: if standardize the DataFrame's index to RangeIndex. False as default.
+    :param calc_nrows: if calculate nrows if shape is not specified.
+    :param use_arrow_dtype: read to arrow dtype. Reduce memory in some saces.
+    :return: Mars DataFrame.
+    """
     from cupid import context
     from .dataframe import read_odps_table
     from ..utils import init_progress_ui
 
     odps_params = dict(
         project=odps.project, endpoint=cupid_internal_endpoint or cupid_options.cupid.runtime.endpoint)
 
     data_src = odps.get_table(table_name)
 
+    odps_schema = data_src.schema
+    if len(odps_schema.partitions) != 0:
+        if partition is None:
+            raise TypeError('Partition should be specified.')
+
+    for col in columns or []:
+        if col not in odps_schema.names:
+            raise TypeError("Specific column {} doesn't exist in table".format(col))
+
+    # persist view table to a temp table
+    if data_src.is_virtual_view:
+        temp_table_name = table_name + '_temp_mars_table_' + str(uuid.uuid4()).replace('-', '_')
+        odps.create_table(temp_table_name, schema=data_src.schema, stored_as='aliorc', lifecycle=1)
+        data_src.to_df().persist(temp_table_name)
+        table_name = temp_table_name
+        data_src = odps.get_table(table_name)
+
     # get dataframe's shape
     if shape is None:
         if calc_nrows and context() is None:
             # obtain count
             if partition is None:
                 odps_df = data_src.to_df()
             else:
@@ -167,14 +222,26 @@
                            chunk_bytes=chunk_bytes, sparse=sparse, columns=columns,
                            odps_params=odps_params, add_offset=add_offset,
                            use_arrow_dtype=use_arrow_dtype)
 
 
 def persist_mars_dataframe(odps, df, table_name, overwrite=False, partition=None, write_batch_size=None,
                            unknown_as_string=True, as_type=None, cupid_internal_endpoint=None):
+    """
+    Write Mars DataFrame to table.
+
+    :param df: Mars DataFrame.
+    :param table_name: table to write.
+    :param overwrite: if overwrite the data. False as default.
+    :param partition: partition spec.
+    :param write_batch_size: batch size of records to write. 1024 as default.
+    :param unknown_as_string: set the columns to string type if it's type is Object.
+    :param as_type: specify column dtypes. {'a': 'string'} will set column `a` as string type.
+    :return: None
+    """
     from .dataframe import write_odps_table
 
     dtypes = df.dtypes
     odps_types = []
     names = []
     for name, t in zip(dtypes.keys(), list(dtypes.values)):
         names.append(name)
@@ -215,16 +282,16 @@
     run_script(script, mode=mode, n_workers=n_workers,
                command_argv=command_argv, odps_params=odps_params, **kw)
 
 
 def run_mars_job(odps, func, args=(), kwargs=None, retry_when_fail=False, n_output=None, **kw):
     from mars.remote import spawn
 
-    if 'notebook' not in kw:
-        kw['notebook'] = False
+    if 'with_notebook' not in kw:
+        kw['with_notebook'] = False
     task_name = kw.get('name', None)
     if task_name is None:
         kw['name'] = str(uuid.uuid4())
         kw['if_exists'] = 'ignore'
 
     cupid_internal_endpoint = kw.pop('cupid_internal_endpoint', None)
     client = odps.create_mars_cluster(**kw)
```

### Comparing `pyodps-0.9.3.2/odps/mars_extension/dataframe/datasource.py` & `pyodps-0.9.5/odps/mars_extension/dataframe/datasource.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 from mars.serialize import StringField, Int64Field, SeriesField, DictField, BoolField, ListField
 from mars.dataframe import ArrowStringDtype
 from mars.dataframe.operands import DataFrameOperandMixin, DataFrameOperand
 from mars.dataframe.utils import parse_index, standardize_range_index, arrow_table_to_pandas_dataframe
 from mars.optimizes.runtime.dataframe import DataSourceHeadRule
 
 from ...df.backends.odpssql.types import odps_type_to_df_type
+from ...errors import ODPSError
 from ...utils import to_str
 
-logger = logging.getLogger('mars.worker')
+logger = logging.getLogger(__name__)
 
 READ_CHUNK_LIMIT = 16 * 1024 ** 2
 MAX_CHUNK_SIZE = 512 * 1024 ** 2
 
 ORC_COMPRESSION_RATIO = 5
 STRING_FIELD_OVERHEAD = 50
 
@@ -120,34 +121,53 @@
     @classmethod
     def tile(cls, op):
         import numpy as np
         import pandas as pd
         from odps import ODPS
         from odps.accounts import BearerTokenAccount
         from cupid import CupidSession, context
+        from mars.context import get_context
 
         cupid_ctx = context()
         if cupid_ctx is None:
             raise SystemError('No Mars cluster found, please create via `o.create_mars_cluster`.')
+
         bearer_token = cupid_ctx.get_bearer_token()
         account = BearerTokenAccount(bearer_token)
         project = os.environ.get('ODPS_PROJECT_NAME', None)
         odps_params = op.odps_params.copy()
         if project:
             odps_params['project'] = project
         o = ODPS(None, None, account=account, **odps_params)
         cupid_session = CupidSession(o)
 
+        mars_context = get_context()
+
         df = op.outputs[0]
         split_size = df.extra_params.chunk_bytes or READ_CHUNK_LIMIT
 
         data_src = o.get_table(op.table_name)
         if op.partition is not None:
             data_src = data_src.get_partition(op.partition)
 
+        try:
+            data_store_size = data_src.size
+        except ODPSError:
+            # fail to get data size, just ignore
+            pass
+        else:
+            if data_store_size < split_size and mars_context is not None:
+                # get worker counts
+                worker_count = max(len(mars_context.get_worker_addresses()), 1)
+                # data is too small, split as many as number of cores
+                split_size = data_store_size // worker_count
+                # at least 1M
+                split_size = max(split_size, 1 * 1024 ** 2)
+                logger.debug('Input data size is too small, split_size is {}'.format(split_size))
+
         logger.debug('Start creating download session of table {} from cupid.'.format(op.table_name))
         while True:
             try:
                 download_session = cupid_session.create_download_session(
                     data_src, split_size=split_size, columns=op.columns)
                 break
             except CupidError:
@@ -169,32 +189,42 @@
 
         logger.warning('Estimated chunk rows: %r', est_chunk_rows)
 
         out_chunks = []
         # Ignore add_offset at this time.
         op._add_offset = False
 
-        for idx, split in enumerate(download_session.splits):
-            chunk_op = DataFrameReadTableSplit(cupid_handle=to_str(split.handle),
-                                               split_index=split.split_index,
-                                               split_file_start=split.split_file_start,
-                                               split_file_end=split.split_file_end,
-                                               schema_file_start=split.schema_file_start,
-                                               schema_file_end=split.schema_file_end,
-                                               add_offset=op.add_offset, dtypes=op.dtypes,
-                                               sparse=op.sparse, split_size=split_size,
-                                               use_arrow_dtype=op.use_arrow_dtype,
-                                               estimate_rows=est_chunk_rows[idx])
-            # the chunk shape is unknown
+        if len(download_session.splits) == 0:
+            logger.debug('Table {} has no data'.format(op.table_name))
+            chunk_op = DataFrameReadTableSplit()
             index_value = parse_index(pd.RangeIndex(0))
             columns_value = parse_index(df.dtypes.index, store_data=True)
             out_chunk = chunk_op.new_chunk(None, shape=(np.nan, df.shape[1]), dtypes=op.dtypes,
                                            index_value=index_value, columns_value=columns_value,
-                                           index=(idx, 0))
-            out_chunks.append(out_chunk)
+                                           index=(0, 0))
+            out_chunks = [out_chunk]
+        else:
+            for idx, split in enumerate(download_session.splits):
+                chunk_op = DataFrameReadTableSplit(cupid_handle=to_str(split.handle),
+                                                   split_index=split.split_index,
+                                                   split_file_start=split.split_file_start,
+                                                   split_file_end=split.split_file_end,
+                                                   schema_file_start=split.schema_file_start,
+                                                   schema_file_end=split.schema_file_end,
+                                                   add_offset=op.add_offset, dtypes=op.dtypes,
+                                                   sparse=op.sparse, split_size=split_size,
+                                                   use_arrow_dtype=op.use_arrow_dtype,
+                                                   estimate_rows=est_chunk_rows[idx])
+                # the chunk shape is unknown
+                index_value = parse_index(pd.RangeIndex(0))
+                columns_value = parse_index(df.dtypes.index, store_data=True)
+                out_chunk = chunk_op.new_chunk(None, shape=(np.nan, df.shape[1]), dtypes=op.dtypes,
+                                               index_value=index_value, columns_value=columns_value,
+                                               index=(idx, 0))
+                out_chunks.append(out_chunk)
 
         if op.add_offset:
             out_chunks = standardize_range_index(out_chunks)
 
         new_op = op.copy()
         nsplits = ((np.nan,) * len(out_chunks), (df.shape[1],))
         return new_op.new_dataframes(None, shape=df.shape, dtypes=op.dtypes,
@@ -293,14 +323,18 @@
             try:
                 return np.issubdtype(dtype, np.object_) \
                        or np.issubdtype(dtype, np.unicode_) \
                        or np.issubdtype(dtype, np.bytes_)
             except TypeError:  # pragma: no cover
                 return False
 
+        if op.split_size is None:
+            ctx[op.outputs[0].key] = (0, 0)
+            return
+
         arrow_size = ORC_COMPRESSION_RATIO * op.split_size
         n_strings = len([dt for dt in op.dtypes if is_object_dtype(dt)])
         if op.estimate_rows or op.nrows:
             rows = op.nrows if op.nrows is not None else op.estimate_rows
             pd_size = arrow_size + n_strings * rows * STRING_FIELD_OVERHEAD
             logger.debug('Estimate pandas memory cost: %r', pd_size)
         else:
@@ -309,14 +343,21 @@
         ctx[op.outputs[0].key] = (pd_size, pd_size + arrow_size)
 
     @classmethod
     def execute(cls, ctx, op):
         import pyarrow as pa
         from cupid.io.table import TableSplit
 
+        if op.cupid_handle is None:
+            empty_df = pd.DataFrame()
+            for name, dtype in op.outputs[0].dtypes.items():
+                empty_df[name] = pd.Series(dtype=dtype)
+            ctx[op.outputs[0].key] = empty_df
+            return
+
         tsp = TableSplit(
             _handle=op.cupid_handle,
             _split_index=op.split_index,
             _split_file_start=op.split_file_start,
             _split_file_end=op.split_file_end,
             _schema_file_start=op.schema_file_start,
             _schema_file_end=op.schema_file_end,
@@ -379,14 +420,19 @@
     if chunk_bytes is not None:
         chunk_bytes = int(parse_readable_size(chunk_bytes)[0])
     table_name = '%s.%s' % (table.project.name, table.name)
     table_columns = table.schema.names
     table_types = table.schema.types
     df_types = [df_type_to_np_type(odps_type_to_df_type(type), use_arrow_dtype=use_arrow_dtype)
                 for type in table_types]
+
+    if columns is not None:
+        df_types = [df_types[table_columns.index(col)] for col in columns]
+        table_columns = columns
+
     dtypes = pd.Series(df_types, index=table_columns)
 
     op = DataFrameReadTable(odps_params=odps_params, table_name=table_name, partition_spec=partition,
                             dtypes=dtypes, sparse=sparse, add_offset=add_offset, columns=columns,
                             use_arrow_dtype=use_arrow_dtype)
     return op(shape, chunk_bytes=chunk_bytes)
```

### Comparing `pyodps-0.9.3.2/odps/mars_extension/dataframe/datastore.py` & `pyodps-0.9.5/odps/mars_extension/dataframe/datastore.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from mars.dataframe.operands import DataFrameOperandMixin, DataFrameOperand
 from mars.dataframe.utils import parse_index
 from mars.serialize import StringField, SeriesField, BoolField, DictField, Int64Field
 
 from ...utils import to_str
 
-logger = logging.getLogger('mars.worker')
+logger = logging.getLogger(__name__)
 
 try:
     from mars.core import OutputType
     _output_type_kw = dict(_output_types=[OutputType.dataframe])
 except ImportError:
     from mars.dataframe.operands import ObjectType
     _output_type_kw = dict(_object_type=ObjectType.dataframe)
```

### Comparing `pyodps-0.9.3.2/odps/mars_extension/dataframe/__init__.py` & `pyodps-0.9.5/odps/mars_extension/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/mars_extension/deploy/client.py` & `pyodps-0.9.5/odps/mars_extension/deploy/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,61 +10,50 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import base64
+import json
 import logging
 import time
 import requests
-import json
 
 from cupid import CupidSession
+from cupid.utils import build_image_name
 from mars.session import new_session
 
 from ...utils import write_log
 from ...models import Instance
 from ...config import options
 from ... import errors
 
 NOTEBOOK_NAME = 'MarsNotebook'
 CUPID_APP_NAME = 'MarsWeb'
-DEFAULT_RESOURCES = ['public.mars-0.4.6.zip', 'public.pyodps-0.9.3.2.zip', 'public.pyarrow.zip']
+DEFAULT_RESOURCES = ['public.mars-0.5.0.zip', 'public.pyodps-0.9.5.zip', 'public.pyarrow.zip']
 logger = logging.getLogger(__name__)
 
 
-def _build_namespace_config(namespace):
-    config = {
-        'kind': 'Namespace',
-        'metadata': {
-            'name': namespace,
-            'labels': {
-                'name': namespace
-            }
-        },
-    }
-    return config
-
-
 class MarsCupidClient(object):
     def __init__(self, odps, inst=None, project=None):
         self._odps = odps
         self._cupid_session = CupidSession(odps, project=project)
         self._kube_instance = inst
         self._kube_url = None
         self._kube_client = None
         self._kube_namespace = None
 
         self._scheduler_key = None
         self._scheduler_config = None
         self._worker_config = None
         self._web_config = None
         self._endpoint = None
-        self._has_notebook = False
+        self._with_notebook = False
         self._notebook_endpoint = None
 
         self._mars_session = None
         self._req_session = None
 
     @property
     def endpoint(self):
@@ -78,70 +67,74 @@
     def session(self):
         return self._mars_session
 
     @property
     def instance_id(self):
         return self._kube_instance.id
 
-    def submit(self, worker_num=1, worker_cpu=8, worker_mem=32, disk_num=1, min_worker_num=None, cache_mem=None,
-               resources=None, module_path=None, create_session=True, priority=None, running_cluster=None,
-               scheduler_num=1, notebook=None, task_name=None, **kw):
+    def submit(self, image=None, scheduler_num=1, scheduler_cpu=8, scheduler_mem=32 * 1024 ** 3,
+               worker_num=1, worker_cpu=8, worker_mem=32 * 1024 ** 3, worker_cache_mem=None,
+               min_worker_num=None, worker_disk_num=1, worker_disk_size=100 * 1024 ** 3,
+               web_num=1, web_cpu=1, web_mem=1024 ** 3, with_notebook=False, notebook_cpu=1,
+               notebook_mem=2 * 1024 ** 3, timeout=None, extra_env=None, extra_modules=None,
+               resources=None, create_session=True, priority=None, running_cluster=None,
+               task_name=None, **kw):
         try:
             async_ = kw.pop('async_', None)
+
+            # compatible with early version
+            mars_image = kw.pop('mars_image', None)
             default_resources = kw.pop('default_resources', None) or DEFAULT_RESOURCES
-            if notebook is not None:
-                self._has_notebook = bool(notebook)
+            instance_idle_timeout = kw.pop('instance_idle_timeout', None)
+            if with_notebook is not None:
+                self._with_notebook = bool(with_notebook)
             else:
-                self._has_notebook = options.mars.launch_notebook
+                self._with_notebook = options.mars.launch_notebook
             if self._kube_instance is None:
-                if module_path is not None:
-                    if isinstance(module_path, (tuple, list)):
-                        module_path = list(module_path) + ['odps.mars_extension']
-                    else:
-                        module_path = [module_path, 'odps.mars_extension']
+                image = image or mars_image or build_image_name('mars')
+
+                extra_modules = extra_modules or []
+                if isinstance(extra_modules, (tuple, list)):
+                    extra_modules = list(extra_modules) + ['odps.mars_extension']
+                else:
+                    extra_modules = [extra_modules, 'odps.mars_extension']
 
                 if resources is not None:
                     if isinstance(resources, (tuple, list)):
                         resources = list(resources)
                         resources.extend(default_resources)
                     else:
                         resources = [resources] + default_resources
                 else:
                     resources = default_resources
 
-                if cache_mem is None:
-                    cache_mem = str(worker_mem * 0.48) + 'G'
+                if worker_cache_mem is None:
+                    worker_cache_mem = int(worker_mem * 0.48)
                 else:
-                    cache_mem = str(cache_mem) + 'G'
-                mars_config = {
-                    'scheduler_num': scheduler_num,
-                    'worker_num': worker_num,
-                    'worker_cpu': worker_cpu,
-                    'worker_mem': worker_mem,
-                    'cache_mem': cache_mem or '',
-                    'disk_num': disk_num,
-                    'resources': resources,
-                    'module_path': module_path or ['odps.mars_extension'],
-                }
-                if 'mars_app_image' in kw:
-                    mars_config['mars_app_image'] = kw.pop('mars_app_image')
-                if 'mars_image' in kw:
-                    mars_config['mars_image'] = kw.pop('mars_image')
-                if 'proxy_endpoint' in kw:
-                    mars_config['proxy_endpoint'] = kw.pop('proxy_endpoint')
-                if 'major_task_version' in kw:
-                    mars_config['major_task_version'] = kw.pop('major_task_version')
-                mars_config['scheduler_mem'] = kw.pop('scheduler_mem', 32)
-                mars_config['scheduler_cpu'] = kw.pop('scheduler_cpu', 8)
+                    worker_cache_mem = worker_cache_mem
+
+                cluster_args = dict(
+                    image=image, scheduler_num=scheduler_num, scheduler_cpu=scheduler_cpu,
+                    scheduler_mem=scheduler_mem, worker_num=worker_num, worker_cpu=worker_cpu,
+                    worker_mem=worker_mem, worker_cache_mem=worker_cache_mem,
+                    min_worker_num=min_worker_num, worker_disk_num=worker_disk_num,
+                    worker_disk_size=worker_disk_size, web_num=web_num, web_cpu=web_cpu,
+                    web_mem=web_mem, with_notebook=with_notebook, notebook_cpu=notebook_cpu,
+                    notebook_mem=notebook_mem, extra_env=extra_env, extra_modules=extra_modules,
+                    instance_idle_timeout=instance_idle_timeout, timeout=timeout)
+
+                command = '/srv/entrypoint.sh %s %s' % (
+                    __name__.rsplit('.', 1)[0] + '.app',
+                    base64.b64encode(json.dumps(cluster_args).encode()).decode()
+                )
 
-                if self._has_notebook:
-                    mars_config['notebook'] = True
                 self._kube_instance = self._cupid_session.start_kubernetes(
                     async_=True, running_cluster=running_cluster, priority=priority,
-                    app_name='mars', app_config=mars_config, task_name=task_name, **kw)
+                    app_image=build_image_name('mars'), app_command=command, resources=resources,
+                    task_name=task_name, **kw)
                 write_log(self._kube_instance.get_logview_address())
             if async_:
                 return self
             else:
                 self.wait_for_success(create_session=create_session, min_worker_num=min_worker_num or worker_num)
                 return self
 
@@ -199,15 +192,15 @@
                     self._endpoint = self.get_mars_endpoint()
                     write_log('Mars UI: ' + self._endpoint)
                     self._req_session = self.get_req_session()
 
                     self._req_session.post(self._endpoint.rstrip('/') + '/api/logger', data=dict(
                         content='Mars UI from client: ' + self._endpoint
                     ))
-                if self._has_notebook and self._notebook_endpoint is None:
+                if self._with_notebook and self._notebook_endpoint is None:
                     self._notebook_endpoint = self.get_notebook_endpoint()
                     write_log('Notebook UI: ' + self._notebook_endpoint)
 
                     self._req_session.post(self._endpoint.rstrip('/') + '/api/logger', data=dict(
                         content='Notebook UI from client: ' + self._notebook_endpoint
                     ))
             except KeyboardInterrupt:
@@ -232,11 +225,15 @@
             except KeyboardInterrupt:
                 raise
             except:
                 if self._kube_instance and self._kube_instance.status == self._kube_instance.Status.RUNNING:
                     self._kube_instance.stop()
                 raise
 
+    def restart_session(self):
+        self._mars_session.close()
+        self._mars_session = new_session(self._endpoint, req_session=self._req_session).as_default()
+
     def stop_server(self):
         if self._kube_instance:
             self._kube_instance.stop()
             self._kube_instance = None
```

### Comparing `pyodps-0.9.3.2/odps/mars_extension/deploy/notebook.py` & `pyodps-0.9.5/odps/mars_extension/deploy/notebook.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,16 @@
     from cupid import context
     from mars.utils import get_next_port
 
     cupid_context = context()
     mars_endpoint = wait_mars_ready(cupid_context.kv_store(), CUPID_APP_NAME)
     host_addr = socket.gethostbyname(socket.gethostname())
 
+    os.environ.pop('KUBE_API_ADDRESS')
+
     if os.environ.get('VM_ENGINE_TYPE') == 'hyper':
         notebook_port = DEFAULT_NOTEBOOK_PORT
     else:
         notebook_port = str(get_next_port())
 
     endpoint = 'http://{0}:{1}'.format(host_addr, notebook_port)
```

### Comparing `pyodps-0.9.3.2/odps/mars_extension/deploy/utils.py` & `pyodps-0.9.5/odps/mars_extension/deploy/utils.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/mars_extension/deploy/__init__.py` & `pyodps-0.9.5/odps/mars_extension/deploy/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.
+# limitations under the License.
```

### Comparing `pyodps-0.9.3.2/odps/mars_extension/io/core.py` & `pyodps-0.9.5/odps/mars_extension/io/core.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/mars_extension/io/local.py` & `pyodps-0.9.5/odps/mars_extension/io/local.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/mars_extension/io/oss.py` & `pyodps-0.9.5/odps/mars_extension/io/oss.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/mars_extension/io/__init__.py` & `pyodps-0.9.5/odps/mars_extension/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/mars_extension/oss.py` & `pyodps-0.9.5/odps/mars_extension/oss.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/mars_extension/run_script.py` & `pyodps-0.9.5/odps/mars_extension/run_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import subprocess
 
 import numpy as np
 from mars.serialize import BytesField, ListField, Int32Field, StringField
 from mars.utils import to_binary
 
 
-logger = logging.getLogger('mars.worker')
+logger = logging.getLogger(__name__)
 
 try:
     from mars.remote.run_script import RunScript
 except ImportError:
     try:
         from mars.learn.operands import LearnMergeDictOperand, OutputType
     except ImportError:
```

### Comparing `pyodps-0.9.3.2/odps/mars_extension/tensor/datasource.py` & `pyodps-0.9.5/odps/mars_extension/tensor/datasource.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from mars.tensor.utils import decide_chunk_sizes, normalize_shape
 from mars.serialize import ValueType, ListField, StringField
 from mars import opcodes as OperandDef
 
 from ..io import glob
 from ...compat import izip, BytesIO
 
-logger = logging.getLogger(__file__)
+logger = logging.getLogger(__name__)
 
 
 class TensorTableCOO(TensorNoInput):
     _op_type_ = OperandDef.TABLE_COO
 
     _paths = ListField('paths', ValueType.string)
     _dim_cols = ListField('dim_cols', ValueType.string)
```

### Comparing `pyodps-0.9.3.2/odps/mars_extension/tensor/datastore.py` & `pyodps-0.9.5/odps/mars_extension/tensor/datastore.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/mars_extension/tensor/__init__.py` & `pyodps-0.9.5/odps/mars_extension/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/mars_extension/__init__.py` & `pyodps-0.9.5/odps/mars_extension/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,34 +19,29 @@
     from .core import create_mars_cluster, to_mars_dataframe, \
         persist_mars_dataframe, run_script_in_mars, run_mars_job, \
         list_mars_instances
 except ImportError:
     create_mars_cluster = None
     to_mars_dataframe = None
     persist_mars_dataframe = None
-    run_script_in_mars = None
+    run_mars_script = None
     run_mars_job = None
     list_mars_instances = None
 
 try:
     from . import dataframe
 except ImportError:
     dataframe = None
 
 try:
     from . import tensor
 except ImportError:
     tensor = None
 
 try:
-    from . import actors
-except ImportError:
-    actors = None
-
-try:
     from mars.executor import register
     from mars.remote.core import RemoteFunction
     from .core import execute_with_odps_context
     from .run_script import RunScript
 
     register(RemoteFunction, execute_with_odps_context(RemoteFunction.execute))
     register(RunScript, execute_with_odps_context(RunScript.execute))
```

### Comparing `pyodps-0.9.3.2/odps/ml/algolib/base_algo.py` & `pyodps-0.9.5/odps/ml/algolib/base_algo.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 
 from __future__ import absolute_import
 
 import functools
 import re
 import time
 import uuid
-from collections import namedtuple, Iterable
+from collections import namedtuple
 
 from odps.df.expr.dynamic import DynamicMixin
 from .objects import SchemaDef
 from ..expr import ModelDataCollectionExpr, ODPSModelExpr
 from ..expr.op import ProgrammaticFieldChangeOperation
 from ..pipeline.core import PipelineStep
 from ..utils import import_class_member, get_function_args, ML_ARG_PREFIX
-from ...compat import six, OrderedDict, irange
+from ...compat import six, OrderedDict, irange, Iterable
 from ...df.core import DataFrame
 from ...models import Schema as TableSchema
 from ..enums import PortType, PortDirection
 from ...utils import underline_to_capitalized, camel_to_underline, survey
 
 
 def is_df_object(obj):
```

### Comparing `pyodps-0.9.3.2/odps/ml/algolib/loader.py` & `pyodps-0.9.5/odps/ml/algolib/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
 import textwrap
-from collections import Iterable
 from functools import partial
 
 from .objects import AlgorithmsDef, AlgorithmDef
 from ..expr import AlgoCollectionExpr, ODPSModelExpr, MetricsResultExpr
 from ..enums import PortType
 from ..utils import import_class_member, get_function_args, ML_ARG_PREFIX
-from ...compat import OrderedDict, six
+from ...compat import OrderedDict, six, Iterable
 from ...df.expr.collections import SequenceExpr
 from ...utils import camel_to_underline, underline_to_capitalized, load_static_text_file,\
     load_internal_static_text_file, survey
 
 SYSTEM_PARAMS = set("""
 isInheritLastType inputTableName inputTablePartitions outputTableName outputTablePartition
 """.strip().split())
```

### Comparing `pyodps-0.9.3.2/odps/ml/algolib/objects.py` & `pyodps-0.9.5/odps/ml/algolib/objects.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/algolib/__init__.py` & `pyodps-0.9.5/odps/ml/algolib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/classifiers/_customize.py` & `pyodps-0.9.5/odps/ml/classifiers/_customize.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/classifiers/__init__.py` & `pyodps-0.9.5/odps/ml/classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/clustering/_customize.py` & `pyodps-0.9.5/odps/ml/clustering/_customize.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/clustering/__init__.py` & `pyodps-0.9.5/odps/ml/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/cross_validation.py` & `pyodps-0.9.5/odps/ml/cross_validation.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/engine.py` & `pyodps-0.9.5/odps/ml/engine.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/enums.py` & `pyodps-0.9.5/odps/ml/enums.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/expr/core.py` & `pyodps-0.9.5/odps/ml/expr/core.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/expr/exporters.py` & `pyodps-0.9.5/odps/ml/expr/exporters.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/expr/mixin.py` & `pyodps-0.9.5/odps/ml/expr/mixin.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/expr/models/base.py` & `pyodps-0.9.5/odps/ml/expr/models/base.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/expr/models/pmml.py` & `pyodps-0.9.5/odps/ml/expr/models/pmml.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/expr/models/__init__.py` & `pyodps-0.9.5/odps/ml/expr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/expr/op.py` & `pyodps-0.9.5/odps/ml/expr/op.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/expr/specialized.py` & `pyodps-0.9.5/odps/ml/expr/specialized.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/expr/__init__.py` & `pyodps-0.9.5/odps/ml/expr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/feature/_customize.py` & `pyodps-0.9.5/odps/ml/feature/_customize.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/feature/__init__.py` & `pyodps-0.9.5/odps/ml/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/metrics/classification.py` & `pyodps-0.9.5/odps/ml/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/metrics/clustering.py` & `pyodps-0.9.5/odps/ml/metrics/clustering.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/metrics/regression.py` & `pyodps-0.9.5/odps/ml/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/metrics/scorer.py` & `pyodps-0.9.5/odps/ml/metrics/scorer.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/metrics/utils.py` & `pyodps-0.9.5/odps/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/metrics/_customize.py` & `pyodps-0.9.5/odps/ml/metrics/_customize.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/metrics/__init__.py` & `pyodps-0.9.5/odps/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/models.py` & `pyodps-0.9.5/odps/ml/models.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/network/_customize.py` & `pyodps-0.9.5/odps/ml/network/_customize.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/network/__init__.py` & `pyodps-0.9.5/odps/ml/network/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/pipeline/core.py` & `pyodps-0.9.5/odps/ml/pipeline/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from collections import namedtuple, Iterable
+
+from collections import namedtuple
 from copy import deepcopy
 from types import MethodType
 
-from ...compat import OrderedDict, reduce, six
+from ...compat import OrderedDict, reduce, six, Iterable
 from ...utils import camel_to_underline, is_namedtuple
 from ..expr.mixin import merge_data
 from ..utils import FieldRole
 
 
 class PipelineBit(object):
     def __init__(self, step, output):
```

### Comparing `pyodps-0.9.3.2/odps/ml/pipeline/steps.py` & `pyodps-0.9.5/odps/ml/pipeline/steps.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/pipeline/__init__.py` & `pyodps-0.9.5/odps/ml/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/preprocess/_customize.py` & `pyodps-0.9.5/odps/ml/preprocess/_customize.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
-from collections import Iterable
 
-from ...compat import six
+from ...compat import six, Iterable
 from ...serializers import JSONSerializableModel, JSONNodeField
 from ..utils import ML_ARG_PREFIX
 
 """
 Exporter
 """
```

### Comparing `pyodps-0.9.3.2/odps/ml/preprocess/__init__.py` & `pyodps-0.9.5/odps/ml/preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/recommend/_customize.py` & `pyodps-0.9.5/odps/ml/recommend/_customize.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/recommend/__init__.py` & `pyodps-0.9.5/odps/ml/recommend/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/regression/__init__.py` & `pyodps-0.9.5/odps/ml/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/runners.py` & `pyodps-0.9.5/odps/ml/runners.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/statistics/_customize.py` & `pyodps-0.9.5/odps/ml/statistics/_customize.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/statistics/__init__.py` & `pyodps-0.9.5/odps/ml/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/tensor/__init__.py` & `pyodps-0.9.5/odps/ml/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/text/_customize.py` & `pyodps-0.9.5/odps/ml/text/_customize.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/text/__init__.py` & `pyodps-0.9.5/odps/ml/text/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/timeseries/_customize.py` & `pyodps-0.9.5/odps/ml/timeseries/_customize.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/timeseries/__init__.py` & `pyodps-0.9.5/odps/ml/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ml/utils.py` & `pyodps-0.9.5/odps/ml/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 import logging
 import time
 from json import JSONEncoder
 from types import FunctionType, MethodType
 from copy import deepcopy
 from functools import partial
 from threading import Thread
-from collections import namedtuple, Iterable
+from collections import namedtuple
 
 from .. import options
-from ..compat import six, getargspec
+from ..compat import six, getargspec, Iterable
 from ..types import Partition
 from ..utils import camel_to_underline, TEMP_TABLE_PREFIX
 from .enums import FieldContinuity, FieldRole
 
 ML_PACKAGE_ROOT = 'odps.ml'
 ML_INTERNAL_PACKAGE_ROOT = 'odps.internal.ml'
 TEMP_MODEL_PREFIX = 'pm_'
```

### Comparing `pyodps-0.9.3.2/odps/ml/__init__.py` & `pyodps-0.9.5/odps/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/cache.py` & `pyodps-0.9.5/odps/models/cache.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/core.py` & `pyodps-0.9.5/odps/models/core.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/function.py` & `pyodps-0.9.5/odps/models/function.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/functions.py` & `pyodps-0.9.5/odps/models/functions.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/instance.py` & `pyodps-0.9.5/odps/models/instance.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/instances.py` & `pyodps-0.9.5/odps/models/instances.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/job.py` & `pyodps-0.9.5/odps/models/job.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/ml/offlinemodel.py` & `pyodps-0.9.5/odps/models/ml/offlinemodel.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/ml/offlinemodels.py` & `pyodps-0.9.5/odps/models/ml/offlinemodels.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/ml/__init__.py` & `pyodps-0.9.5/odps/models/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/partition.py` & `pyodps-0.9.5/odps/models/partition.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/partitions.py` & `pyodps-0.9.5/odps/models/partitions.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/project.py` & `pyodps-0.9.5/odps/models/project.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/projects.py` & `pyodps-0.9.5/odps/models/projects.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/record.py` & `pyodps-0.9.5/odps/models/record.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/resource.py` & `pyodps-0.9.5/odps/models/resource.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/resources.py` & `pyodps-0.9.5/odps/models/resources.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/security/config.py` & `pyodps-0.9.5/odps/models/security/config.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/security/roles.py` & `pyodps-0.9.5/odps/models/security/roles.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/security/users.py` & `pyodps-0.9.5/odps/models/security/users.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/security/__init__.py` & `pyodps-0.9.5/odps/models/security/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/session.py` & `pyodps-0.9.5/odps/models/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,23 +152,24 @@
 class InSessionInstance(Instance):
     """
         This represents the instance created
         for SQL tasks that run inside a session. This instance is useful
         when fetching results.
     """
 
-    __slots__ = ('_project_name', '_session_task_name', '_session_instance', '_is_select')
+    __slots__ = ('_project_name', '_session_task_name', '_session_instance', '_is_select', '_subquery_id')
 
     def __init__(self, **kw):
         if ('session_task_name' not in kw) or ('session_project_name' not in kw) or ('session_instance' not in kw):
             raise errors.InvalidArgument("Creating InSessionInstance without enough information.")
         self._session_task_name = kw.pop("session_task_name", "")
         self._project_name = kw.pop("session_project_name", "")
         self._session_instance = kw.pop("session_instance", None)
         self._is_select = kw.pop("session_is_select", False)
+        self._subquery_id = -1
         super(InSessionInstance, self).__init__(**kw)
 
     @utils.survey
     def _open_result_reader(self, schema=None, task_name=None, **_):
         # you just can't.
         # for non-select SQL, no result you may fetch.
         # for select SQL, use instance tunnel. This is deprecated.
@@ -176,31 +177,34 @@
             raise errors.InstanceTypeNotSupported("Use tunnel to fetch select result.")
         else:
             raise errors.InstanceTypeNotSupported("No results for non-select SQL.")
 
     def _open_tunnel_reader(self, **kw):
         if not self._is_select:
             raise errors.InstanceTypeNotSupported("InstanceTunnel cannot be opened at a non-select SQL Task.")
+        
+        while (self._subquery_id == -1) and (self._status != Instance.Status.TERMINATED):
+            self.reload()
+        
+        if self._subquery_id == -1:
+            raise errors.InternalServerError("SubQueryId not returned by the server.")
 
         from ..tunnel.instancetunnel import InstanceDownloadSession
 
         reopen = kw.pop('reopen', False)
         endpoint = kw.pop('endpoint', None)
         kw['sessional'] = True
+        kw['session_subquery_id'] = self._subquery_id
         if 'session_task_name' not in kw:
             kw['session_task_name'] = self._session_task_name
 
         tunnel = self._create_instance_tunnel(endpoint=endpoint)
-        download_id = self._download_id if not reopen else None
 
         try:
-            download_session = tunnel.create_download_session(instance=self,
-                                                              download_id=download_id, **kw)
-            if download_id and download_session.status != InstanceDownloadSession.Status.Normal:
-                download_session = tunnel.create_download_session(instance=self, **kw)
+            download_session = tunnel.create_download_session(instance=self, **kw)
         except errors.InternalServerError:
             e, tb = sys.exc_info()[1:]
             e.__class__ = Instance.DownloadSessionCreationError
             six.reraise(Instance.DownloadSessionCreationError, e, tb)
 
         self._download_id = download_session.id
 
@@ -210,15 +214,14 @@
                 self._schema = download_session.schema
 
             @property
             def count(self):
                 # we can't count session results before it's
                 # fully retrieved.
                 return -1
-
             @property
             def status(self):
                 # force reload to update download session status
                 # this is for supporting the stream download of instance tunnel
                 # without the following line will not trigger reload
                 download_session.reload()
                 return download_session.status
@@ -264,9 +267,10 @@
             query_reslt = json.loads(st_resp.text)
             if query_reslt["status"] == SessionTaskStatus.Terminated.value:
                 self._status = Instance.Status.TERMINATED
             elif query_reslt["status"] == SessionTaskStatus.Running.value:
                 self._status = Instance.Status.RUNNING
             else:
                 self._status = Instance.Status.SUSPENDED
+            self._subquery_id = int(query_reslt.get("subQueryId", -1))
         except BaseException as ex:
             raise errors.ODPSError("Invalid Response Format: %s\n Response JSON:%s\n" % (str(ex), st_resp.text))
```

### Comparing `pyodps-0.9.3.2/odps/models/table.py` & `pyodps-0.9.5/odps/models/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     storage_handler = serializers.JSONNodeField(
         'storageHandler', set_to_parent=True)
     resources = serializers.JSONNodeField(
         'resources', set_to_parent=True)
     serde_properties = serializers.JSONNodeField(
         'serDeProperties', type='json', set_to_parent=True)
     reserved = serializers.JSONNodeField(
-        'reserved', type='json', set_to_parent=True)
+        'Reserved', type='json', set_to_parent=True)
     shard = serializers.JSONNodeReferenceField(
         Shard, 'shardInfo', check_before=['shardExist'], set_to_parent=True)
     table_label = serializers.JSONNodeField(
         'tableLabel', callback=lambda t: t if t != '0' else '', set_to_parent=True)
     _columns = serializers.JSONNodesReferencesField(TableColumn, 'columns')
     _partitions = serializers.JSONNodesReferencesField(TablePartition, 'partitionKeys')
 
@@ -255,14 +255,18 @@
                     repr(partition.type).ljust(type_space),
                     '# {0}'.format(utils.to_str(partition.comment)) if not_empty(partition.comment) else ''
                 ))
             buf.write(utils.indent('\n'.join(partition_strs), 4))
 
         return buf.getvalue()
 
+    @property
+    def stored_as(self):
+        return (self.reserved or dict()).get('StoredAs')
+
     @staticmethod
     def gen_create_table_sql(table_name, table_schema, comment=None, if_not_exists=False,
                              lifecycle=None, shard_num=None, hub_lifecycle=None,
                              with_column_comments=True, project=None, **kw):
         from ..utils import escape_odps_string
 
         buf = six.StringIO()
```

### Comparing `pyodps-0.9.3.2/odps/models/tables.py` & `pyodps-0.9.5/odps/models/tables.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/tasks.py` & `pyodps-0.9.5/odps/models/tasks.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/volumes.py` & `pyodps-0.9.5/odps/models/volumes.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/volume_fs.py` & `pyodps-0.9.5/odps/models/volume_fs.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/volume_parted.py` & `pyodps-0.9.5/odps/models/volume_parted.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/worker.py` & `pyodps-0.9.5/odps/models/worker.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/xflow.py` & `pyodps-0.9.5/odps/models/xflow.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/xflows.py` & `pyodps-0.9.5/odps/models/xflows.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/models/__init__.py` & `pyodps-0.9.5/odps/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/readers.py` & `pyodps-0.9.5/odps/readers.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/rest.py` & `pyodps-0.9.5/odps/rest.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/serializers.py` & `pyodps-0.9.5/odps/serializers.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/src/crc32.c` & `pyodps-0.9.5/odps/src/crc32.c`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/src/crc32c_c.pxd` & `pyodps-0.9.5/odps/src/crc32c_c.pxd`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/src/crc32c_c.pyx` & `pyodps-0.9.5/odps/src/crc32c_c.pyx`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/src/types_c.pxd` & `pyodps-0.9.5/odps/src/types_c.pxd`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/src/types_c.pyx` & `pyodps-0.9.5/odps/src/types_c.pyx`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/src/__init__.py` & `pyodps-0.9.5/odps/src/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/algorithms/classifier.xml` & `pyodps-0.9.5/odps/static/algorithms/classifier.xml`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/algorithms/clustering.xml` & `pyodps-0.9.5/odps/static/algorithms/clustering.xml`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/algorithms/feature.xml` & `pyodps-0.9.5/odps/static/algorithms/feature.xml`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/algorithms/metrics.xml` & `pyodps-0.9.5/odps/static/algorithms/metrics.xml`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/algorithms/network.xml` & `pyodps-0.9.5/odps/static/algorithms/network.xml`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/algorithms/preprocess.xml` & `pyodps-0.9.5/odps/static/algorithms/preprocess.xml`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/algorithms/recommend.xml` & `pyodps-0.9.5/odps/static/algorithms/recommend.xml`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/algorithms/regression.xml` & `pyodps-0.9.5/odps/static/algorithms/regression.xml`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/algorithms/statistics.xml` & `pyodps-0.9.5/odps/static/algorithms/statistics.xml`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/algorithms/text.xml` & `pyodps-0.9.5/odps/static/algorithms/text.xml`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/data/dow_jones.txt` & `pyodps-0.9.5/odps/static/data/dow_jones.txt`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/data/ionosphere.txt` & `pyodps-0.9.5/odps/static/data/ionosphere.txt`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/data/iris.txt` & `pyodps-0.9.5/odps/static/data/iris.txt`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/data/splited_words.txt` & `pyodps-0.9.5/odps/static/data/splited_words.txt`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/Gruntfile.js` & `pyodps-0.9.5/odps/static/ui/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/chosen-sprite.png` & `pyodps-0.9.5/odps/static/ui/src/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/chosen-sprite@2x.png` & `pyodps-0.9.5/odps/static/ui/src/chosen-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/chosen.css` & `pyodps-0.9.5/odps/static/ui/src/chosen.css`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/chosen.js` & `pyodps-0.9.5/odps/static/ui/src/chosen.js`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/common.js` & `pyodps-0.9.5/odps/static/ui/src/common.js`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/df-view.js` & `pyodps-0.9.5/odps/static/ui/src/df-view.js`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/echarts.min.js` & `pyodps-0.9.5/odps/static/ui/src/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/fonts/custom-font.css` & `pyodps-0.9.5/odps/static/ui/src/fonts/custom-font.css`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/fonts/custom-font.eot` & `pyodps-0.9.5/odps/static/ui/src/fonts/custom-font.eot`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/fonts/custom-font.svg` & `pyodps-0.9.5/odps/static/ui/src/fonts/custom-font.svg`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/fonts/custom-font.ttf` & `pyodps-0.9.5/odps/static/ui/src/fonts/custom-font.ttf`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/fonts/custom-font.woff` & `pyodps-0.9.5/odps/static/ui/src/fonts/custom-font.woff`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/html-notify.js` & `pyodps-0.9.5/odps/static/ui/src/html-notify.js`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/ml-retry.js` & `pyodps-0.9.5/odps/static/ui/src/ml-retry.js`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/progress.js` & `pyodps-0.9.5/odps/static/ui/src/progress.js`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/styles.css` & `pyodps-0.9.5/odps/static/ui/src/styles.css`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/src/westeros.js` & `pyodps-0.9.5/odps/static/ui/src/westeros.js`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/target/chosen-sprite.png` & `pyodps-0.9.5/odps/static/ui/target/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/target/chosen-sprite@2x.png` & `pyodps-0.9.5/odps/static/ui/target/chosen-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/target/chosen.css` & `pyodps-0.9.5/odps/static/ui/target/chosen.css`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/target/fonts/custom-font.eot` & `pyodps-0.9.5/odps/static/ui/target/fonts/custom-font.eot`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/target/fonts/custom-font.svg` & `pyodps-0.9.5/odps/static/ui/target/fonts/custom-font.svg`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/target/fonts/custom-font.ttf` & `pyodps-0.9.5/odps/static/ui/target/fonts/custom-font.ttf`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/target/fonts/custom-font.woff` & `pyodps-0.9.5/odps/static/ui/target/fonts/custom-font.woff`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/target/main.js` & `pyodps-0.9.5/odps/static/ui/target/main.js`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/static/ui/target/styles.css` & `pyodps-0.9.5/odps/static/ui/target/styles.css`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tempobj.py` & `pyodps-0.9.5/odps/tempobj.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/base.py` & `pyodps-0.9.5/odps/tunnel/base.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/checksum.py` & `pyodps-0.9.5/odps/tunnel/checksum.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/checksum_c.pxd` & `pyodps-0.9.5/odps/tunnel/checksum_c.pxd`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/checksum_c.pyx` & `pyodps-0.9.5/odps/tunnel/checksum_c.pyx`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/errors.py` & `pyodps-0.9.5/odps/tunnel/errors.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/instancetunnel.py` & `pyodps-0.9.5/odps/tunnel/instancetunnel.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,23 +17,24 @@
 from .base import BaseTunnel
 from .io.reader import TunnelRecordReader
 from .io.stream import CompressOption, SnappyRequestsInputStream, RequestsInputStream
 from .errors import TunnelError
 from .. import errors, serializers, types
 from ..compat import Enum, six
 from ..models import Projects, Schema
+from ..models.table import TableSchema
 
 try:
     import numpy as np
 except ImportError:
     np = None
 
 
 class InstanceDownloadSession(serializers.JSONSerializableModel):
-    __slots__ = '_client', '_instance', '_limit_enabled', '_compress_option', '_sessional', '_session_task_name'
+    __slots__ = '_client', '_instance', '_limit_enabled', '_compress_option', '_sessional', '_session_task_name', '_session_subquery_id'
 
     class Status(Enum):
         Unknown = 'UNKNOWN'
         Normal = 'NORMAL'
         Closes = 'CLOSES'
         Expired = 'EXPIRED'
         Failed = 'FAILED'
@@ -50,89 +51,104 @@
         super(InstanceDownloadSession, self).__init__()
 
         self._client = client
         self._instance = instance
         self._limit_enabled = limit if limit is not None else kw.get('limit_enabled', False)
         self._sessional = kw.pop("sessional", False)
         self._session_task_name = kw.pop("session_task_name", "")
-        if self._sessional and (not self._session_task_name):
-            raise TunnelError("Taskname('sess_tname') keyword argument must be provided for session instance tunnels.")
+        self._session_subquery_id = int(kw.pop("session_subquery_id", -1))
+        if self._sessional and ((not self._session_task_name) or (self._session_subquery_id == -1)):
+            raise TunnelError("Taskname('session_task_name') and Subquery ID ('session_subquery_id') keyword argument must be provided for session instance tunnels.")
 
         if download_id is None:
             self._init()
         else:
             self.id = download_id
             self.reload()
         self._compress_option = compress_option
 
     def _init(self):
         params = {'downloads': ''}
         headers = {'Content-Length': 0}
-        if self._sessional:
-            params['cached'] = ''
-            params['taskname'] = self._session_task_name
-
-        if self._limit_enabled:
-            params['instance_tunnel_limit_enabled'] = ''
-
-        url = self._instance.resource()
-        resp = self._client.post(url, {}, params=params, headers=headers)
-        if self._client.is_ok(resp):
-            self.parse(resp, obj=self)
-            if self.schema is not None:
-                self.schema.build_snapshot()
-        else:
-            e = TunnelError.parse(resp)
-            raise e
+        # Now we use DirectDownloadMode to fetch session results(any other method is removed)
+        # This mode, only one request needed. So we dont have to send request here ..
+        if not self._sessional:
+            if self._limit_enabled:
+                params['instance_tunnel_limit_enabled'] = ''
+            url = self._instance.resource()
+            resp = self._client.post(url, {}, params=params, headers=headers)
+            if self._client.is_ok(resp):
+                self.parse(resp, obj=self)
+                if self.schema is not None:
+                    self.schema.build_snapshot()
+            else:
+                e = TunnelError.parse(resp)
+                raise e
 
     def reload(self):
-        params = {'downloadid': self.id}
-        headers = {'Content-Length': 0}
-        if self._sessional:
-            params['cached'] = ''
-            params['taskname'] = self._session_task_name
-
-        url = self._instance.resource()
-        resp = self._client.get(url, params=params, headers=headers)
-        if self._client.is_ok(resp):
-            self.parse(resp, obj=self)
-            if self.schema is not None:
-                self.schema.build_snapshot()
+        if not self._sessional:
+            params = {'downloadid': self.id}
+            headers = {'Content-Length': 0}
+            if self._sessional:
+                params['cached'] = ''
+                params['taskname'] = self._session_task_name
+
+            url = self._instance.resource()
+            resp = self._client.get(url, params=params, headers=headers)
+            if self._client.is_ok(resp):
+                self.parse(resp, obj=self)
+                if self.schema is not None:
+                    self.schema.build_snapshot()
+            else:
+                e = TunnelError.parse(resp)
+                raise e
         else:
-            e = TunnelError.parse(resp)
-            raise e
+            self.status = InstanceDownloadSession.Status.Normal
+
 
     def _open_reader(self, start, count, compress=False, columns=None, reader_cls=None):
         compress_option = self._compress_option or CompressOption()
 
         params = {}
-        headers = {'Content-Length': 0, 'x-odps-tunnel-version': 4}
+        headers = {'x-odps-tunnel-version': 4}
+        if self._sessional:
+            params['cached'] = ''
+            params['taskname'] = self._session_task_name
+            params['queryid'] = str(self._session_subquery_id)
+        else:
+            params['downloadid'] = self.id
+            params['rowrange'] = '(%s,%s)' % (start, count)
+            headers['Content-Length'] = 0
         if compress:
             if compress_option.algorithm == \
                     CompressOption.CompressAlgorithm.ODPS_ZLIB:
                 headers['Accept-Encoding'] = 'deflate'
             elif compress_option.algorithm == \
                     CompressOption.CompressAlgorithm.ODPS_SNAPPY:
                 headers['Accept-Encoding'] = 'x-snappy-framed'
             elif compress_option.algorithm != \
                     CompressOption.CompressAlgorithm.ODPS_RAW:
                 raise TunnelError('invalid compression option')
-        params['downloadid'] = self.id
         params['data'] = ''
-        if not self._sessional:
-            params['rowrange'] = '(%s,%s)' % (start, count)
         if columns is not None and len(columns) > 0:
             col_name = lambda col: col.name if isinstance(col, types.Column) else col
             params['columns'] = ','.join(col_name(col) for col in columns)
 
         url = self._instance.resource()
         resp = self._client.get(url, stream=True, params=params, headers=headers)
         if not self._client.is_ok(resp):
             e = TunnelError.parse(resp)
             raise e
+        
+        if self._sessional:
+            # in DirectDownloadMode, the schema is brought back in HEADER.
+            # handle this.
+            schema_json = resp.headers.get('odps-tunnel-schema')
+            self.schema = TableSchema()
+            self.schema = self.schema.deserial(schema_json)
 
         content_encoding = resp.headers.get('Content-Encoding')
         if content_encoding is not None:
             if content_encoding == 'deflate':
                 self._compress_option = CompressOption(
                     CompressOption.CompressAlgorithm.ODPS_ZLIB, -1, 0)
             elif content_encoding == 'x-snappy-framed':
```

### Comparing `pyodps-0.9.3.2/odps/tunnel/io/reader.py` & `pyodps-0.9.5/odps/tunnel/io/reader.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/io/reader_c.pxd` & `pyodps-0.9.5/odps/tunnel/io/reader_c.pxd`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/io/reader_c.pyx` & `pyodps-0.9.5/odps/tunnel/io/reader_c.pyx`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/io/stream.py` & `pyodps-0.9.5/odps/tunnel/io/stream.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/io/writer.py` & `pyodps-0.9.5/odps/tunnel/io/writer.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/io/writer_c.pxd` & `pyodps-0.9.5/odps/tunnel/io/writer_c.pxd`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/io/writer_c.pyx` & `pyodps-0.9.5/odps/tunnel/io/writer_c.pyx`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/io/__init__.py` & `pyodps-0.9.5/odps/tunnel/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pb/decoder.py` & `pyodps-0.9.5/odps/tunnel/pb/decoder.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pb/decoder_c.pxd` & `pyodps-0.9.5/odps/tunnel/pb/decoder_c.pxd`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pb/decoder_c.pyx` & `pyodps-0.9.5/odps/tunnel/pb/decoder_c.pyx`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pb/encoder.py` & `pyodps-0.9.5/odps/tunnel/pb/encoder.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pb/encoder_c.pxd` & `pyodps-0.9.5/odps/tunnel/pb/encoder_c.pxd`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pb/encoder_c.pyx` & `pyodps-0.9.5/odps/tunnel/pb/encoder_c.pyx`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pb/errors.py` & `pyodps-0.9.5/odps/tunnel/pb/errors.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pb/input_stream.py` & `pyodps-0.9.5/odps/tunnel/pb/input_stream.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pb/output_stream.py` & `pyodps-0.9.5/odps/tunnel/pb/output_stream.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pb/util_c.pxd` & `pyodps-0.9.5/odps/tunnel/pb/util_c.pxd`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pb/util_c.pyx` & `pyodps-0.9.5/odps/tunnel/pb/util_c.pyx`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pb/wire_format.py` & `pyodps-0.9.5/odps/tunnel/pb/wire_format.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pb/__init__.py` & `pyodps-0.9.5/odps/tunnel/pb/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pdio/block_decoder_c.pxd` & `pyodps-0.9.5/odps/tunnel/pdio/block_decoder_c.pxd`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pdio/block_decoder_c.pyx` & `pyodps-0.9.5/odps/tunnel/pdio/block_decoder_c.pyx`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pdio/block_encoder_c.pxd` & `pyodps-0.9.5/odps/tunnel/pdio/block_encoder_c.pxd`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pdio/block_encoder_c.pyx` & `pyodps-0.9.5/odps/tunnel/pdio/block_encoder_c.pyx`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pdio/errno.py` & `pyodps-0.9.5/odps/tunnel/pdio/errno.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pdio/pdreader_c.pxd` & `pyodps-0.9.5/odps/tunnel/pdio/pdreader_c.pxd`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pdio/pdreader_c.pyx` & `pyodps-0.9.5/odps/tunnel/pdio/pdreader_c.pyx`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pdio/pdwriter.py` & `pyodps-0.9.5/odps/tunnel/pdio/pdwriter.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pdio/pdwriter_c.pxd` & `pyodps-0.9.5/odps/tunnel/pdio/pdwriter_c.pxd`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pdio/pdwriter_c.pyx` & `pyodps-0.9.5/odps/tunnel/pdio/pdwriter_c.pyx`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pdio/util_c.pxd` & `pyodps-0.9.5/odps/tunnel/pdio/util_c.pxd`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/pdio/__init__.py` & `pyodps-0.9.5/odps/tunnel/pdio/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/tabletunnel.py` & `pyodps-0.9.5/odps/tunnel/tabletunnel.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/volumetunnel.py` & `pyodps-0.9.5/odps/tunnel/volumetunnel.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/wireconstants.py` & `pyodps-0.9.5/odps/tunnel/wireconstants.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/tunnel/__init__.py` & `pyodps-0.9.5/odps/tunnel/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/types.py` & `pyodps-0.9.5/odps/types.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/udf/runtime.py` & `pyodps-0.9.5/odps/udf/runtime.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/udf/tools/runners.py` & `pyodps-0.9.5/odps/udf/tools/runners.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/udf/tools/utils.py` & `pyodps-0.9.5/odps/udf/tools/utils.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/udf/tools/__init__.py` & `pyodps-0.9.5/odps/udf/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/udf/__init__.py` & `pyodps-0.9.5/odps/udf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ui/common.py` & `pyodps-0.9.5/odps/ui/common.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ui/progress.py` & `pyodps-0.9.5/odps/ui/progress.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/ui/__init__.py` & `pyodps-0.9.5/odps/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/utils.py` & `pyodps-0.9.5/odps/utils.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/odps/_version.py` & `pyodps-0.9.5/odps/_version.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-version_info = (0, 9, 3, 2)
+version_info = (0, 9, 5)
 _num_index = max(idx if isinstance(v, int) else 0
                  for idx, v in enumerate(version_info))
 __version__ = '.'.join(map(str, version_info[:_num_index + 1])) + \
               ''.join(version_info[_num_index + 1:])
```

### Comparing `pyodps-0.9.3.2/odps/__init__.py` & `pyodps-0.9.5/odps/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/PKG-INFO` & `pyodps-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodps
-Version: 0.9.3.2
+Version: 0.9.5
 Summary: ODPS Python SDK and data analysis framework
 Home-page: http://github.com/aliyun/aliyun-odps-python-sdk
 Author: Wu Wei
 Author-email: weiwu@cacheme.net
 Maintainer: Qin Xuye
 Maintainer-email: qin@qinxuye.me
 License: Apache License 2.0
```

### Comparing `pyodps-0.9.3.2/pyodps.egg-info/PKG-INFO` & `pyodps-0.9.5/pyodps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodps
-Version: 0.9.3.2
+Version: 0.9.5
 Summary: ODPS Python SDK and data analysis framework
 Home-page: http://github.com/aliyun/aliyun-odps-python-sdk
 Author: Wu Wei
 Author-email: weiwu@cacheme.net
 Maintainer: Qin Xuye
 Maintainer-email: qin@qinxuye.me
 License: Apache License 2.0
```

### Comparing `pyodps-0.9.3.2/pyodps.egg-info/SOURCES.txt` & `pyodps-0.9.5/pyodps.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -145,32 +145,36 @@
 odps/lib/tzlocal/win32.py
 odps/lib/tzlocal/windows_tz.py
 odps/mars_extension/__init__.py
 odps/mars_extension/core.py
 odps/mars_extension/oss.py
 odps/mars_extension/run_script.py
 odps/mars_extension/actors/__init__.py
-odps/mars_extension/actors/prochelper.py
+odps/mars_extension/actors/session.py
 odps/mars_extension/dataframe/__init__.py
 odps/mars_extension/dataframe/datasource.py
 odps/mars_extension/dataframe/datastore.py
 odps/mars_extension/deploy/__init__.py
+odps/mars_extension/deploy/app.py
 odps/mars_extension/deploy/client.py
+odps/mars_extension/deploy/core.py
 odps/mars_extension/deploy/notebook.py
 odps/mars_extension/deploy/scheduler.py
 odps/mars_extension/deploy/utils.py
 odps/mars_extension/deploy/web.py
 odps/mars_extension/deploy/worker.py
 odps/mars_extension/io/__init__.py
 odps/mars_extension/io/core.py
 odps/mars_extension/io/local.py
 odps/mars_extension/io/oss.py
 odps/mars_extension/tensor/__init__.py
 odps/mars_extension/tensor/datasource.py
 odps/mars_extension/tensor/datastore.py
+odps/mars_extension/web/__init__.py
+odps/mars_extension/web/apihandlers.py
 odps/ml/__init__.py
 odps/ml/cross_validation.py
 odps/ml/engine.py
 odps/ml/enums.py
 odps/ml/models.py
 odps/ml/runners.py
 odps/ml/utils.py
```

### Comparing `pyodps-0.9.3.2/README.rst` & `pyodps-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/scripts/pyou` & `pyodps-0.9.5/scripts/pyou`

 * *Files identical despite different names*

### Comparing `pyodps-0.9.3.2/setup.py` & `pyodps-0.9.5/setup.py`

 * *Files identical despite different names*

