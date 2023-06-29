# Comparing `tmp/polygon-etl-0.3.6.tar.gz` & `tmp/polygon-etl-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polygon-etl-0.3.6.tar", last modified: Mon May 15 10:01:58 2023, max compression
+gzip compressed data, was "polygon-etl-0.3.7.tar", last modified: Thu Jun 29 10:21:54 2023, max compression
```

## Comparing `polygon-etl-0.3.6.tar` & `polygon-etl-0.3.7.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.506116 polygon-etl-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-15 10:01:58.506116 polygon-etl-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.494116 polygon-etl-0.3.6/polygon_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-15 10:01:58.000000 polygon-etl-0.3.6/polygon_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-15 10:01:58.000000 polygon-etl-0.3.6/polygon_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:01:58.000000 polygon-etl-0.3.6/polygon_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 10:01:58.000000 polygon-etl-0.3.6/polygon_etl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-15 10:01:58.000000 polygon-etl-0.3.6/polygon_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 10:01:58.000000 polygon-etl-0.3.6/polygon_etl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.498116 polygon-etl-0.3.6/polygonetl/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/atomic_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.498116 polygon-etl-0.3.6/polygonetl/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/export_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/export_blocks_and_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/export_contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/export_geth_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/export_receipts_and_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/export_token_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/export_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/export_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/extract_contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/extract_csv_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/extract_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/extract_geth_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/extract_token_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/extract_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/filter_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/get_block_range_for_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/get_block_range_for_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/get_keccak_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/cli/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/csv_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.498116 polygon-etl-0.3.6/polygonetl/domain/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/geth_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/receipt_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/token_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/domain/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.498116 polygon-etl-0.3.6/polygonetl/enumeration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/enumeration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/enumeration/entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/erc20_abi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.502116 polygon-etl-0.3.6/polygonetl/executors/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/executors/batch_work_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/executors/bounded_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/executors/fail_safe_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/exporters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.502116 polygon-etl-0.3.6/polygonetl/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/export_all_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/export_blocks_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/export_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/export_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/export_receipts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/export_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/export_tokens_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/export_traces_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.502116 polygon-etl-0.3.6/polygonetl/jobs/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/exporters/blocks_and_transactions_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/exporters/contracts_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/exporters/geth_traces_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/exporters/receipts_and_logs_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/exporters/token_transfers_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/exporters/tokens_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/exporters/traces_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/extract_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/extract_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/extract_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/jobs/extract_tokens_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/json_rpc_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mainnet_daofork_state_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mainnet_genesis_alloc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.502116 polygon-etl-0.3.6/polygonetl/mappers/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/block_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/contract_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/geth_trace_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/receipt_log_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/receipt_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/token_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/token_transfer_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/trace_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/mappers/transaction_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.502116 polygon-etl-0.3.6/polygonetl/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/misc/retriable_value_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/progress_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.502116 polygon-etl-0.3.6/polygonetl/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/providers/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/providers/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/providers/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/providers/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.506116 polygon-etl-0.3.6/polygonetl/service/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/eth_contract_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/eth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/eth_special_trace_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/eth_token_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/graph_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/token_transfer_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/trace_id_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/service/trace_status_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.506116 polygon-etl-0.3.6/polygonetl/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/streaming/enrich.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/streaming/eth_item_id_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/streaming/eth_item_timestamp_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/streaming/eth_streamer_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/streaming/item_exporter_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/streaming/postgres_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/thread_local_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/polygonetl/web3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 10:01:58.506116 polygon-etl-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.494116 polygon-etl-0.3.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.506116 polygon-etl-0.3.6/tests/polygonetl/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.506116 polygon-etl-0.3.6/tests/polygonetl/job/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/mock_batch_web3_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/mock_web3_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_export_blocks_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_export_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_export_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_export_receipts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_export_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_export_tokens_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_export_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_extract_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_extract_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_extract_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/polygonetl/job/test_extract_tokens_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:01:58.506116 polygon-etl-0.3.6/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-15 10:01:50.000000 polygon-etl-0.3.6/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.092124 polygon-etl-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-29 10:21:54.092124 polygon-etl-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.080124 polygon-etl-0.3.7/polygon_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-29 10:21:54.000000 polygon-etl-0.3.7/polygon_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-29 10:21:54.000000 polygon-etl-0.3.7/polygon_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:21:54.000000 polygon-etl-0.3.7/polygon_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 10:21:54.000000 polygon-etl-0.3.7/polygon_etl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-29 10:21:54.000000 polygon-etl-0.3.7/polygon_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 10:21:54.000000 polygon-etl-0.3.7/polygon_etl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.080124 polygon-etl-0.3.7/polygonetl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/atomic_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.084124 polygon-etl-0.3.7/polygonetl/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/export_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/export_blocks_and_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/export_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/export_geth_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/export_receipts_and_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/export_token_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/export_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/export_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/extract_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/extract_csv_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/extract_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/extract_geth_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/extract_token_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/extract_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/filter_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/get_block_range_for_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/get_block_range_for_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/get_keccak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/cli/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/csv_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.084124 polygon-etl-0.3.7/polygonetl/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/domain/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/domain/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/domain/geth_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/domain/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/domain/receipt_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/domain/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/domain/token_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/domain/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/domain/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.084124 polygon-etl-0.3.7/polygonetl/enumeration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/enumeration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/enumeration/entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/erc20_abi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.084124 polygon-etl-0.3.7/polygonetl/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/executors/batch_work_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/executors/bounded_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/executors/fail_safe_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/exporters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.084124 polygon-etl-0.3.7/polygonetl/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/export_all_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/export_blocks_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/export_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/export_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/export_receipts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/export_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/export_tokens_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/export_traces_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.088124 polygon-etl-0.3.7/polygonetl/jobs/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/exporters/blocks_and_transactions_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/exporters/contracts_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/exporters/geth_traces_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/exporters/receipts_and_logs_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/exporters/token_transfers_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/exporters/tokens_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/exporters/traces_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/extract_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/extract_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/extract_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/jobs/extract_tokens_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/json_rpc_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/mainnet_daofork_state_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/mainnet_genesis_alloc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.088124 polygon-etl-0.3.7/polygonetl/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/mappers/block_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/mappers/contract_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/mappers/geth_trace_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/mappers/receipt_log_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/mappers/receipt_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/mappers/token_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/mappers/token_transfer_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/mappers/trace_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/mappers/transaction_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.088124 polygon-etl-0.3.7/polygonetl/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/misc/retriable_value_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/progress_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.088124 polygon-etl-0.3.7/polygonetl/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/providers/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/providers/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/providers/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/providers/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.088124 polygon-etl-0.3.7/polygonetl/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/service/eth_contract_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/service/eth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/service/eth_special_trace_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/service/eth_token_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/service/graph_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/service/token_transfer_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/service/trace_id_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/service/trace_status_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.088124 polygon-etl-0.3.7/polygonetl/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/streaming/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/streaming/eth_item_id_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/streaming/eth_item_timestamp_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/streaming/eth_streamer_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/streaming/item_exporter_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/streaming/postgres_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/thread_local_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/polygonetl/web3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 10:21:54.092124 polygon-etl-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.080124 polygon-etl-0.3.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.092124 polygon-etl-0.3.7/tests/polygonetl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/polygonetl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.092124 polygon-etl-0.3.7/tests/polygonetl/job/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/polygonetl/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/polygonetl/job/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/polygonetl/job/mock_batch_web3_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/polygonetl/job/mock_web3_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/polygonetl/job/test_export_blocks_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/polygonetl/job/test_export_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/polygonetl/job/test_export_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/polygonetl/job/test_export_receipts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/polygonetl/job/test_export_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/polygonetl/job/test_export_tokens_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/polygonetl/job/test_export_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/polygonetl/job/test_extract_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/polygonetl/job/test_extract_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/polygonetl/job/test_extract_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/polygonetl/job/test_extract_tokens_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:21:54.092124 polygon-etl-0.3.7/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-29 10:21:45.000000 polygon-etl-0.3.7/tests/resources/__init__.py
```

### Comparing `polygon-etl-0.3.6/PKG-INFO` & `polygon-etl-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polygon-etl
-Version: 0.3.6
+Version: 0.3.7
 Summary: Tools for exporting Polygon blockchain data to CSV or JSON
 Home-page: https://github.com/blockchain-etl/polygon-etl
 Author: Evgeny Medvedev
 Author-email: evge.medvedev@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/blockchain-etl/polygon-etl/issues
 Project-URL: Source, https://github.com/blockchain-etl/polygon-etl
```

### Comparing `polygon-etl-0.3.6/README.md` & `polygon-etl-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygon_etl.egg-info/PKG-INFO` & `polygon-etl-0.3.7/polygon_etl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polygon-etl
-Version: 0.3.6
+Version: 0.3.7
 Summary: Tools for exporting Polygon blockchain data to CSV or JSON
 Home-page: https://github.com/blockchain-etl/polygon-etl
 Author: Evgeny Medvedev
 Author-email: evge.medvedev@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/blockchain-etl/polygon-etl/issues
 Project-URL: Source, https://github.com/blockchain-etl/polygon-etl
```

### Comparing `polygon-etl-0.3.6/polygon_etl.egg-info/SOURCES.txt` & `polygon-etl-0.3.7/polygon_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/__init__.py` & `polygon-etl-0.3.7/polygonetl/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/__main__.py` & `polygon-etl-0.3.7/polygonetl/__main__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/atomic_counter.py` & `polygon-etl-0.3.7/polygonetl/atomic_counter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/__init__.py` & `polygon-etl-0.3.7/polygonetl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/export_all.py` & `polygon-etl-0.3.7/polygonetl/cli/export_all.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/export_blocks_and_transactions.py` & `polygon-etl-0.3.7/polygonetl/cli/export_blocks_and_transactions.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/export_contracts.py` & `polygon-etl-0.3.7/polygonetl/cli/export_contracts.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/export_geth_traces.py` & `polygon-etl-0.3.7/polygonetl/cli/export_geth_traces.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/export_receipts_and_logs.py` & `polygon-etl-0.3.7/polygonetl/cli/export_receipts_and_logs.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/export_token_transfers.py` & `polygon-etl-0.3.7/polygonetl/cli/export_token_transfers.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/export_tokens.py` & `polygon-etl-0.3.7/polygonetl/cli/export_tokens.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/export_traces.py` & `polygon-etl-0.3.7/polygonetl/cli/export_traces.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/extract_contracts.py` & `polygon-etl-0.3.7/polygonetl/cli/extract_contracts.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/extract_csv_column.py` & `polygon-etl-0.3.7/polygonetl/cli/extract_csv_column.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/extract_field.py` & `polygon-etl-0.3.7/polygonetl/cli/extract_field.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/extract_geth_traces.py` & `polygon-etl-0.3.7/polygonetl/cli/extract_geth_traces.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/extract_token_transfers.py` & `polygon-etl-0.3.7/polygonetl/cli/extract_token_transfers.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/extract_tokens.py` & `polygon-etl-0.3.7/polygonetl/cli/extract_tokens.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/filter_items.py` & `polygon-etl-0.3.7/polygonetl/cli/filter_items.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/get_block_range_for_date.py` & `polygon-etl-0.3.7/polygonetl/cli/get_block_range_for_date.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/get_block_range_for_timestamps.py` & `polygon-etl-0.3.7/polygonetl/cli/get_block_range_for_timestamps.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/get_keccak_hash.py` & `polygon-etl-0.3.7/polygonetl/cli/get_keccak_hash.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/cli/stream.py` & `polygon-etl-0.3.7/polygonetl/cli/stream.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/csv_utils.py` & `polygon-etl-0.3.7/polygonetl/csv_utils.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/domain/__init__.py` & `polygon-etl-0.3.7/polygonetl/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/domain/block.py` & `polygon-etl-0.3.7/polygonetl/domain/block.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/domain/contract.py` & `polygon-etl-0.3.7/polygonetl/domain/contract.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/domain/geth_trace.py` & `polygon-etl-0.3.7/polygonetl/domain/geth_trace.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/domain/receipt.py` & `polygon-etl-0.3.7/polygonetl/domain/receipt.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/domain/receipt_log.py` & `polygon-etl-0.3.7/polygonetl/domain/receipt_log.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/domain/token.py` & `polygon-etl-0.3.7/polygonetl/domain/token.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/domain/token_transfer.py` & `polygon-etl-0.3.7/polygonetl/domain/token_transfer.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/domain/trace.py` & `polygon-etl-0.3.7/polygonetl/domain/trace.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/domain/transaction.py` & `polygon-etl-0.3.7/polygonetl/domain/transaction.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/erc20_abi.py` & `polygon-etl-0.3.7/polygonetl/erc20_abi.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/executors/__init__.py` & `polygon-etl-0.3.7/polygonetl/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/executors/batch_work_executor.py` & `polygon-etl-0.3.7/polygonetl/executors/batch_work_executor.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/executors/bounded_executor.py` & `polygon-etl-0.3.7/polygonetl/executors/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/executors/fail_safe_executor.py` & `polygon-etl-0.3.7/polygonetl/executors/fail_safe_executor.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/exporters.py` & `polygon-etl-0.3.7/polygonetl/exporters.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/__init__.py` & `polygon-etl-0.3.7/polygonetl/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/export_all_common.py` & `polygon-etl-0.3.7/polygonetl/jobs/export_all_common.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/export_blocks_job.py` & `polygon-etl-0.3.7/polygonetl/jobs/export_blocks_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/export_contracts_job.py` & `polygon-etl-0.3.7/polygonetl/jobs/export_contracts_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/export_geth_traces_job.py` & `polygon-etl-0.3.7/polygonetl/jobs/export_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/export_receipts_job.py` & `polygon-etl-0.3.7/polygonetl/jobs/export_receipts_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/export_token_transfers_job.py` & `polygon-etl-0.3.7/polygonetl/jobs/export_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/export_tokens_job.py` & `polygon-etl-0.3.7/polygonetl/jobs/export_tokens_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/export_traces_job.py` & `polygon-etl-0.3.7/polygonetl/jobs/export_traces_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/exporters/__init__.py` & `polygon-etl-0.3.7/polygonetl/jobs/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/exporters/blocks_and_transactions_item_exporter.py` & `polygon-etl-0.3.7/polygonetl/jobs/exporters/blocks_and_transactions_item_exporter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/exporters/contracts_item_exporter.py` & `polygon-etl-0.3.7/polygonetl/jobs/exporters/contracts_item_exporter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/exporters/geth_traces_item_exporter.py` & `polygon-etl-0.3.7/polygonetl/jobs/exporters/geth_traces_item_exporter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/exporters/receipts_and_logs_item_exporter.py` & `polygon-etl-0.3.7/polygonetl/jobs/exporters/receipts_and_logs_item_exporter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/exporters/token_transfers_item_exporter.py` & `polygon-etl-0.3.7/polygonetl/jobs/exporters/token_transfers_item_exporter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/exporters/tokens_item_exporter.py` & `polygon-etl-0.3.7/polygonetl/jobs/exporters/tokens_item_exporter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/exporters/traces_item_exporter.py` & `polygon-etl-0.3.7/polygonetl/jobs/exporters/traces_item_exporter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/extract_contracts_job.py` & `polygon-etl-0.3.7/polygonetl/jobs/extract_contracts_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/extract_geth_traces_job.py` & `polygon-etl-0.3.7/polygonetl/jobs/extract_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/extract_token_transfers_job.py` & `polygon-etl-0.3.7/polygonetl/jobs/extract_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/jobs/extract_tokens_job.py` & `polygon-etl-0.3.7/polygonetl/jobs/extract_tokens_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/json_rpc_requests.py` & `polygon-etl-0.3.7/polygonetl/json_rpc_requests.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/mainnet_daofork_state_changes.py` & `polygon-etl-0.3.7/polygonetl/mainnet_daofork_state_changes.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/mainnet_genesis_alloc.py` & `polygon-etl-0.3.7/polygonetl/mainnet_genesis_alloc.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/mappers/__init__.py` & `polygon-etl-0.3.7/polygonetl/mappers/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/mappers/block_mapper.py` & `polygon-etl-0.3.7/polygonetl/mappers/block_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/mappers/contract_mapper.py` & `polygon-etl-0.3.7/polygonetl/mappers/contract_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/mappers/geth_trace_mapper.py` & `polygon-etl-0.3.7/polygonetl/mappers/geth_trace_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/mappers/receipt_log_mapper.py` & `polygon-etl-0.3.7/polygonetl/mappers/receipt_log_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/mappers/receipt_mapper.py` & `polygon-etl-0.3.7/polygonetl/mappers/receipt_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/mappers/token_mapper.py` & `polygon-etl-0.3.7/polygonetl/mappers/token_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/mappers/token_transfer_mapper.py` & `polygon-etl-0.3.7/polygonetl/mappers/token_transfer_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/mappers/trace_mapper.py` & `polygon-etl-0.3.7/polygonetl/mappers/trace_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/mappers/transaction_mapper.py` & `polygon-etl-0.3.7/polygonetl/mappers/transaction_mapper.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/misc/__init__.py` & `polygon-etl-0.3.7/polygonetl/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/misc_utils.py` & `polygon-etl-0.3.7/polygonetl/misc_utils.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/progress_logger.py` & `polygon-etl-0.3.7/polygonetl/progress_logger.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/providers/__init__.py` & `polygon-etl-0.3.7/polygonetl/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/providers/auto.py` & `polygon-etl-0.3.7/polygonetl/providers/auto.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/providers/ipc.py` & `polygon-etl-0.3.7/polygonetl/providers/ipc.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/providers/request.py` & `polygon-etl-0.3.7/polygonetl/providers/request.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/providers/rpc.py` & `polygon-etl-0.3.7/polygonetl/providers/rpc.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/service/__init__.py` & `polygon-etl-0.3.7/polygonetl/service/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/service/eth_contract_service.py` & `polygon-etl-0.3.7/polygonetl/service/eth_contract_service.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/service/eth_service.py` & `polygon-etl-0.3.7/polygonetl/service/eth_service.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/service/eth_special_trace_service.py` & `polygon-etl-0.3.7/polygonetl/service/eth_special_trace_service.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/service/eth_token_service.py` & `polygon-etl-0.3.7/polygonetl/service/eth_token_service.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/service/graph_operations.py` & `polygon-etl-0.3.7/polygonetl/service/graph_operations.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/service/token_transfer_extractor.py` & `polygon-etl-0.3.7/polygonetl/service/token_transfer_extractor.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/service/trace_id_calculator.py` & `polygon-etl-0.3.7/polygonetl/service/trace_id_calculator.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/service/trace_status_calculator.py` & `polygon-etl-0.3.7/polygonetl/service/trace_status_calculator.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/streaming/__init__.py` & `polygon-etl-0.3.7/polygonetl/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/streaming/enrich.py` & `polygon-etl-0.3.7/polygonetl/streaming/enrich.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/streaming/eth_item_id_calculator.py` & `polygon-etl-0.3.7/polygonetl/streaming/eth_item_id_calculator.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/streaming/eth_item_timestamp_calculator.py` & `polygon-etl-0.3.7/polygonetl/streaming/eth_item_timestamp_calculator.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/streaming/eth_streamer_adapter.py` & `polygon-etl-0.3.7/polygonetl/streaming/eth_streamer_adapter.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/streaming/item_exporter_creator.py` & `polygon-etl-0.3.7/polygonetl/streaming/item_exporter_creator.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/streaming/postgres_tables.py` & `polygon-etl-0.3.7/polygonetl/streaming/postgres_tables.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/thread_local_proxy.py` & `polygon-etl-0.3.7/polygonetl/thread_local_proxy.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/utils.py` & `polygon-etl-0.3.7/polygonetl/utils.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/polygonetl/web3_utils.py` & `polygon-etl-0.3.7/polygonetl/web3_utils.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/setup.py` & `polygon-etl-0.3.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 long_description = read("README.md") if os.path.isfile("README.md") else ""
 
 setup(
     name="polygon-etl",
-    version="0.3.6",
+    version="0.3.7",
     author="Evgeny Medvedev",
     author_email="evge.medvedev@gmail.com",
     description="Tools for exporting Polygon blockchain data to CSV or JSON",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/blockchain-etl/polygon-etl",
     packages=find_packages(exclude=["schemas", "tests"]),
```

### Comparing `polygon-etl-0.3.6/tests/polygonetl/__init__.py` & `polygon-etl-0.3.7/tests/polygonetl/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/tests/polygonetl/job/__init__.py` & `polygon-etl-0.3.7/tests/polygonetl/job/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/tests/polygonetl/job/helpers.py` & `polygon-etl-0.3.7/tests/polygonetl/job/helpers.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/tests/polygonetl/job/mock_batch_web3_provider.py` & `polygon-etl-0.3.7/tests/polygonetl/job/mock_batch_web3_provider.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/tests/polygonetl/job/mock_web3_provider.py` & `polygon-etl-0.3.7/tests/polygonetl/job/mock_web3_provider.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/tests/polygonetl/job/test_export_blocks_job.py` & `polygon-etl-0.3.7/tests/polygonetl/job/test_export_blocks_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/tests/polygonetl/job/test_export_contracts_job.py` & `polygon-etl-0.3.7/tests/polygonetl/job/test_export_contracts_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/tests/polygonetl/job/test_export_geth_traces_job.py` & `polygon-etl-0.3.7/tests/polygonetl/job/test_export_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/tests/polygonetl/job/test_export_receipts_job.py` & `polygon-etl-0.3.7/tests/polygonetl/job/test_export_receipts_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/tests/polygonetl/job/test_export_token_transfers_job.py` & `polygon-etl-0.3.7/tests/polygonetl/job/test_export_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/tests/polygonetl/job/test_export_tokens_job.py` & `polygon-etl-0.3.7/tests/polygonetl/job/test_export_tokens_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/tests/polygonetl/job/test_export_traces_job.py` & `polygon-etl-0.3.7/tests/polygonetl/job/test_export_traces_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/tests/polygonetl/job/test_extract_contracts_job.py` & `polygon-etl-0.3.7/tests/polygonetl/job/test_extract_contracts_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/tests/polygonetl/job/test_extract_geth_traces_job.py` & `polygon-etl-0.3.7/tests/polygonetl/job/test_extract_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/tests/polygonetl/job/test_extract_token_transfers_job.py` & `polygon-etl-0.3.7/tests/polygonetl/job/test_extract_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/tests/polygonetl/job/test_extract_tokens_job.py` & `polygon-etl-0.3.7/tests/polygonetl/job/test_extract_tokens_job.py`

 * *Files identical despite different names*

### Comparing `polygon-etl-0.3.6/tests/resources/__init__.py` & `polygon-etl-0.3.7/tests/resources/__init__.py`

 * *Files identical despite different names*

