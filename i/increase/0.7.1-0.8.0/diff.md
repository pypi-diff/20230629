# Comparing `tmp/increase-0.7.1.tar.gz` & `tmp/increase-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "increase-0.7.1.tar", max compression
+gzip compressed data, was "increase-0.8.0.tar", max compression
```

## Comparing `increase-0.7.1.tar` & `increase-0.8.0.tar`

### file list

```diff
@@ -1,210 +1,210 @@
--rw-r--r--   0        0        0    11338 2023-06-19 20:19:01.358159 increase-0.7.1/LICENSE
--rw-r--r--   0        0        0     8425 2023-06-19 20:19:01.358159 increase-0.7.1/README.md
--rw-r--r--   0        0        0     1883 2023-06-19 20:19:01.358159 increase-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     2587 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/__init__.py
--rw-r--r--   0        0        0    46808 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_base_client.py
--rw-r--r--   0        0        0     3889 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_base_exceptions.py
--rw-r--r--   0        0        0    26762 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_client.py
--rw-r--r--   0        0        0    10875 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_exceptions.py
--rw-r--r--   0        0        0     7343 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_models.py
--rw-r--r--   0        0        0     4846 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_qs.py
--rw-r--r--   0        0        0      890 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_resource.py
--rw-r--r--   0        0        0     5884 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_streaming.py
--rw-r--r--   0        0        0     4229 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_types.py
--rw-r--r--   0        0        0     1277 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_utils/__init__.py
--rw-r--r--   0        0        0     6710 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_utils/_transform.py
--rw-r--r--   0        0        0     9411 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_utils/_utils.py
--rw-r--r--   0        0        0      127 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_version.py
--rw-r--r--   0        0        0     1109 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/pagination.py
--rw-r--r--   0        0        0        0 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/py.typed
--rw-r--r--   0        0        0     4478 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/resources/__init__.py
--rw-r--r--   0        0        0    15065 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/account_numbers.py
--rw-r--r--   0        0        0     7400 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/account_statements.py
--rw-r--r--   0        0        0    18102 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/account_transfers.py
--rw-r--r--   0        0        0    18476 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/accounts.py
--rw-r--r--   0        0        0    15600 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/ach_prenotifications.py
--rw-r--r--   0        0        0    26071 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/ach_transfers.py
--rw-r--r--   0        0        0     4285 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/balance_lookups.py
--rw-r--r--   0        0        0     8651 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/bookkeeping_accounts.py
--rw-r--r--   0        0        0     4122 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/bookkeeping_entries.py
--rw-r--r--   0        0        0     4842 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/bookkeeping_entry_sets.py
--rw-r--r--   0        0        0    10707 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/card_disputes.py
--rw-r--r--   0        0        0    10597 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/card_profiles.py
--rw-r--r--   0        0        0    19120 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/cards.py
--rw-r--r--   0        0        0    11757 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/check_deposits.py
--rw-r--r--   0        0        0    23188 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/check_transfers.py
--rw-r--r--   0        0        0     7771 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/declined_transactions.py
--rw-r--r--   0        0        0     7353 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/digital_wallet_tokens.py
--rw-r--r--   0        0        0     7177 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/documents.py
--rw-r--r--   0        0        0      282 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/entities/__init__.py
--rw-r--r--   0        0        0    14010 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/entities/entities.py
--rw-r--r--   0        0        0     8071 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/entities/supplemental_documents.py
--rw-r--r--   0        0        0    18799 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/event_subscriptions.py
--rw-r--r--   0        0        0     7154 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/events.py
--rw-r--r--   0        0        0    10548 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/exports.py
--rw-r--r--   0        0        0    15315 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/external_accounts.py
--rw-r--r--   0        0        0    12781 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/files.py
--rw-r--r--   0        0        0     2040 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/groups.py
--rw-r--r--   0        0        0    12035 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/inbound_ach_transfer_returns.py
--rw-r--r--   0        0        0     7075 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/inbound_wire_drawdown_requests.py
--rw-r--r--   0        0        0    14231 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/limits.py
--rw-r--r--   0        0        0     6593 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/oauth_connections.py
--rw-r--r--   0        0        0     8344 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/pending_transactions.py
--rw-r--r--   0        0        0     6300 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/programs.py
--rw-r--r--   0        0        0     8536 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/real_time_decisions.py
--rw-r--r--   0        0        0    14968 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/real_time_payments_transfers.py
--rw-r--r--   0        0        0     4951 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/routing_numbers.py
--rw-r--r--   0        0        0     1989 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/__init__.py
--rw-r--r--   0        0        0     4026 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/account_statements.py
--rw-r--r--   0        0        0     4024 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/account_transfers.py
--rw-r--r--   0        0        0    21913 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/ach_transfers.py
--rw-r--r--   0        0        0     5051 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/card_disputes.py
--rw-r--r--   0        0        0     3967 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/card_refunds.py
--rw-r--r--   0        0        0    11463 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/cards.py
--rw-r--r--   0        0        0    10125 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/check_deposits.py
--rw-r--r--   0        0        0    11013 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/check_transfers.py
--rw-r--r--   0        0        0     4085 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/digital_wallet_token_requests.py
--rw-r--r--   0        0        0     3639 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/documents.py
--rw-r--r--   0        0        0    13466 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/inbound_wire_drawdown_requests.py
--rw-r--r--   0        0        0     4411 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/interest_payments.py
--rw-r--r--   0        0        0     3919 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/programs.py
--rw-r--r--   0        0        0    11257 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/real_time_payments_transfers.py
--rw-r--r--   0        0        0     4588 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/simulations.py
--rw-r--r--   0        0        0    12351 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/wire_transfers.py
--rw-r--r--   0        0        0     7800 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/transactions.py
--rw-r--r--   0        0        0    13338 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/wire_drawdown_requests.py
--rw-r--r--   0        0        0    27583 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/wire_transfers.py
--rw-r--r--   0        0        0     8739 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/__init__.py
--rw-r--r--   0        0        0     1666 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account.py
--rw-r--r--   0        0        0      747 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_create_params.py
--rw-r--r--   0        0        0     1693 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_list_params.py
--rw-r--r--   0        0        0     1026 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_number.py
--rw-r--r--   0        0        0      408 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_number_create_params.py
--rw-r--r--   0        0        0     1598 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_number_list_params.py
--rw-r--r--   0        0        0      435 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_number_update_params.py
--rw-r--r--   0        0        0     1347 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_statement.py
--rw-r--r--   0        0        0     1534 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_statement_list_params.py
--rw-r--r--   0        0        0     2648 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_transfer.py
--rw-r--r--   0        0        0      814 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_transfer_create_params.py
--rw-r--r--   0        0        0     1494 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_transfer_list_params.py
--rw-r--r--   0        0        0      271 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_update_params.py
--rw-r--r--   0        0        0     2152 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/ach_prenotification.py
--rw-r--r--   0        0        0     1847 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/ach_prenotification_create_params.py
--rw-r--r--   0        0        0     1391 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/ach_prenotification_list_params.py
--rw-r--r--   0        0        0     8899 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/ach_transfer.py
--rw-r--r--   0        0        0     3388 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/ach_transfer_create_params.py
--rw-r--r--   0        0        0     1592 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/ach_transfer_list_params.py
--rw-r--r--   0        0        0      585 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/balance_lookup_lookup_params.py
--rw-r--r--   0        0        0      780 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/balance_lookup_lookup_response.py
--rw-r--r--   0        0        0      823 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/bookkeeping_account.py
--rw-r--r--   0        0        0      626 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/bookkeeping_account_create_params.py
--rw-r--r--   0        0        0      428 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/bookkeeping_account_list_params.py
--rw-r--r--   0        0        0      698 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/bookkeeping_entry.py
--rw-r--r--   0        0        0      424 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/bookkeeping_entry_list_params.py
--rw-r--r--   0        0        0      895 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/bookkeeping_entry_set.py
--rw-r--r--   0        0        0     1133 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/bookkeeping_entry_set_create_params.py
--rw-r--r--   0        0        0     2342 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card.py
--rw-r--r--   0        0        0     1767 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_create_params.py
--rw-r--r--   0        0        0      907 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_details.py
--rw-r--r--   0        0        0     2011 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_dispute.py
--rw-r--r--   0        0        0      483 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_dispute_create_params.py
--rw-r--r--   0        0        0     1661 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_dispute_list_params.py
--rw-r--r--   0        0        0     1451 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_list_params.py
--rw-r--r--   0        0        0     2186 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_profile.py
--rw-r--r--   0        0        0     1820 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_profile_create_params.py
--rw-r--r--   0        0        0      716 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_profile_list_params.py
--rw-r--r--   0        0        0     1619 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_update_params.py
--rw-r--r--   0        0        0     4894 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/check_deposit.py
--rw-r--r--   0        0        0      748 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/check_deposit_create_params.py
--rw-r--r--   0        0        0     1477 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/check_deposit_list_params.py
--rw-r--r--   0        0        0     6647 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/check_transfer.py
--rw-r--r--   0        0        0     1939 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/check_transfer_create_params.py
--rw-r--r--   0        0        0     1488 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/check_transfer_list_params.py
--rw-r--r--   0        0        0    13068 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/declined_transaction.py
--rw-r--r--   0        0        0     1598 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/declined_transaction_list_params.py
--rw-r--r--   0        0        0      950 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/digital_wallet_token.py
--rw-r--r--   0        0        0     1489 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/digital_wallet_token_list_params.py
--rw-r--r--   0        0        0     2581 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/document.py
--rw-r--r--   0        0        0     3900 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/document_list_params.py
--rw-r--r--   0        0        0      418 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/entities/__init__.py
--rw-r--r--   0        0        0      634 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/entities/supplemental_document.py
--rw-r--r--   0        0        0      343 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/entities/supplemental_document_create_params.py
--rw-r--r--   0        0        0      547 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/entities/supplemental_document_list_params.py
--rw-r--r--   0        0        0    11893 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/entity.py
--rw-r--r--   0        0        0    25685 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/entity_create_params.py
--rw-r--r--   0        0        0     1367 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/entity_list_params.py
--rw-r--r--   0        0        0     2724 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/event.py
--rw-r--r--   0        0        0     4044 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/event_list_params.py
--rw-r--r--   0        0        0     3124 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/event_subscription.py
--rw-r--r--   0        0        0     2526 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/event_subscription_create_params.py
--rw-r--r--   0        0        0      426 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/event_subscription_list_params.py
--rw-r--r--   0        0        0      360 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/event_subscription_update_params.py
--rw-r--r--   0        0        0     1147 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/export.py
--rw-r--r--   0        0        0     2946 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/export_create_params.py
--rw-r--r--   0        0        0      404 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/export_list_params.py
--rw-r--r--   0        0        0     1205 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/external_account.py
--rw-r--r--   0        0        0      706 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/external_account_create_params.py
--rw-r--r--   0        0        0      701 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/external_account_list_params.py
--rw-r--r--   0        0        0      420 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/external_account_update_params.py
--rw-r--r--   0        0        0     1546 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/file.py
--rw-r--r--   0        0        0     1041 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/file_create_params.py
--rw-r--r--   0        0        0     2120 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/file_list_params.py
--rw-r--r--   0        0        0      738 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/group.py
--rw-r--r--   0        0        0     1693 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/inbound_ach_transfer_return.py
--rw-r--r--   0        0        0     1109 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/inbound_ach_transfer_return_create_params.py
--rw-r--r--   0        0        0      440 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/inbound_ach_transfer_return_list_params.py
--rw-r--r--   0        0        0     2916 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/inbound_wire_drawdown_request.py
--rw-r--r--   0        0        0      444 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/inbound_wire_drawdown_request_list_params.py
--rw-r--r--   0        0        0     1041 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/limit.py
--rw-r--r--   0        0        0      696 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/limit_create_params.py
--rw-r--r--   0        0        0      527 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/limit_list_params.py
--rw-r--r--   0        0        0      332 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/limit_update_params.py
--rw-r--r--   0        0        0      779 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/oauth_connection.py
--rw-r--r--   0        0        0      422 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/oauth_connection_list_params.py
--rw-r--r--   0        0        0    12078 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/pending_transaction.py
--rw-r--r--   0        0        0     1956 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/pending_transaction_list_params.py
--rw-r--r--   0        0        0      735 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/program.py
--rw-r--r--   0        0        0      406 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/program_list_params.py
--rw-r--r--   0        0        0     6113 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/real_time_decision.py
--rw-r--r--   0        0        0     2451 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/real_time_decision_action_params.py
--rw-r--r--   0        0        0     5096 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/real_time_payments_transfer.py
--rw-r--r--   0        0        0     1283 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/real_time_payments_transfer_create_params.py
--rw-r--r--   0        0        0     1664 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/real_time_payments_transfer_list_params.py
--rw-r--r--   0        0        0      895 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/routing_number.py
--rw-r--r--   0        0        0      522 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/routing_number_list_params.py
--rw-r--r--   0        0        0      155 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/shared/__init__.py
--rw-r--r--   0        0        0      489 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/shared/point_of_service_entry_mode.py
--rw-r--r--   0        0        0      155 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/shared_params/__init__.py
--rw-r--r--   0        0        0      525 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/shared_params/point_of_service_entry_mode.py
--rw-r--r--   0        0        0     2608 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/__init__.py
--rw-r--r--   0        0        0      338 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/account_statement_create_params.py
--rw-r--r--   0        0        0     1027 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/ach_transfer_create_inbound_params.py
--rw-r--r--   0        0        0     3320 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/ach_transfer_return_params.py
--rw-r--r--   0        0        0    50512 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/ach_transfer_simulation.py
--rw-r--r--   0        0        0    26885 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/card_authorization_simulation.py
--rw-r--r--   0        0        0      823 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/card_authorize_params.py
--rw-r--r--   0        0        0      443 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/card_dispute_action_params.py
--rw-r--r--   0        0        0      400 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/card_refund_create_params.py
--rw-r--r--   0        0        0      610 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/card_settlement_params.py
--rw-r--r--   0        0        0      425 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/check_transfer_return_params.py
--rw-r--r--   0        0        0      346 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/digital_wallet_token_request_create_params.py
--rw-r--r--   0        0        0      953 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/digital_wallet_token_request_create_response.py
--rw-r--r--   0        0        0      325 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/document_create_params.py
--rw-r--r--   0        0        0    50683 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py
--rw-r--r--   0        0        0     2648 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py
--rw-r--r--   0        0        0      435 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/interest_payment_create_params.py
--rw-r--r--   0        0        0    36778 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/interest_payment_simulation_result.py
--rw-r--r--   0        0        0      299 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/program_create_params.py
--rw-r--r--   0        0        0     1362 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/real_time_payments_transfer_complete_params.py
--rw-r--r--   0        0        0     1020 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py
--rw-r--r--   0        0        0     2591 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/wire_transfer_create_inbound_params.py
--rw-r--r--   0        0        0    36822 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/wire_transfer_simulation.py
--rw-r--r--   0        0        0    35302 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/transaction.py
--rw-r--r--   0        0        0     3251 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/transaction_list_params.py
--rw-r--r--   0        0        0     2239 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/wire_drawdown_request.py
--rw-r--r--   0        0        0     1148 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/wire_drawdown_request_create_params.py
--rw-r--r--   0        0        0      430 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/wire_drawdown_request_list_params.py
--rw-r--r--   0        0        0     5343 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/wire_transfer.py
--rw-r--r--   0        0        0     1367 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/wire_transfer_create_params.py
--rw-r--r--   0        0        0     1588 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/wire_transfer_list_params.py
--rw-r--r--   0        0        0     9328 1970-01-01 00:00:00.000000 increase-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-06-29 12:24:52.608649 increase-0.8.0/LICENSE
+-rw-r--r--   0        0        0     8418 2023-06-29 12:24:52.608649 increase-0.8.0/README.md
+-rw-r--r--   0        0        0     1883 2023-06-29 12:24:52.608649 increase-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2587 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/__init__.py
+-rw-r--r--   0        0        0    46808 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_base_exceptions.py
+-rw-r--r--   0        0        0    26762 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_client.py
+-rw-r--r--   0        0        0    10875 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_exceptions.py
+-rw-r--r--   0        0        0     7343 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_models.py
+-rw-r--r--   0        0        0     4846 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_qs.py
+-rw-r--r--   0        0        0      890 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_resource.py
+-rw-r--r--   0        0        0     5884 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_streaming.py
+-rw-r--r--   0        0        0     4229 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_types.py
+-rw-r--r--   0        0        0     1277 2023-06-29 12:24:52.608649 increase-0.8.0/src/increase/_utils/__init__.py
+-rw-r--r--   0        0        0     6710 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/_utils/_transform.py
+-rw-r--r--   0        0        0     9411 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/_utils/_utils.py
+-rw-r--r--   0        0        0      127 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/_version.py
+-rw-r--r--   0        0        0     1109 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/pagination.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/py.typed
+-rw-r--r--   0        0        0     4478 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/__init__.py
+-rw-r--r--   0        0        0    15065 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/account_numbers.py
+-rw-r--r--   0        0        0     7400 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/account_statements.py
+-rw-r--r--   0        0        0    18102 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/account_transfers.py
+-rw-r--r--   0        0        0    18476 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/accounts.py
+-rw-r--r--   0        0        0    15600 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/ach_prenotifications.py
+-rw-r--r--   0        0        0    26071 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/ach_transfers.py
+-rw-r--r--   0        0        0     4285 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/balance_lookups.py
+-rw-r--r--   0        0        0     8651 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/bookkeeping_accounts.py
+-rw-r--r--   0        0        0     4122 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/bookkeeping_entries.py
+-rw-r--r--   0        0        0     4842 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/bookkeeping_entry_sets.py
+-rw-r--r--   0        0        0    10707 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/card_disputes.py
+-rw-r--r--   0        0        0    10597 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/card_profiles.py
+-rw-r--r--   0        0        0    19120 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/cards.py
+-rw-r--r--   0        0        0    11757 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/check_deposits.py
+-rw-r--r--   0        0        0    23188 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/check_transfers.py
+-rw-r--r--   0        0        0     7771 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/declined_transactions.py
+-rw-r--r--   0        0        0     7353 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/digital_wallet_tokens.py
+-rw-r--r--   0        0        0     7177 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/documents.py
+-rw-r--r--   0        0        0      282 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/entities/__init__.py
+-rw-r--r--   0        0        0    14010 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/entities/entities.py
+-rw-r--r--   0        0        0     8071 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/entities/supplemental_documents.py
+-rw-r--r--   0        0        0    18799 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/event_subscriptions.py
+-rw-r--r--   0        0        0     7154 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/events.py
+-rw-r--r--   0        0        0    10548 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/exports.py
+-rw-r--r--   0        0        0    15315 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/external_accounts.py
+-rw-r--r--   0        0        0    12929 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/files.py
+-rw-r--r--   0        0        0     2040 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/groups.py
+-rw-r--r--   0        0        0    12035 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/inbound_ach_transfer_returns.py
+-rw-r--r--   0        0        0     7075 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/inbound_wire_drawdown_requests.py
+-rw-r--r--   0        0        0    14231 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/limits.py
+-rw-r--r--   0        0        0     6593 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/oauth_connections.py
+-rw-r--r--   0        0        0     8344 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/pending_transactions.py
+-rw-r--r--   0        0        0     6300 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/programs.py
+-rw-r--r--   0        0        0     8536 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/real_time_decisions.py
+-rw-r--r--   0        0        0    14968 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/real_time_payments_transfers.py
+-rw-r--r--   0        0        0     4951 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/routing_numbers.py
+-rw-r--r--   0        0        0     1989 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/__init__.py
+-rw-r--r--   0        0        0     4026 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/account_statements.py
+-rw-r--r--   0        0        0     4024 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/account_transfers.py
+-rw-r--r--   0        0        0    21871 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/ach_transfers.py
+-rw-r--r--   0        0        0     5051 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/card_disputes.py
+-rw-r--r--   0        0        0     3967 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/card_refunds.py
+-rw-r--r--   0        0        0    11463 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/cards.py
+-rw-r--r--   0        0        0    10125 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/check_deposits.py
+-rw-r--r--   0        0        0    11013 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/check_transfers.py
+-rw-r--r--   0        0        0     4085 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/digital_wallet_token_requests.py
+-rw-r--r--   0        0        0     3639 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/documents.py
+-rw-r--r--   0        0        0    13466 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/inbound_wire_drawdown_requests.py
+-rw-r--r--   0        0        0     4411 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/interest_payments.py
+-rw-r--r--   0        0        0     3919 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/programs.py
+-rw-r--r--   0        0        0    11257 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/real_time_payments_transfers.py
+-rw-r--r--   0        0        0     4588 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/simulations.py
+-rw-r--r--   0        0        0    12351 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/simulations/wire_transfers.py
+-rw-r--r--   0        0        0     7800 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/transactions.py
+-rw-r--r--   0        0        0    13338 2023-06-29 12:24:52.612649 increase-0.8.0/src/increase/resources/wire_drawdown_requests.py
+-rw-r--r--   0        0        0    27583 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/resources/wire_transfers.py
+-rw-r--r--   0        0        0     8739 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/__init__.py
+-rw-r--r--   0        0        0     1666 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account.py
+-rw-r--r--   0        0        0      747 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_create_params.py
+-rw-r--r--   0        0        0     1693 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_list_params.py
+-rw-r--r--   0        0        0     1026 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_number.py
+-rw-r--r--   0        0        0      408 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_number_create_params.py
+-rw-r--r--   0        0        0     1598 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_number_list_params.py
+-rw-r--r--   0        0        0      435 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_number_update_params.py
+-rw-r--r--   0        0        0     1347 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_statement.py
+-rw-r--r--   0        0        0     1534 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_statement_list_params.py
+-rw-r--r--   0        0        0     2648 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_transfer.py
+-rw-r--r--   0        0        0      814 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_transfer_create_params.py
+-rw-r--r--   0        0        0     1494 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_transfer_list_params.py
+-rw-r--r--   0        0        0      271 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/account_update_params.py
+-rw-r--r--   0        0        0     2152 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/ach_prenotification.py
+-rw-r--r--   0        0        0     1847 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/ach_prenotification_create_params.py
+-rw-r--r--   0        0        0     1391 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/ach_prenotification_list_params.py
+-rw-r--r--   0        0        0     8882 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/ach_transfer.py
+-rw-r--r--   0        0        0     3388 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/ach_transfer_create_params.py
+-rw-r--r--   0        0        0     1592 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/ach_transfer_list_params.py
+-rw-r--r--   0        0        0      585 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/balance_lookup_lookup_params.py
+-rw-r--r--   0        0        0      780 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/balance_lookup_lookup_response.py
+-rw-r--r--   0        0        0      823 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/bookkeeping_account.py
+-rw-r--r--   0        0        0      626 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/bookkeeping_account_create_params.py
+-rw-r--r--   0        0        0      428 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/bookkeeping_account_list_params.py
+-rw-r--r--   0        0        0      698 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/bookkeeping_entry.py
+-rw-r--r--   0        0        0      424 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/bookkeeping_entry_list_params.py
+-rw-r--r--   0        0        0      895 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/bookkeeping_entry_set.py
+-rw-r--r--   0        0        0     1133 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/bookkeeping_entry_set_create_params.py
+-rw-r--r--   0        0        0     2342 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card.py
+-rw-r--r--   0        0        0     1767 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_create_params.py
+-rw-r--r--   0        0        0      907 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_details.py
+-rw-r--r--   0        0        0     2011 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_dispute.py
+-rw-r--r--   0        0        0      483 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_dispute_create_params.py
+-rw-r--r--   0        0        0     1661 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_dispute_list_params.py
+-rw-r--r--   0        0        0     1451 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_list_params.py
+-rw-r--r--   0        0        0     2186 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_profile.py
+-rw-r--r--   0        0        0     1820 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_profile_create_params.py
+-rw-r--r--   0        0        0      716 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_profile_list_params.py
+-rw-r--r--   0        0        0     1611 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/card_update_params.py
+-rw-r--r--   0        0        0     4894 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/check_deposit.py
+-rw-r--r--   0        0        0      748 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/check_deposit_create_params.py
+-rw-r--r--   0        0        0     1477 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/check_deposit_list_params.py
+-rw-r--r--   0        0        0     6750 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/check_transfer.py
+-rw-r--r--   0        0        0     1939 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/check_transfer_create_params.py
+-rw-r--r--   0        0        0     1488 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/check_transfer_list_params.py
+-rw-r--r--   0        0        0    13068 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/declined_transaction.py
+-rw-r--r--   0        0        0     1598 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/declined_transaction_list_params.py
+-rw-r--r--   0        0        0      950 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/digital_wallet_token.py
+-rw-r--r--   0        0        0     1489 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/digital_wallet_token_list_params.py
+-rw-r--r--   0        0        0      883 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/document.py
+-rw-r--r--   0        0        0     1780 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/document_list_params.py
+-rw-r--r--   0        0        0      418 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/entities/__init__.py
+-rw-r--r--   0        0        0      634 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/entities/supplemental_document.py
+-rw-r--r--   0        0        0      343 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/entities/supplemental_document_create_params.py
+-rw-r--r--   0        0        0      547 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/entities/supplemental_document_list_params.py
+-rw-r--r--   0        0        0    11893 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/entity.py
+-rw-r--r--   0        0        0    25685 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/entity_create_params.py
+-rw-r--r--   0        0        0     1367 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/entity_list_params.py
+-rw-r--r--   0        0        0     2724 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/event.py
+-rw-r--r--   0        0        0     4044 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/event_list_params.py
+-rw-r--r--   0        0        0     3124 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/event_subscription.py
+-rw-r--r--   0        0        0     2526 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/event_subscription_create_params.py
+-rw-r--r--   0        0        0      426 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/event_subscription_list_params.py
+-rw-r--r--   0        0        0      360 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/event_subscription_update_params.py
+-rw-r--r--   0        0        0     1147 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/export.py
+-rw-r--r--   0        0        0     2946 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/export_create_params.py
+-rw-r--r--   0        0        0      404 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/export_list_params.py
+-rw-r--r--   0        0        0     1205 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/external_account.py
+-rw-r--r--   0        0        0      706 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/external_account_create_params.py
+-rw-r--r--   0        0        0      701 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/external_account_list_params.py
+-rw-r--r--   0        0        0      420 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/external_account_update_params.py
+-rw-r--r--   0        0        0     1612 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/file.py
+-rw-r--r--   0        0        0     1115 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/file_create_params.py
+-rw-r--r--   0        0        0     2202 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/file_list_params.py
+-rw-r--r--   0        0        0      738 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/group.py
+-rw-r--r--   0        0        0     1693 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/inbound_ach_transfer_return.py
+-rw-r--r--   0        0        0     1109 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/inbound_ach_transfer_return_create_params.py
+-rw-r--r--   0        0        0      440 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/inbound_ach_transfer_return_list_params.py
+-rw-r--r--   0        0        0     2916 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/inbound_wire_drawdown_request.py
+-rw-r--r--   0        0        0      444 2023-06-29 12:24:52.616649 increase-0.8.0/src/increase/types/inbound_wire_drawdown_request_list_params.py
+-rw-r--r--   0        0        0     1041 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/limit.py
+-rw-r--r--   0        0        0      696 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/limit_create_params.py
+-rw-r--r--   0        0        0      527 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/limit_list_params.py
+-rw-r--r--   0        0        0      332 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/limit_update_params.py
+-rw-r--r--   0        0        0      779 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/oauth_connection.py
+-rw-r--r--   0        0        0      422 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/oauth_connection_list_params.py
+-rw-r--r--   0        0        0    12078 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/pending_transaction.py
+-rw-r--r--   0        0        0     1956 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/pending_transaction_list_params.py
+-rw-r--r--   0        0        0      735 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/program.py
+-rw-r--r--   0        0        0      406 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/program_list_params.py
+-rw-r--r--   0        0        0     6113 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/real_time_decision.py
+-rw-r--r--   0        0        0     2451 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/real_time_decision_action_params.py
+-rw-r--r--   0        0        0     5096 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/real_time_payments_transfer.py
+-rw-r--r--   0        0        0     1283 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/real_time_payments_transfer_create_params.py
+-rw-r--r--   0        0        0     1664 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/real_time_payments_transfer_list_params.py
+-rw-r--r--   0        0        0      895 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/routing_number.py
+-rw-r--r--   0        0        0      522 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/routing_number_list_params.py
+-rw-r--r--   0        0        0      155 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/shared/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/shared/point_of_service_entry_mode.py
+-rw-r--r--   0        0        0      155 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/shared_params/__init__.py
+-rw-r--r--   0        0        0      525 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/shared_params/point_of_service_entry_mode.py
+-rw-r--r--   0        0        0     2608 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/__init__.py
+-rw-r--r--   0        0        0      338 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/account_statement_create_params.py
+-rw-r--r--   0        0        0     1027 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/ach_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0     3303 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/ach_transfer_return_params.py
+-rw-r--r--   0        0        0    51481 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/ach_transfer_simulation.py
+-rw-r--r--   0        0        0    26885 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/card_authorization_simulation.py
+-rw-r--r--   0        0        0      823 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/card_authorize_params.py
+-rw-r--r--   0        0        0      443 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/card_dispute_action_params.py
+-rw-r--r--   0        0        0      400 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/card_refund_create_params.py
+-rw-r--r--   0        0        0      610 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/card_settlement_params.py
+-rw-r--r--   0        0        0      425 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/check_transfer_return_params.py
+-rw-r--r--   0        0        0      346 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/digital_wallet_token_request_create_params.py
+-rw-r--r--   0        0        0      953 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/digital_wallet_token_request_create_response.py
+-rw-r--r--   0        0        0      325 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/document_create_params.py
+-rw-r--r--   0        0        0    51652 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py
+-rw-r--r--   0        0        0     2648 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py
+-rw-r--r--   0        0        0      435 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/interest_payment_create_params.py
+-rw-r--r--   0        0        0    37747 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/interest_payment_simulation_result.py
+-rw-r--r--   0        0        0      299 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/program_create_params.py
+-rw-r--r--   0        0        0     1362 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/real_time_payments_transfer_complete_params.py
+-rw-r--r--   0        0        0     1020 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0     2591 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/wire_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0    37791 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/simulations/wire_transfer_simulation.py
+-rw-r--r--   0        0        0    36238 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/transaction.py
+-rw-r--r--   0        0        0     3293 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/transaction_list_params.py
+-rw-r--r--   0        0        0     2239 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/wire_drawdown_request.py
+-rw-r--r--   0        0        0     1148 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/wire_drawdown_request_create_params.py
+-rw-r--r--   0        0        0      430 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/wire_drawdown_request_list_params.py
+-rw-r--r--   0        0        0     5343 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/wire_transfer.py
+-rw-r--r--   0        0        0     1367 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/wire_transfer_create_params.py
+-rw-r--r--   0        0        0     1588 2023-06-29 12:24:52.620649 increase-0.8.0/src/increase/types/wire_transfer_list_params.py
+-rw-r--r--   0        0        0     9321 1970-01-01 00:00:00.000000 increase-0.8.0/PKG-INFO
```

### Comparing `increase-0.7.1/LICENSE` & `increase-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/README.md` & `increase-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 Or just work directly with the returned data:
 
 ```python
 first_page = await increase.accounts.list()
 
 print(f"next page cursor: {first_page.next_cursor}")  # => "next page cursor: ..."
 for account in first_page.data:
-    print(account.created_at)
+    print(account.id)
 
 # Remove `await` for non-async usage.
 ```
 
 ## Nested params
 
 Nested parameters are dictionaries, typed using `TypedDict`, for example:
@@ -300,8 +300,8 @@
 This package is in beta. Its internals and interfaces are not stable and subject to change without a major semver bump;
 please reach out if you rely on any undocumented behavior.
 
 We are keen for your feedback; please open an [issue](https://www.github.com/increase/increase-python/issues) with questions, bugs, or suggestions.
 
 ## Requirements
 
-Python 3.7 or higher.
+Python 3.7 or higher.
```

### Comparing `increase-0.7.1/pyproject.toml` & `increase-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "increase"
-version = "0.7.1"
+version = "0.8.0"
 description = "Client library for the increase API"
 readme = "README.md"
 authors = ["Increase <dev-feedback@increase.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/increase/increase-python"
 packages = [
   { include = "increase", from = "src" }
```

### Comparing `increase-0.7.1/src/increase/__init__.py` & `increase-0.8.0/src/increase/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/_base_client.py` & `increase-0.8.0/src/increase/_base_client.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/_base_exceptions.py` & `increase-0.8.0/src/increase/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/_client.py` & `increase-0.8.0/src/increase/_client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -312,18 +312,18 @@
             return exceptions.InternalServerError(err_msg, request=request, response=response, body=body)
         if response.status_code == 500:
             return exceptions.InternalServerError(
                 err_msg,
                 request=request,
                 response=response,
                 body={
-                    "type": "internal_server_error",
-                    "title": "",
                     "detail": None,
                     "status": 500,
+                    "title": "",
+                    "type": "internal_server_error",
                 },
             )
         return super()._make_status_error(err_msg, request=request, response=response, body=body)
 
 
 class AsyncIncrease(AsyncAPIClient):
     accounts: resources.AsyncAccounts
@@ -587,18 +587,18 @@
             return exceptions.InternalServerError(err_msg, request=request, response=response, body=body)
         if response.status_code == 500:
             return exceptions.InternalServerError(
                 err_msg,
                 request=request,
                 response=response,
                 body={
-                    "type": "internal_server_error",
-                    "title": "",
                     "detail": None,
                     "status": 500,
+                    "title": "",
+                    "type": "internal_server_error",
                 },
             )
         return super()._make_status_error(err_msg, request=request, response=response, body=body)
 
 
 Client = Increase
```

### Comparing `increase-0.7.1/src/increase/_exceptions.py` & `increase-0.8.0/src/increase/_exceptions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,19 +62,19 @@
     type: Literal["invalid_parameters_error"]
 
     def __init__(self, message: str, *, body: object, request: httpx.Request, response: httpx.Response) -> None:
         data = cast(Mapping[str, object], body if is_mapping(body) else {})
         title = cast(Any, data.get("title"))
         super().__init__(title or message, request=request, response=response, body=body)
 
-        self.type = cast(Any, data.get("type"))
-        self.title = cast(Any, data.get("title"))
         self.detail = cast(Any, data.get("detail"))
-        self.status = cast(Any, data.get("status"))
         self.errors = cast(Any, data.get("errors"))
+        self.status = cast(Any, data.get("status"))
+        self.title = cast(Any, data.get("title"))
+        self.type = cast(Any, data.get("type"))
 
 
 class MalformedRequestError(exceptions.BadRequestError):
     detail: Optional[str]
 
     status: Literal[400]
```

### Comparing `increase-0.7.1/src/increase/_models.py` & `increase-0.8.0/src/increase/_models.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/_qs.py` & `increase-0.8.0/src/increase/_qs.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/_resource.py` & `increase-0.8.0/src/increase/_resource.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/_streaming.py` & `increase-0.8.0/src/increase/_streaming.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/_types.py` & `increase-0.8.0/src/increase/_types.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/_utils/__init__.py` & `increase-0.8.0/src/increase/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/_utils/_transform.py` & `increase-0.8.0/src/increase/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/_utils/_utils.py` & `increase-0.8.0/src/increase/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/pagination.py` & `increase-0.8.0/src/increase/pagination.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/__init__.py` & `increase-0.8.0/src/increase/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/account_numbers.py` & `increase-0.8.0/src/increase/resources/account_numbers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/account_statements.py` & `increase-0.8.0/src/increase/resources/account_statements.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/account_transfers.py` & `increase-0.8.0/src/increase/resources/account_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/accounts.py` & `increase-0.8.0/src/increase/resources/accounts.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/ach_prenotifications.py` & `increase-0.8.0/src/increase/resources/ach_prenotifications.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/ach_transfers.py` & `increase-0.8.0/src/increase/resources/ach_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/balance_lookups.py` & `increase-0.8.0/src/increase/resources/balance_lookups.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/bookkeeping_accounts.py` & `increase-0.8.0/src/increase/resources/bookkeeping_accounts.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/bookkeeping_entries.py` & `increase-0.8.0/src/increase/resources/bookkeeping_entries.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/bookkeeping_entry_sets.py` & `increase-0.8.0/src/increase/resources/bookkeeping_entry_sets.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/card_disputes.py` & `increase-0.8.0/src/increase/resources/card_disputes.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/card_profiles.py` & `increase-0.8.0/src/increase/resources/card_profiles.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/cards.py` & `increase-0.8.0/src/increase/resources/cards.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/check_deposits.py` & `increase-0.8.0/src/increase/resources/check_deposits.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/check_transfers.py` & `increase-0.8.0/src/increase/resources/check_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/declined_transactions.py` & `increase-0.8.0/src/increase/resources/declined_transactions.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/digital_wallet_tokens.py` & `increase-0.8.0/src/increase/resources/digital_wallet_tokens.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/documents.py` & `increase-0.8.0/src/increase/resources/documents.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/entities/entities.py` & `increase-0.8.0/src/increase/resources/entities/entities.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/entities/supplemental_documents.py` & `increase-0.8.0/src/increase/resources/entities/supplemental_documents.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/event_subscriptions.py` & `increase-0.8.0/src/increase/resources/event_subscriptions.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/events.py` & `increase-0.8.0/src/increase/resources/events.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/exports.py` & `increase-0.8.0/src/increase/resources/exports.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/external_accounts.py` & `increase-0.8.0/src/increase/resources/external_accounts.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/files.py` & `increase-0.8.0/src/increase/resources/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
             "check_image_back",
             "form_ss_4",
             "identity_document",
             "other",
             "trust_formation_document",
             "digital_wallet_artwork",
             "digital_wallet_app_icon",
+            "physical_card_artwork",
+            "physical_card_carrier",
             "document_request",
             "entity_supplemental_document",
         ],
         description: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
@@ -189,14 +191,16 @@
             "check_image_back",
             "form_ss_4",
             "identity_document",
             "other",
             "trust_formation_document",
             "digital_wallet_artwork",
             "digital_wallet_app_icon",
+            "physical_card_artwork",
+            "physical_card_carrier",
             "document_request",
             "entity_supplemental_document",
         ],
         description: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
```

### Comparing `increase-0.7.1/src/increase/resources/groups.py` & `increase-0.8.0/src/increase/resources/groups.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/inbound_ach_transfer_returns.py` & `increase-0.8.0/src/increase/resources/inbound_ach_transfer_returns.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/inbound_wire_drawdown_requests.py` & `increase-0.8.0/src/increase/resources/inbound_wire_drawdown_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/limits.py` & `increase-0.8.0/src/increase/resources/limits.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/oauth_connections.py` & `increase-0.8.0/src/increase/resources/oauth_connections.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/pending_transactions.py` & `increase-0.8.0/src/increase/resources/pending_transactions.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/programs.py` & `increase-0.8.0/src/increase/resources/programs.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/real_time_decisions.py` & `increase-0.8.0/src/increase/resources/real_time_decisions.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/real_time_payments_transfers.py` & `increase-0.8.0/src/increase/resources/real_time_payments_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/routing_numbers.py` & `increase-0.8.0/src/increase/resources/routing_numbers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/simulations/__init__.py` & `increase-0.8.0/src/increase/resources/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/simulations/account_statements.py` & `increase-0.8.0/src/increase/resources/simulations/account_statements.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/simulations/account_transfers.py` & `increase-0.8.0/src/increase/resources/simulations/account_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/simulations/ach_transfers.py` & `increase-0.8.0/src/increase/resources/simulations/ach_transfers.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,14 @@
             "authorization_revoked_by_customer",
             "invalid_ach_routing_number",
             "file_record_edit_criteria",
             "enr_invalid_individual_name",
             "returned_per_odfi_request",
             "limited_participation_dfi",
             "incorrectly_coded_outbound_international_payment",
-            "other",
             "account_sold_to_another_dfi",
             "addenda_error",
             "beneficiary_or_account_holder_deceased",
             "customer_advised_not_within_authorization_terms",
             "corrected_return",
             "duplicate_entry",
             "duplicate_return",
@@ -364,15 +363,14 @@
             "authorization_revoked_by_customer",
             "invalid_ach_routing_number",
             "file_record_edit_criteria",
             "enr_invalid_individual_name",
             "returned_per_odfi_request",
             "limited_participation_dfi",
             "incorrectly_coded_outbound_international_payment",
-            "other",
             "account_sold_to_another_dfi",
             "addenda_error",
             "beneficiary_or_account_holder_deceased",
             "customer_advised_not_within_authorization_terms",
             "corrected_return",
             "duplicate_entry",
             "duplicate_return",
```

### Comparing `increase-0.7.1/src/increase/resources/simulations/card_disputes.py` & `increase-0.8.0/src/increase/resources/simulations/card_disputes.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/simulations/card_refunds.py` & `increase-0.8.0/src/increase/resources/simulations/card_refunds.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/simulations/cards.py` & `increase-0.8.0/src/increase/resources/simulations/cards.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/simulations/check_deposits.py` & `increase-0.8.0/src/increase/resources/simulations/check_deposits.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/simulations/check_transfers.py` & `increase-0.8.0/src/increase/resources/simulations/check_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/simulations/digital_wallet_token_requests.py` & `increase-0.8.0/src/increase/resources/simulations/digital_wallet_token_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/simulations/documents.py` & `increase-0.8.0/src/increase/resources/simulations/documents.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/simulations/inbound_wire_drawdown_requests.py` & `increase-0.8.0/src/increase/resources/simulations/inbound_wire_drawdown_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/simulations/interest_payments.py` & `increase-0.8.0/src/increase/resources/simulations/interest_payments.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/simulations/programs.py` & `increase-0.8.0/src/increase/resources/simulations/programs.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/simulations/real_time_payments_transfers.py` & `increase-0.8.0/src/increase/resources/simulations/real_time_payments_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/simulations/simulations.py` & `increase-0.8.0/src/increase/resources/simulations/simulations.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/simulations/wire_transfers.py` & `increase-0.8.0/src/increase/resources/simulations/wire_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/transactions.py` & `increase-0.8.0/src/increase/resources/transactions.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/wire_drawdown_requests.py` & `increase-0.8.0/src/increase/resources/wire_drawdown_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/resources/wire_transfers.py` & `increase-0.8.0/src/increase/resources/wire_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/__init__.py` & `increase-0.8.0/src/increase/types/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/account.py` & `increase-0.8.0/src/increase/types/account.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 from .._models import BaseModel
 
 __all__ = ["Account"]
 
 
 class Account(BaseModel):
+    id: str
+    """The Account identifier."""
+
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the Account
     was created.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
@@ -21,17 +24,14 @@
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the Account
     currency.
     """
 
     entity_id: Optional[str]
     """The identifier for the Entity the Account belongs to."""
 
-    id: str
-    """The Account identifier."""
-
     informational_entity_id: Optional[str]
     """
     The identifier of an Entity that, while not owning the Account, is associated
     with its activity.
     """
 
     interest_accrued: str
```

### Comparing `increase-0.7.1/src/increase/types/account_create_params.py` & `increase-0.8.0/src/increase/types/account_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/account_list_params.py` & `increase-0.8.0/src/increase/types/account_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/account_number.py` & `increase-0.8.0/src/increase/types/account_number.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 from .._models import BaseModel
 
 __all__ = ["AccountNumber"]
 
 
 class AccountNumber(BaseModel):
+    id: str
+    """The Account Number identifier."""
+
     account_id: str
     """The identifier for the account this Account Number belongs to."""
 
     account_number: str
     """The account number."""
 
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the Account
     Number was created.
     """
 
-    id: str
-    """The Account Number identifier."""
-
     name: str
     """The name you choose for the Account Number."""
 
     routing_number: str
     """The American Bankers' Association (ABA) Routing Transit Number (RTN)."""
 
     status: Literal["active", "disabled", "canceled"]
```

### Comparing `increase-0.7.1/src/increase/types/account_number_list_params.py` & `increase-0.8.0/src/increase/types/account_number_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/account_statement.py` & `increase-0.8.0/src/increase/types/account_statement.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from .._models import BaseModel
 
 __all__ = ["AccountStatement"]
 
 
 class AccountStatement(BaseModel):
+    id: str
+    """The Account Statement identifier."""
+
     account_id: str
     """The identifier for the Account this Account Statement belongs to."""
 
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the Account
     Statement was created.
@@ -20,17 +23,14 @@
 
     ending_balance: int
     """The Account's balance at the start of its statement period."""
 
     file_id: str
     """The identifier of the File containing a PDF of the statement."""
 
-    id: str
-    """The Account Statement identifier."""
-
     starting_balance: int
     """The Account's balance at the start of its statement period."""
 
     statement_period_end: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time representing the end
     of the period the Account Statement covers.
```

### Comparing `increase-0.7.1/src/increase/types/account_statement_list_params.py` & `increase-0.8.0/src/increase/types/account_statement_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/account_transfer.py` & `increase-0.8.0/src/increase/types/account_transfer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,17 @@
     """
     If the Transfer was canceled by a user in the dashboard, the email address of
     that user.
     """
 
 
 class AccountTransfer(BaseModel):
+    id: str
+    """The account transfer's identifier."""
+
     account_id: str
     """The Account to which the transfer belongs."""
 
     amount: int
     """The transfer amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
@@ -76,17 +79,14 @@
 
     destination_account_id: str
     """The destination account's identifier."""
 
     destination_transaction_id: Optional[str]
     """The ID for the transaction receiving the transfer."""
 
-    id: str
-    """The account transfer's identifier."""
-
     network: Literal["account"]
     """The transfer's network."""
 
     status: Literal["pending_approval", "canceled", "complete"]
     """The lifecycle status of the transfer."""
 
     transaction_id: Optional[str]
```

### Comparing `increase-0.7.1/src/increase/types/account_transfer_create_params.py` & `increase-0.8.0/src/increase/types/account_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/account_transfer_list_params.py` & `increase-0.8.0/src/increase/types/account_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/ach_prenotification.py` & `increase-0.8.0/src/increase/types/ach_prenotification.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     """
 
     return_reason_code: str
     """Why the Prenotification was returned."""
 
 
 class ACHPrenotification(BaseModel):
+    id: str
+    """The ACH Prenotification's identifier."""
+
     account_number: str
     """The destination account number."""
 
     addendum: Optional[str]
     """Additional information for the recipient."""
 
     company_descriptive_date: Optional[str]
@@ -49,17 +52,14 @@
     """If the notification is for a future credit or debit."""
 
     effective_date: Optional[datetime]
     """
     The effective date in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
     """
 
-    id: str
-    """The ACH Prenotification's identifier."""
-
     prenotification_return: Optional[PrenotificationReturn]
     """If your prenotification is returned, this will contain details of the return."""
 
     routing_number: str
     """The American Bankers' Association (ABA) Routing Transit Number (RTN)."""
 
     status: Literal["pending_submitting", "requires_attention", "returned", "submitted"]
```

### Comparing `increase-0.7.1/src/increase/types/ach_prenotification_create_params.py` & `increase-0.8.0/src/increase/types/ach_prenotification_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/ach_prenotification_list_params.py` & `increase-0.8.0/src/increase/types/ach_prenotification_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/ach_transfer.py` & `increase-0.8.0/src/increase/types/ach_transfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
         "authorization_revoked_by_customer",
         "invalid_ach_routing_number",
         "file_record_edit_criteria",
         "enr_invalid_individual_name",
         "returned_per_odfi_request",
         "limited_participation_dfi",
         "incorrectly_coded_outbound_international_payment",
-        "other",
         "account_sold_to_another_dfi",
         "addenda_error",
         "beneficiary_or_account_holder_deceased",
         "customer_advised_not_within_authorization_terms",
         "corrected_return",
         "duplicate_entry",
         "duplicate_return",
@@ -150,14 +149,17 @@
     """When the ACH transfer was sent to FedACH."""
 
     trace_number: str
     """The trace number for the submission."""
 
 
 class ACHTransfer(BaseModel):
+    id: str
+    """The ACH transfer's identifier."""
+
     account_id: str
     """The Account to which the transfer belongs."""
 
     account_number: str
     """The destination account number."""
 
     addendum: Optional[str]
@@ -215,17 +217,14 @@
 
     external_account_id: Optional[str]
     """The identifier of the External Account the transfer was made to, if any."""
 
     funding: Literal["checking", "savings"]
     """The type of the account to which the transfer will be sent."""
 
-    id: str
-    """The ACH transfer's identifier."""
-
     individual_id: Optional[str]
     """Your identifer for the transfer recipient."""
 
     individual_name: Optional[str]
     """The name of the transfer recipient.
 
     This value is information and not verified by the recipient's bank.
```

### Comparing `increase-0.7.1/src/increase/types/ach_transfer_create_params.py` & `increase-0.8.0/src/increase/types/ach_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/ach_transfer_list_params.py` & `increase-0.8.0/src/increase/types/ach_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/balance_lookup_lookup_params.py` & `increase-0.8.0/src/increase/types/balance_lookup_lookup_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/balance_lookup_lookup_response.py` & `increase-0.8.0/src/increase/types/balance_lookup_lookup_response.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/bookkeeping_account.py` & `increase-0.8.0/src/increase/types/bookkeeping_account.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 from .._models import BaseModel
 
 __all__ = ["BookkeepingAccount"]
 
 
 class BookkeepingAccount(BaseModel):
+    id: str
+    """The account identifier."""
+
     account_id: Optional[str]
     """The API Account associated with this bookkeeping account."""
 
     compliance_category: Optional[Literal["commingled_cash", "customer_balance"]]
     """The compliance category of the account."""
 
     entity_id: Optional[str]
     """The Entity associated with this bookkeeping account."""
 
-    id: str
-    """The account identifier."""
-
     name: str
     """The name you choose for the account."""
 
     type: Literal["bookkeeping_account"]
     """A constant representing the object's type.
 
     For this resource it will always be `bookkeeping_account`.
```

### Comparing `increase-0.7.1/src/increase/types/bookkeeping_account_create_params.py` & `increase-0.8.0/src/increase/types/bookkeeping_account_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/bookkeeping_entry.py` & `increase-0.8.0/src/increase/types/bookkeeping_entry.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 from .._models import BaseModel
 
 __all__ = ["BookkeepingEntry"]
 
 
 class BookkeepingEntry(BaseModel):
+    id: str
+    """The entry identifier."""
+
     account_id: str
     """The identifier for the Account the Entry belongs to."""
 
     amount: int
     """The Entry amount in the minor unit of its currency.
 
     For dollars, for example, this is cents.
     """
 
     entry_set_id: str
     """The identifier for the Account the Entry belongs to."""
 
-    id: str
-    """The entry identifier."""
-
     type: Literal["bookkeeping_entry"]
     """A constant representing the object's type.
 
     For this resource it will always be `bookkeeping_entry`.
     """
```

### Comparing `increase-0.7.1/src/increase/types/bookkeeping_entry_set.py` & `increase-0.8.0/src/increase/types/bookkeeping_entry_set.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 
 from .._models import BaseModel
 
 __all__ = ["BookkeepingEntrySet", "Entry"]
 
 
 class Entry(BaseModel):
+    id: str
+    """The entry identifier."""
+
     account_id: str
     """The bookkeeping account impacted by the entry."""
 
     amount: int
     """The amount of the entry in minor units."""
 
-    id: str
-    """The entry identifier."""
-
 
 class BookkeepingEntrySet(BaseModel):
+    id: str
+    """The entry set identifier."""
+
     date: datetime
     """The timestamp of the entry set."""
 
     entries: List[Entry]
     """The entries"""
 
-    id: str
-    """The entry set identifier."""
-
     transaction_id: Optional[str]
     """The transaction identifier, if any."""
 
     type: Literal["bookkeeping_entry_set"]
     """A constant representing the object's type.
 
     For this resource it will always be `bookkeeping_entry_set`.
```

### Comparing `increase-0.7.1/src/increase/types/bookkeeping_entry_set_create_params.py` & `increase-0.8.0/src/increase/types/bookkeeping_entry_set_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/card.py` & `increase-0.8.0/src/increase/types/card.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,17 @@
     """
     A phone number that can be used to verify the cardholder via one-time passcode
     over SMS.
     """
 
 
 class Card(BaseModel):
+    id: str
+    """The card identifier."""
+
     account_id: str
     """The identifier for the account this card belongs to."""
 
     billing_address: BillingAddress
     """The Card's billing address."""
 
     created_at: datetime
@@ -71,17 +74,14 @@
 
     expiration_month: int
     """The month the card expires in M format (e.g., August is 8)."""
 
     expiration_year: int
     """The year the card expires in YYYY format (e.g., 2025)."""
 
-    id: str
-    """The card identifier."""
-
     last4: str
     """The last 4 digits of the Card's Primary Account Number."""
 
     status: Literal["active", "disabled", "canceled"]
     """This indicates if payments can be made with the card."""
 
     type: Literal["card"]
```

### Comparing `increase-0.7.1/src/increase/types/card_create_params.py` & `increase-0.8.0/src/increase/types/card_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/card_details.py` & `increase-0.8.0/src/increase/types/card_details.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/card_dispute.py` & `increase-0.8.0/src/increase/types/card_dispute.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the Card Dispute was rejected.
     """
 
 
 class CardDispute(BaseModel):
+    id: str
+    """The Card Dispute identifier."""
+
     acceptance: Optional[Acceptance]
     """
     If the Card Dispute's status is `accepted`, this will contain details of the
     successful dispute.
     """
 
     created_at: datetime
@@ -55,17 +58,14 @@
 
     disputed_transaction_id: str
     """The identifier of the Transaction that was disputed."""
 
     explanation: str
     """Why you disputed the Transaction in question."""
 
-    id: str
-    """The Card Dispute identifier."""
-
     rejection: Optional[Rejection]
     """
     If the Card Dispute's status is `rejected`, this will contain details of the
     unsuccessful dispute.
     """
 
     status: Literal["pending_reviewing", "accepted", "rejected"]
```

### Comparing `increase-0.7.1/src/increase/types/card_dispute_list_params.py` & `increase-0.8.0/src/increase/types/card_dispute_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/card_list_params.py` & `increase-0.8.0/src/increase/types/card_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/card_profile.py` & `increase-0.8.0/src/increase/types/card_profile.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,17 @@
     """A user-facing description for whoever is issuing the card."""
 
     text_color: DigitalWalletsTextColor
     """The Card's text color, specified as an RGB triple."""
 
 
 class CardProfile(BaseModel):
+    id: str
+    """The Card Profile identifier."""
+
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the Card Dispute was created.
     """
 
     description: str
@@ -59,17 +62,14 @@
     digital_wallets: DigitalWallets
     """How Cards should appear in digital wallets such as Apple Pay.
 
     Different wallets will use these values to render card artwork appropriately for
     their app.
     """
 
-    id: str
-    """The Card Profile identifier."""
-
     status: Literal["pending", "rejected", "active", "archived"]
     """The status of the Card Profile."""
 
     type: Literal["card_profile"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_profile`.
```

### Comparing `increase-0.7.1/src/increase/types/card_profile_create_params.py` & `increase-0.8.0/src/increase/types/card_profile_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/card_profile_list_params.py` & `increase-0.8.0/src/increase/types/card_profile_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/card_update_params.py` & `increase-0.8.0/src/increase/types/card_update_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     line2: str
     """The second line of the billing address."""
 
 
 class DigitalWallet(TypedDict, total=False):
     card_profile_id: str
-    """The card profile assigned to this digital card.
+    """The card profile assigned to this card.
 
     Card profiles may also be assigned at the program level.
     """
 
     email: str
     """
     An email address that can be used to verify the cardholder via one-time passcode
```

### Comparing `increase-0.7.1/src/increase/types/check_deposit.py` & `increase-0.8.0/src/increase/types/check_deposit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -118,14 +118,17 @@
     """
     The identifier of the transaction that reversed the original check deposit
     transaction.
     """
 
 
 class CheckDeposit(BaseModel):
+    id: str
+    """The deposit's identifier."""
+
     account_id: str
     """The Account the check was deposited into."""
 
     amount: int
     """The deposited amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
@@ -160,17 +163,14 @@
     If your deposit is returned, this will contain details as to why it was
     returned.
     """
 
     front_image_file_id: str
     """The ID for the File containing the image of the front of the check."""
 
-    id: str
-    """The deposit's identifier."""
-
     status: Literal["pending", "submitted", "rejected", "returned"]
     """The status of the Check Deposit."""
 
     transaction_id: Optional[str]
     """The ID for the Transaction created by the deposit."""
 
     type: Literal["check_deposit"]
```

### Comparing `increase-0.7.1/src/increase/types/check_deposit_create_params.py` & `increase-0.8.0/src/increase/types/check_deposit_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/check_deposit_list_params.py` & `increase-0.8.0/src/increase/types/check_deposit_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/check_transfer.py` & `increase-0.8.0/src/increase/types/check_transfer.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,44 +4,24 @@
 from datetime import datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
 __all__ = [
     "CheckTransfer",
-    "ReturnAddress",
     "Approval",
     "Cancellation",
-    "Submission",
-    "StopPaymentRequest",
     "Deposit",
+    "ReturnAddress",
     "ReturnDetails",
+    "StopPaymentRequest",
+    "Submission",
 ]
 
 
-class ReturnAddress(BaseModel):
-    city: Optional[str]
-    """The city of the address."""
-
-    line1: Optional[str]
-    """The first line of the address."""
-
-    line2: Optional[str]
-    """The second line of the address."""
-
-    name: Optional[str]
-    """The name of the address."""
-
-    state: Optional[str]
-    """The US state of the address."""
-
-    zip: Optional[str]
-    """The postal code of the address."""
-
-
 class Approval(BaseModel):
     approved_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the transfer was approved.
     """
 
@@ -62,56 +42,57 @@
     canceled_by: Optional[str]
     """
     If the Transfer was canceled by a user in the dashboard, the email address of
     that user.
     """
 
 
-class Submission(BaseModel):
-    check_number: str
-    """The identitying number of the check."""
-
-    submitted_at: datetime
-    """When this check transfer was submitted to our check printer."""
-
-
-class StopPaymentRequest(BaseModel):
-    requested_at: datetime
-    """The time the stop-payment was requested."""
-
-    transaction_id: str
-    """The transaction ID of the corresponding credit transaction."""
-
-    transfer_id: str
-    """The ID of the check transfer that was stopped."""
-
-    type: Literal["check_transfer_stop_payment_request"]
-    """A constant representing the object's type.
-
-    For this resource it will always be `check_transfer_stop_payment_request`.
-    """
-
-
 class Deposit(BaseModel):
     back_image_file_id: Optional[str]
-    """The ID for the File containing the image of the rear of the check."""
+    """
+    The identifier of the API File object containing an image of the back of the
+    deposited check.
+    """
 
     deposited_at: datetime
     """When the check was deposited."""
 
     front_image_file_id: Optional[str]
-    """The ID for the File containing the image of the front of the check."""
+    """
+    The identifier of the API File object containing an image of the front of the
+    deposited check.
+    """
 
     type: Literal["check_transfer_deposit"]
     """A constant representing the object's type.
 
     For this resource it will always be `check_transfer_deposit`.
     """
 
 
+class ReturnAddress(BaseModel):
+    city: Optional[str]
+    """The city of the address."""
+
+    line1: Optional[str]
+    """The first line of the address."""
+
+    line2: Optional[str]
+    """The second line of the address."""
+
+    name: Optional[str]
+    """The name of the address."""
+
+    state: Optional[str]
+    """The US state of the address."""
+
+    zip: Optional[str]
+    """The postal code of the address."""
+
+
 class ReturnDetails(BaseModel):
     file_id: Optional[str]
     """If available, a document with additional information about the return."""
 
     reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"]
     """The reason why the check was returned."""
 
@@ -127,31 +108,59 @@
     returned check.
     """
 
     transfer_id: str
     """The identifier of the returned Check Transfer."""
 
 
+class StopPaymentRequest(BaseModel):
+    requested_at: datetime
+    """The time the stop-payment was requested."""
+
+    transaction_id: str
+    """The transaction ID of the corresponding credit transaction."""
+
+    transfer_id: str
+    """The ID of the check transfer that was stopped."""
+
+    type: Literal["check_transfer_stop_payment_request"]
+    """A constant representing the object's type.
+
+    For this resource it will always be `check_transfer_stop_payment_request`.
+    """
+
+
+class Submission(BaseModel):
+    check_number: str
+    """The identitying number of the check."""
+
+    submitted_at: datetime
+    """When this check transfer was submitted to our check printer."""
+
+
 class CheckTransfer(BaseModel):
+    id: str
+    """The Check transfer's identifier."""
+
     account_id: str
     """The identifier of the Account from which funds will be transferred."""
 
-    address_city: str
+    address_city: Optional[str]
     """The city of the check's destination."""
 
-    address_line1: str
+    address_line1: Optional[str]
     """The street address of the check's destination."""
 
     address_line2: Optional[str]
     """The second line of the address of the check's destination."""
 
-    address_state: str
+    address_state: Optional[str]
     """The state of the check's destination."""
 
-    address_zip: str
+    address_zip: Optional[str]
     """The postal code of the check's destination."""
 
     amount: int
     """The transfer amount in USD cents."""
 
     approval: Optional[Approval]
     """
@@ -176,30 +185,27 @@
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the check's
     currency.
     """
 
     deposit: Optional[Deposit]
     """After a check transfer is deposited, this will contain supplemental details."""
 
-    id: str
-    """The Check transfer's identifier."""
-
     mailed_at: Optional[datetime]
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the check was mailed.
     """
 
-    message: str
+    message: Optional[str]
     """The descriptor that will be printed on the memo field on the check."""
 
     note: Optional[str]
     """The descriptor that will be printed on the letter included with the check."""
 
-    recipient_name: str
+    recipient_name: Optional[str]
     """The name that will be printed on the check."""
 
     return_address: Optional[ReturnAddress]
     """The return address to be printed on the check."""
 
     return_details: Optional[ReturnDetails]
     """After a check transfer is returned, this will contain supplemental details.
@@ -209,15 +215,14 @@
     """
 
     status: Literal[
         "pending_approval",
         "pending_submission",
         "submitted",
         "pending_mailing",
-        "stopped_and_pending_mailing",
         "mailed",
         "canceled",
         "deposited",
         "stopped",
         "returned",
         "rejected",
         "requires_attention",
```

### Comparing `increase-0.7.1/src/increase/types/check_transfer_create_params.py` & `increase-0.8.0/src/increase/types/check_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/check_transfer_list_params.py` & `increase-0.8.0/src/increase/types/check_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/declined_transaction.py` & `increase-0.8.0/src/increase/types/declined_transaction.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -417,14 +417,17 @@
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_decline`.
     """
 
 
 class DeclinedTransaction(BaseModel):
+    id: str
+    """The Declined Transaction identifier."""
+
     account_id: str
     """The identifier for the Account the Declined Transaction belongs to."""
 
     amount: int
     """The Declined Transaction amount in the minor unit of its currency.
 
     For dollars, for example, this is cents.
@@ -442,17 +445,14 @@
     Transaction's currency. This will match the currency on the Declined
     Transcation's Account.
     """
 
     description: str
     """This is the description the vendor provides."""
 
-    id: str
-    """The Declined Transaction identifier."""
-
     route_id: Optional[str]
     """The identifier for the route this Declined Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
     route_type: Optional[Literal["account_number", "card"]]
```

### Comparing `increase-0.7.1/src/increase/types/declined_transaction_list_params.py` & `increase-0.8.0/src/increase/types/declined_transaction_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/digital_wallet_token.py` & `increase-0.8.0/src/increase/types/digital_wallet_token.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 from .._models import BaseModel
 
 __all__ = ["DigitalWalletToken"]
 
 
 class DigitalWalletToken(BaseModel):
+    id: str
+    """The Digital Wallet Token identifier."""
+
     card_id: str
     """The identifier for the Card this Digital Wallet Token belongs to."""
 
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the Card was created.
     """
 
-    id: str
-    """The Digital Wallet Token identifier."""
-
     status: Literal["active", "inactive", "suspended", "deactivated"]
     """This indicates if payments can be made with the Digital Wallet Token."""
 
     token_requestor: Literal["apple_pay", "google_pay"]
     """The digital wallet app being used."""
 
     type: Literal["digital_wallet_token"]
```

### Comparing `increase-0.7.1/src/increase/types/digital_wallet_token_list_params.py` & `increase-0.8.0/src/increase/types/digital_wallet_token_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/entities/supplemental_document.py` & `increase-0.8.0/src/increase/types/entities/supplemental_document.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/entities/supplemental_document_list_params.py` & `increase-0.8.0/src/increase/types/entities/supplemental_document_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/entity.py` & `increase-0.8.0/src/increase/types/entity.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,31 +10,31 @@
     "Entity",
     "Corporation",
     "CorporationAddress",
     "CorporationBeneficialOwner",
     "CorporationBeneficialOwnerIndividual",
     "CorporationBeneficialOwnerIndividualAddress",
     "CorporationBeneficialOwnerIndividualIdentification",
-    "NaturalPerson",
-    "NaturalPersonAddress",
-    "NaturalPersonIdentification",
     "Joint",
     "JointIndividual",
     "JointIndividualAddress",
     "JointIndividualIdentification",
+    "NaturalPerson",
+    "NaturalPersonAddress",
+    "NaturalPersonIdentification",
+    "SupplementalDocument",
     "Trust",
     "TrustAddress",
+    "TrustGrantor",
+    "TrustGrantorAddress",
+    "TrustGrantorIdentification",
     "TrustTrustee",
     "TrustTrusteeIndividual",
     "TrustTrusteeIndividualAddress",
     "TrustTrusteeIndividualIdentification",
-    "TrustGrantor",
-    "TrustGrantorAddress",
-    "TrustGrantorIdentification",
-    "SupplementalDocument",
 ]
 
 
 class CorporationAddress(BaseModel):
     city: str
     """The city of the address."""
 
@@ -134,15 +134,15 @@
     tax_identifier: Optional[str]
     """The Employer Identification Number (EIN) for the corporation."""
 
     website: Optional[str]
     """The website of the corporation."""
 
 
-class NaturalPersonAddress(BaseModel):
+class JointIndividualAddress(BaseModel):
     city: str
     """The city of the address."""
 
     line1: str
     """The first line of the address."""
 
     line2: Optional[str]
@@ -154,42 +154,50 @@
     the address.
     """
 
     zip: str
     """The ZIP code of the address."""
 
 
-class NaturalPersonIdentification(BaseModel):
+class JointIndividualIdentification(BaseModel):
     method: Literal[
         "social_security_number", "individual_taxpayer_identification_number", "passport", "drivers_license", "other"
     ]
     """A method that can be used to verify the individual's identity."""
 
     number_last4: str
     """
     The last 4 digits of the identification number that can be used to verify the
     individual's identity.
     """
 
 
-class NaturalPerson(BaseModel):
-    address: NaturalPersonAddress
+class JointIndividual(BaseModel):
+    address: JointIndividualAddress
     """The person's address."""
 
     date_of_birth: date
     """The person's date of birth in YYYY-MM-DD format."""
 
-    identification: NaturalPersonIdentification
+    identification: JointIndividualIdentification
     """A means of verifying the person's identity."""
 
     name: str
     """The person's legal name."""
 
 
-class JointIndividualAddress(BaseModel):
+class Joint(BaseModel):
+    individuals: List[JointIndividual]
+    """The two individuals that share control of the entity."""
+
+    name: str
+    """The entity's name."""
+
+
+class NaturalPersonAddress(BaseModel):
     city: str
     """The city of the address."""
 
     line1: str
     """The first line of the address."""
 
     line2: Optional[str]
@@ -201,47 +209,56 @@
     the address.
     """
 
     zip: str
     """The ZIP code of the address."""
 
 
-class JointIndividualIdentification(BaseModel):
+class NaturalPersonIdentification(BaseModel):
     method: Literal[
         "social_security_number", "individual_taxpayer_identification_number", "passport", "drivers_license", "other"
     ]
     """A method that can be used to verify the individual's identity."""
 
     number_last4: str
     """
     The last 4 digits of the identification number that can be used to verify the
     individual's identity.
     """
 
 
-class JointIndividual(BaseModel):
-    address: JointIndividualAddress
+class NaturalPerson(BaseModel):
+    address: NaturalPersonAddress
     """The person's address."""
 
     date_of_birth: date
     """The person's date of birth in YYYY-MM-DD format."""
 
-    identification: JointIndividualIdentification
+    identification: NaturalPersonIdentification
     """A means of verifying the person's identity."""
 
     name: str
     """The person's legal name."""
 
 
-class Joint(BaseModel):
-    individuals: List[JointIndividual]
-    """The two individuals that share control of the entity."""
+class SupplementalDocument(BaseModel):
+    created_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the
+    Supplemental Document was created.
+    """
 
-    name: str
-    """The entity's name."""
+    file_id: str
+    """The File containing the document."""
+
+    type: Literal["entity_supplemental_document"]
+    """A constant representing the object's type.
+
+    For this resource it will always be `entity_supplemental_document`.
+    """
 
 
 class TrustAddress(BaseModel):
     city: str
     """The city of the address."""
 
     line1: str
@@ -256,15 +273,15 @@
     the address.
     """
 
     zip: str
     """The ZIP code of the address."""
 
 
-class TrustTrusteeIndividualAddress(BaseModel):
+class TrustGrantorAddress(BaseModel):
     city: str
     """The city of the address."""
 
     line1: str
     """The first line of the address."""
 
     line2: Optional[str]
@@ -276,53 +293,42 @@
     the address.
     """
 
     zip: str
     """The ZIP code of the address."""
 
 
-class TrustTrusteeIndividualIdentification(BaseModel):
+class TrustGrantorIdentification(BaseModel):
     method: Literal[
         "social_security_number", "individual_taxpayer_identification_number", "passport", "drivers_license", "other"
     ]
     """A method that can be used to verify the individual's identity."""
 
     number_last4: str
     """
     The last 4 digits of the identification number that can be used to verify the
     individual's identity.
     """
 
 
-class TrustTrusteeIndividual(BaseModel):
-    address: TrustTrusteeIndividualAddress
+class TrustGrantor(BaseModel):
+    address: TrustGrantorAddress
     """The person's address."""
 
     date_of_birth: date
     """The person's date of birth in YYYY-MM-DD format."""
 
-    identification: TrustTrusteeIndividualIdentification
+    identification: TrustGrantorIdentification
     """A means of verifying the person's identity."""
 
     name: str
     """The person's legal name."""
 
 
-class TrustTrustee(BaseModel):
-    individual: Optional[TrustTrusteeIndividual]
-    """The individual trustee of the trust.
-
-    Will be present if the trustee's `structure` is equal to `individual`.
-    """
-
-    structure: Literal["individual"]
-    """The structure of the trustee. Will always be equal to `individual`."""
-
-
-class TrustGrantorAddress(BaseModel):
+class TrustTrusteeIndividualAddress(BaseModel):
     city: str
     """The city of the address."""
 
     line1: str
     """The first line of the address."""
 
     line2: Optional[str]
@@ -334,41 +340,52 @@
     the address.
     """
 
     zip: str
     """The ZIP code of the address."""
 
 
-class TrustGrantorIdentification(BaseModel):
+class TrustTrusteeIndividualIdentification(BaseModel):
     method: Literal[
         "social_security_number", "individual_taxpayer_identification_number", "passport", "drivers_license", "other"
     ]
     """A method that can be used to verify the individual's identity."""
 
     number_last4: str
     """
     The last 4 digits of the identification number that can be used to verify the
     individual's identity.
     """
 
 
-class TrustGrantor(BaseModel):
-    address: TrustGrantorAddress
+class TrustTrusteeIndividual(BaseModel):
+    address: TrustTrusteeIndividualAddress
     """The person's address."""
 
     date_of_birth: date
     """The person's date of birth in YYYY-MM-DD format."""
 
-    identification: TrustGrantorIdentification
+    identification: TrustTrusteeIndividualIdentification
     """A means of verifying the person's identity."""
 
     name: str
     """The person's legal name."""
 
 
+class TrustTrustee(BaseModel):
+    individual: Optional[TrustTrusteeIndividual]
+    """The individual trustee of the trust.
+
+    Will be present if the trustee's `structure` is equal to `individual`.
+    """
+
+    structure: Literal["individual"]
+    """The structure of the trustee. Will always be equal to `individual`."""
+
+
 class Trust(BaseModel):
     address: TrustAddress
     """The trust's address."""
 
     category: Literal["revocable", "irrevocable"]
     """Whether the trust is `revocable` or `irrevocable`."""
 
@@ -390,44 +407,27 @@
     tax_identifier: Optional[str]
     """The Employer Identification Number (EIN) of the trust itself."""
 
     trustees: List[TrustTrustee]
     """The trustees of the trust."""
 
 
-class SupplementalDocument(BaseModel):
-    created_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the
-    Supplemental Document was created.
-    """
-
-    file_id: str
-    """The File containing the document."""
-
-    type: Literal["entity_supplemental_document"]
-    """A constant representing the object's type.
-
-    For this resource it will always be `entity_supplemental_document`.
-    """
-
-
 class Entity(BaseModel):
+    id: str
+    """The entity's identifier."""
+
     corporation: Optional[Corporation]
     """Details of the corporation entity.
 
     Will be present if `structure` is equal to `corporation`.
     """
 
     description: Optional[str]
     """The entity's description for display purposes."""
 
-    id: str
-    """The entity's identifier."""
-
     joint: Optional[Joint]
     """Details of the joint entity.
 
     Will be present if `structure` is equal to `joint`.
     """
 
     natural_person: Optional[NaturalPerson]
```

### Comparing `increase-0.7.1/src/increase/types/entity_create_params.py` & `increase-0.8.0/src/increase/types/entity_create_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,46 +12,46 @@
     "EntityCreateParams",
     "Corporation",
     "CorporationAddress",
     "CorporationBeneficialOwner",
     "CorporationBeneficialOwnerIndividual",
     "CorporationBeneficialOwnerIndividualAddress",
     "CorporationBeneficialOwnerIndividualIdentification",
-    "CorporationBeneficialOwnerIndividualIdentificationPassport",
     "CorporationBeneficialOwnerIndividualIdentificationDriversLicense",
     "CorporationBeneficialOwnerIndividualIdentificationOther",
+    "CorporationBeneficialOwnerIndividualIdentificationPassport",
     "Joint",
     "JointIndividual",
     "JointIndividualAddress",
     "JointIndividualIdentification",
-    "JointIndividualIdentificationPassport",
     "JointIndividualIdentificationDriversLicense",
     "JointIndividualIdentificationOther",
+    "JointIndividualIdentificationPassport",
     "NaturalPerson",
     "NaturalPersonAddress",
     "NaturalPersonIdentification",
-    "NaturalPersonIdentificationPassport",
     "NaturalPersonIdentificationDriversLicense",
     "NaturalPersonIdentificationOther",
+    "NaturalPersonIdentificationPassport",
     "SupplementalDocument",
     "Trust",
     "TrustAddress",
     "TrustTrustee",
     "TrustTrusteeIndividual",
     "TrustTrusteeIndividualAddress",
     "TrustTrusteeIndividualIdentification",
-    "TrustTrusteeIndividualIdentificationPassport",
     "TrustTrusteeIndividualIdentificationDriversLicense",
     "TrustTrusteeIndividualIdentificationOther",
+    "TrustTrusteeIndividualIdentificationPassport",
     "TrustGrantor",
     "TrustGrantorAddress",
     "TrustGrantorIdentification",
-    "TrustGrantorIdentificationPassport",
     "TrustGrantorIdentificationDriversLicense",
     "TrustGrantorIdentificationOther",
+    "TrustGrantorIdentificationPassport",
 ]
 
 
 class EntityCreateParams(TypedDict, total=False):
     relationship: Required[Literal["affiliated", "informational", "unaffiliated"]]
     """The relationship between your group and the entity."""
 
@@ -127,25 +127,14 @@
     zip: Required[str]
     """The ZIP code of the address."""
 
     line2: str
     """The second line of the address. This might be the floor or room number."""
 
 
-class CorporationBeneficialOwnerIndividualIdentificationPassport(TypedDict, total=False):
-    country: Required[str]
-    """The country that issued the passport."""
-
-    expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
-    """The passport's expiration date in YYYY-MM-DD format."""
-
-    file_id: Required[str]
-    """The identifier of the File containing the passport."""
-
-
 class CorporationBeneficialOwnerIndividualIdentificationDriversLicense(TypedDict, total=False):
     expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
     """The driver's license's expiration date in YYYY-MM-DD format."""
 
     file_id: Required[str]
     """The identifier of the File containing the driver's license."""
 
@@ -166,14 +155,25 @@
     file_id: Required[str]
     """The identifier of the File containing the document."""
 
     expiration_date: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
     """The document's expiration date in YYYY-MM-DD format."""
 
 
+class CorporationBeneficialOwnerIndividualIdentificationPassport(TypedDict, total=False):
+    country: Required[str]
+    """The country that issued the passport."""
+
+    expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
+    """The passport's expiration date in YYYY-MM-DD format."""
+
+    file_id: Required[str]
+    """The identifier of the File containing the passport."""
+
+
 class CorporationBeneficialOwnerIndividualIdentification(TypedDict, total=False):
     method: Required[
         Literal[
             "social_security_number",
             "individual_taxpayer_identification_number",
             "passport",
             "drivers_license",
@@ -282,25 +282,14 @@
     zip: Required[str]
     """The ZIP code of the address."""
 
     line2: str
     """The second line of the address. This might be the floor or room number."""
 
 
-class JointIndividualIdentificationPassport(TypedDict, total=False):
-    country: Required[str]
-    """The country that issued the passport."""
-
-    expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
-    """The passport's expiration date in YYYY-MM-DD format."""
-
-    file_id: Required[str]
-    """The identifier of the File containing the passport."""
-
-
 class JointIndividualIdentificationDriversLicense(TypedDict, total=False):
     expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
     """The driver's license's expiration date in YYYY-MM-DD format."""
 
     file_id: Required[str]
     """The identifier of the File containing the driver's license."""
 
@@ -321,14 +310,25 @@
     file_id: Required[str]
     """The identifier of the File containing the document."""
 
     expiration_date: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
     """The document's expiration date in YYYY-MM-DD format."""
 
 
+class JointIndividualIdentificationPassport(TypedDict, total=False):
+    country: Required[str]
+    """The country that issued the passport."""
+
+    expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
+    """The passport's expiration date in YYYY-MM-DD format."""
+
+    file_id: Required[str]
+    """The identifier of the File containing the passport."""
+
+
 class JointIndividualIdentification(TypedDict, total=False):
     method: Required[
         Literal[
             "social_security_number",
             "individual_taxpayer_identification_number",
             "passport",
             "drivers_license",
@@ -408,25 +408,14 @@
     zip: Required[str]
     """The ZIP code of the address."""
 
     line2: str
     """The second line of the address. This might be the floor or room number."""
 
 
-class NaturalPersonIdentificationPassport(TypedDict, total=False):
-    country: Required[str]
-    """The country that issued the passport."""
-
-    expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
-    """The passport's expiration date in YYYY-MM-DD format."""
-
-    file_id: Required[str]
-    """The identifier of the File containing the passport."""
-
-
 class NaturalPersonIdentificationDriversLicense(TypedDict, total=False):
     expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
     """The driver's license's expiration date in YYYY-MM-DD format."""
 
     file_id: Required[str]
     """The identifier of the File containing the driver's license."""
 
@@ -447,14 +436,25 @@
     file_id: Required[str]
     """The identifier of the File containing the document."""
 
     expiration_date: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
     """The document's expiration date in YYYY-MM-DD format."""
 
 
+class NaturalPersonIdentificationPassport(TypedDict, total=False):
+    country: Required[str]
+    """The country that issued the passport."""
+
+    expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
+    """The passport's expiration date in YYYY-MM-DD format."""
+
+    file_id: Required[str]
+    """The identifier of the File containing the passport."""
+
+
 class NaturalPersonIdentification(TypedDict, total=False):
     method: Required[
         Literal[
             "social_security_number",
             "individual_taxpayer_identification_number",
             "passport",
             "drivers_license",
@@ -551,25 +551,14 @@
     zip: Required[str]
     """The ZIP code of the address."""
 
     line2: str
     """The second line of the address. This might be the floor or room number."""
 
 
-class TrustTrusteeIndividualIdentificationPassport(TypedDict, total=False):
-    country: Required[str]
-    """The country that issued the passport."""
-
-    expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
-    """The passport's expiration date in YYYY-MM-DD format."""
-
-    file_id: Required[str]
-    """The identifier of the File containing the passport."""
-
-
 class TrustTrusteeIndividualIdentificationDriversLicense(TypedDict, total=False):
     expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
     """The driver's license's expiration date in YYYY-MM-DD format."""
 
     file_id: Required[str]
     """The identifier of the File containing the driver's license."""
 
@@ -590,14 +579,25 @@
     file_id: Required[str]
     """The identifier of the File containing the document."""
 
     expiration_date: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
     """The document's expiration date in YYYY-MM-DD format."""
 
 
+class TrustTrusteeIndividualIdentificationPassport(TypedDict, total=False):
+    country: Required[str]
+    """The country that issued the passport."""
+
+    expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
+    """The passport's expiration date in YYYY-MM-DD format."""
+
+    file_id: Required[str]
+    """The identifier of the File containing the passport."""
+
+
 class TrustTrusteeIndividualIdentification(TypedDict, total=False):
     method: Required[
         Literal[
             "social_security_number",
             "individual_taxpayer_identification_number",
             "passport",
             "drivers_license",
@@ -680,25 +680,14 @@
     zip: Required[str]
     """The ZIP code of the address."""
 
     line2: str
     """The second line of the address. This might be the floor or room number."""
 
 
-class TrustGrantorIdentificationPassport(TypedDict, total=False):
-    country: Required[str]
-    """The country that issued the passport."""
-
-    expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
-    """The passport's expiration date in YYYY-MM-DD format."""
-
-    file_id: Required[str]
-    """The identifier of the File containing the passport."""
-
-
 class TrustGrantorIdentificationDriversLicense(TypedDict, total=False):
     expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
     """The driver's license's expiration date in YYYY-MM-DD format."""
 
     file_id: Required[str]
     """The identifier of the File containing the driver's license."""
 
@@ -719,14 +708,25 @@
     file_id: Required[str]
     """The identifier of the File containing the document."""
 
     expiration_date: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
     """The document's expiration date in YYYY-MM-DD format."""
 
 
+class TrustGrantorIdentificationPassport(TypedDict, total=False):
+    country: Required[str]
+    """The country that issued the passport."""
+
+    expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
+    """The passport's expiration date in YYYY-MM-DD format."""
+
+    file_id: Required[str]
+    """The identifier of the File containing the passport."""
+
+
 class TrustGrantorIdentification(TypedDict, total=False):
     method: Required[
         Literal[
             "social_security_number",
             "individual_taxpayer_identification_number",
             "passport",
             "drivers_license",
```

### Comparing `increase-0.7.1/src/increase/types/entity_list_params.py` & `increase-0.8.0/src/increase/types/entity_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/event.py` & `increase-0.8.0/src/increase/types/event.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from .._models import BaseModel
 
 __all__ = ["Event"]
 
 
 class Event(BaseModel):
+    id: str
+    """The Event identifier."""
+
     associated_object_id: str
     """The identifier of the object that generated this Event."""
 
     associated_object_type: str
     """The type of the object that generated this Event."""
 
     category: Literal[
@@ -72,15 +75,12 @@
     We may add additional possible values for this enum over time; your application
     should be able to handle such additions gracefully.
     """
 
     created_at: datetime
     """The time the Event was created."""
 
-    id: str
-    """The Event identifier."""
-
     type: Literal["event"]
     """A constant representing the object's type.
 
     For this resource it will always be `event`.
     """
```

### Comparing `increase-0.7.1/src/increase/types/event_list_params.py` & `increase-0.8.0/src/increase/types/event_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/event_subscription.py` & `increase-0.8.0/src/increase/types/event_subscription.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 from .._models import BaseModel
 
 __all__ = ["EventSubscription"]
 
 
 class EventSubscription(BaseModel):
-    created_at: datetime
-    """The time the event subscription was created."""
-
     id: str
     """The event subscription identifier."""
 
+    created_at: datetime
+    """The time the event subscription was created."""
+
     selected_event_category: Optional[
         Literal[
             "account.created",
             "account.updated",
             "account_number.created",
             "account_number.updated",
             "account_statement.created",
```

### Comparing `increase-0.7.1/src/increase/types/event_subscription_create_params.py` & `increase-0.8.0/src/increase/types/event_subscription_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/export.py` & `increase-0.8.0/src/increase/types/export.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 from .._models import BaseModel
 
 __all__ = ["Export"]
 
 
 class Export(BaseModel):
+    id: str
+    """The Export identifier."""
+
     category: Literal["transaction_csv", "balance_csv"]
     """The category of the Export.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle that gracefully.
     """
 
@@ -28,17 +31,14 @@
 
     file_id: Optional[str]
     """The File containing the contents of the Export.
 
     This will be present when the Export's status transitions to `complete`.
     """
 
-    id: str
-    """The Export identifier."""
-
     status: Literal["pending", "complete"]
     """The status of the Export."""
 
     type: Literal["export"]
     """A constant representing the object's type.
 
     For this resource it will always be `export`.
```

### Comparing `increase-0.7.1/src/increase/types/export_create_params.py` & `increase-0.8.0/src/increase/types/export_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/external_account.py` & `increase-0.8.0/src/increase/types/external_account.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from .._models import BaseModel
 
 __all__ = ["ExternalAccount"]
 
 
 class ExternalAccount(BaseModel):
+    id: str
+    """The External Account's identifier."""
+
     account_number: str
     """The destination account number."""
 
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the External Account was created.
@@ -20,17 +23,14 @@
 
     description: str
     """The External Account's description for display purposes."""
 
     funding: Literal["checking", "savings", "other"]
     """The type of the account to which the transfer will be sent."""
 
-    id: str
-    """The External Account's identifier."""
-
     routing_number: str
     """The American Bankers' Association (ABA) Routing Transit Number (RTN)."""
 
     status: Literal["active", "archived"]
     """The External Account's status."""
 
     type: Literal["external_account"]
```

### Comparing `increase-0.7.1/src/increase/types/external_account_create_params.py` & `increase-0.8.0/src/increase/types/external_account_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/external_account_list_params.py` & `increase-0.8.0/src/increase/types/external_account_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/file.py` & `increase-0.8.0/src/increase/types/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 from .._models import BaseModel
 
 __all__ = ["File"]
 
 
 class File(BaseModel):
+    id: str
+    """The File's identifier."""
+
     created_at: datetime
     """The time the File was created."""
 
     description: Optional[str]
     """A description of the File."""
 
     direction: Literal["to_increase", "from_increase"]
@@ -24,28 +27,27 @@
 
     The location of this URL may change over time.
     """
 
     filename: Optional[str]
     """The filename that was provided upon upload or generated by Increase."""
 
-    id: str
-    """The File's identifier."""
-
     purpose: Literal[
         "check_image_front",
         "check_image_back",
         "form_1099_int",
         "form_ss_4",
         "identity_document",
         "increase_statement",
         "other",
         "trust_formation_document",
         "digital_wallet_artwork",
         "digital_wallet_app_icon",
+        "physical_card_artwork",
+        "physical_card_carrier",
         "document_request",
         "entity_supplemental_document",
         "export",
     ]
     """What the File will be used for.
 
     We may add additional possible values for this enum over time; your application
```

### Comparing `increase-0.7.1/src/increase/types/file_create_params.py` & `increase-0.8.0/src/increase/types/file_create_params.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,16 @@
             "check_image_back",
             "form_ss_4",
             "identity_document",
             "other",
             "trust_formation_document",
             "digital_wallet_artwork",
             "digital_wallet_app_icon",
+            "physical_card_artwork",
+            "physical_card_carrier",
             "document_request",
             "entity_supplemental_document",
         ]
     ]
     """What the File will be used for in Increase's systems."""
 
     description: str
```

### Comparing `increase-0.7.1/src/increase/types/file_list_params.py` & `increase-0.8.0/src/increase/types/file_list_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,16 @@
                 "form_ss_4",
                 "identity_document",
                 "increase_statement",
                 "other",
                 "trust_formation_document",
                 "digital_wallet_artwork",
                 "digital_wallet_app_icon",
+                "physical_card_artwork",
+                "physical_card_carrier",
                 "document_request",
                 "entity_supplemental_document",
                 "export",
             ]
         ],
     },
     total=False,
```

### Comparing `increase-0.7.1/src/increase/types/group.py` & `increase-0.8.0/src/increase/types/group.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 from .._models import BaseModel
 
 __all__ = ["Group"]
 
 
 class Group(BaseModel):
+    id: str
+    """The Group identifier."""
+
     ach_debit_status: Literal["disabled", "enabled"]
     """If the Group is allowed to create ACH debits."""
 
     activation_status: Literal["unactivated", "activated"]
     """If the Group is activated or not."""
 
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the Group
     was created.
     """
 
-    id: str
-    """The Group identifier."""
-
     type: Literal["group"]
     """A constant representing the object's type.
 
     For this resource it will always be `group`.
     """
```

### Comparing `increase-0.7.1/src/increase/types/inbound_ach_transfer_return.py` & `increase-0.8.0/src/increase/types/inbound_ach_transfer_return.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/inbound_ach_transfer_return_create_params.py` & `increase-0.8.0/src/increase/types/inbound_ach_transfer_return_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/inbound_wire_drawdown_request.py` & `increase-0.8.0/src/increase/types/inbound_wire_drawdown_request.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from .._models import BaseModel
 
 __all__ = ["InboundWireDrawdownRequest"]
 
 
 class InboundWireDrawdownRequest(BaseModel):
+    id: str
+    """The Wire drawdown request identifier."""
+
     amount: int
     """The amount being requested in cents."""
 
     beneficiary_account_number: str
     """The drawdown request's beneficiary's account number."""
 
     beneficiary_address_line1: Optional[str]
@@ -32,17 +35,14 @@
 
     currency: str
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the amount being
     requested. Will always be "USD".
     """
 
-    id: str
-    """The Wire drawdown request identifier."""
-
     message_to_recipient: Optional[str]
     """A message from the drawdown request's originator."""
 
     originator_account_number: str
     """The drawdown request's originator's account number."""
 
     originator_address_line1: Optional[str]
```

### Comparing `increase-0.7.1/src/increase/types/limit.py` & `increase-0.8.0/src/increase/types/limit.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/limit_create_params.py` & `increase-0.8.0/src/increase/types/limit_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/limit_list_params.py` & `increase-0.8.0/src/increase/types/limit_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/oauth_connection.py` & `increase-0.8.0/src/increase/types/oauth_connection.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 from .._models import BaseModel
 
 __all__ = ["OauthConnection"]
 
 
 class OauthConnection(BaseModel):
+    id: str
+    """The OAuth Connection's identifier."""
+
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp when the OAuth
     Connection was created.
     """
 
     group_id: str
     """The identifier of the Group that has authorized your OAuth application."""
 
-    id: str
-    """The OAuth Connection's identifier."""
-
     status: Literal["active", "inactive"]
     """Whether the connection is active."""
 
     type: Literal["oauth_connection"]
     """A constant representing the object's type.
 
     For this resource it will always be `oauth_connection`.
```

### Comparing `increase-0.7.1/src/increase/types/pending_transaction.py` & `increase-0.8.0/src/increase/types/pending_transaction.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,17 @@
 
 class SourceCardAuthorizationNetworkDetails(BaseModel):
     visa: SourceCardAuthorizationNetworkDetailsVisa
     """Fields specific to the `visa` network"""
 
 
 class SourceCardAuthorization(BaseModel):
+    id: str
+    """The Card Authorization identifier."""
+
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
@@ -103,17 +106,14 @@
 
     expires_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) when this authorization
     will expire and the pending transaction will be released.
     """
 
-    id: str
-    """The Card Authorization identifier."""
-
     merchant_acceptor_id: str
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
 
     merchant_category_code: Optional[str]
@@ -339,14 +339,17 @@
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_transfer_instruction`.
     """
 
 
 class PendingTransaction(BaseModel):
+    id: str
+    """The Pending Transaction identifier."""
+
     account_id: str
     """The identifier for the account this Pending Transaction belongs to."""
 
     amount: int
     """The Pending Transaction amount in the minor unit of its currency.
 
     For dollars, for example, this is cents.
@@ -374,17 +377,14 @@
     description: str
     """
     For a Pending Transaction related to a transfer, this is the description you
     provide. For a Pending Transaction related to a payment, this is the description
     the vendor provides.
     """
 
-    id: str
-    """The Pending Transaction identifier."""
-
     route_id: Optional[str]
     """The identifier for the route this Pending Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
     route_type: Optional[Literal["account_number", "card"]]
```

### Comparing `increase-0.7.1/src/increase/types/pending_transaction_list_params.py` & `increase-0.8.0/src/increase/types/pending_transaction_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/program.py` & `increase-0.8.0/src/increase/types/program.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 from .._models import BaseModel
 
 __all__ = ["Program"]
 
 
 class Program(BaseModel):
+    id: str
+    """The Program identifier."""
+
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the Program
     was created.
     """
 
-    id: str
-    """The Program identifier."""
-
     name: str
     """The name of the Program."""
 
     type: Literal["program"]
     """A constant representing the object's type.
 
     For this resource it will always be `program`.
```

### Comparing `increase-0.7.1/src/increase/types/real_time_decision.py` & `increase-0.8.0/src/increase/types/real_time_decision.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from .._models import BaseModel
 
 __all__ = [
     "RealTimeDecision",
     "CardAuthorization",
     "CardAuthorizationNetworkDetails",
     "CardAuthorizationNetworkDetailsVisa",
-    "DigitalWalletToken",
     "DigitalWalletAuthentication",
+    "DigitalWalletToken",
 ]
 
 
 class CardAuthorizationNetworkDetailsVisa(BaseModel):
     electronic_commerce_indicator: Optional[
         Literal[
             "mail_phone_order",
@@ -107,35 +107,14 @@
     settlement_currency: str
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the currency the
     transaction will be settled in.
     """
 
 
-class DigitalWalletToken(BaseModel):
-    card_id: str
-    """The identifier of the Card that is being tokenized."""
-
-    card_profile_id: Optional[str]
-    """The identifier of the Card Profile that was set via the real time decision.
-
-    This will be null until the real time decision is responded to or if the real
-    time decision did not set a card profile.
-    """
-
-    decision: Optional[Literal["approve", "decline"]]
-    """Whether or not the provisioning request was approved.
-
-    This will be null until the real time decision is responded to.
-    """
-
-    digital_wallet: Literal["apple_pay", "google_pay"]
-    """The digital wallet app being used."""
-
-
 class DigitalWalletAuthentication(BaseModel):
     card_id: str
     """The identifier of the Card that is being tokenized."""
 
     channel: Literal["sms", "email"]
     """The channel to send the card user their one-time passcode."""
 
@@ -154,15 +133,39 @@
     `sms`.
     """
 
     result: Optional[Literal["success", "failure"]]
     """Whether your application successfully delivered the one-time passcode."""
 
 
+class DigitalWalletToken(BaseModel):
+    card_id: str
+    """The identifier of the Card that is being tokenized."""
+
+    card_profile_id: Optional[str]
+    """The identifier of the Card Profile that was set via the real time decision.
+
+    This will be null until the real time decision is responded to or if the real
+    time decision did not set a card profile.
+    """
+
+    decision: Optional[Literal["approve", "decline"]]
+    """Whether or not the provisioning request was approved.
+
+    This will be null until the real time decision is responded to.
+    """
+
+    digital_wallet: Literal["apple_pay", "google_pay"]
+    """The digital wallet app being used."""
+
+
 class RealTimeDecision(BaseModel):
+    id: str
+    """The Real-Time Decision identifier."""
+
     card_authorization: Optional[CardAuthorization]
     """Fields related to a card authorization."""
 
     category: Literal[
         "card_authorization_requested", "digital_wallet_token_requested", "digital_wallet_authentication_requested"
     ]
     """The category of the Real-Time Decision."""
@@ -175,17 +178,14 @@
 
     digital_wallet_authentication: Optional[DigitalWalletAuthentication]
     """Fields related to a digital wallet authentication attempt."""
 
     digital_wallet_token: Optional[DigitalWalletToken]
     """Fields related to a digital wallet token provisioning attempt."""
 
-    id: str
-    """The Real-Time Decision identifier."""
-
     status: Literal["pending", "responded", "timed_out"]
     """The status of the Real-Time Decision."""
 
     timeout_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     your application can no longer respond to the Real-Time Decision.
```

### Comparing `increase-0.7.1/src/increase/types/real_time_decision_action_params.py` & `increase-0.8.0/src/increase/types/real_time_decision_action_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/real_time_payments_transfer.py` & `increase-0.8.0/src/increase/types/real_time_payments_transfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Optional
 from datetime import datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
-__all__ = ["RealTimePaymentsTransfer", "Approval", "Cancellation", "Submission", "Rejection"]
+__all__ = ["RealTimePaymentsTransfer", "Approval", "Cancellation", "Rejection", "Submission"]
 
 
 class Approval(BaseModel):
     approved_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the transfer was approved.
@@ -33,25 +33,14 @@
     canceled_by: Optional[str]
     """
     If the Transfer was canceled by a user in the dashboard, the email address of
     that user.
     """
 
 
-class Submission(BaseModel):
-    submitted_at: Optional[datetime]
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
-    the transfer was submitted to The Clearing House.
-    """
-
-    transaction_identification: str
-    """The Real Time Payments network identification of the transfer."""
-
-
 class Rejection(BaseModel):
     reject_reason_additional_information: Optional[str]
     """
     Additional information about the rejection provided by the recipient bank when
     the `reject_reason_code` is `NARRATIVE`.
     """
 
@@ -86,15 +75,29 @@
     rejected_at: Optional[datetime]
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the transfer was rejected.
     """
 
 
+class Submission(BaseModel):
+    submitted_at: Optional[datetime]
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
+    the transfer was submitted to The Clearing House.
+    """
+
+    transaction_identification: str
+    """The Real Time Payments network identification of the transfer."""
+
+
 class RealTimePaymentsTransfer(BaseModel):
+    id: str
+    """The Real Time Payments Transfer's identifier."""
+
     account_id: str
     """The Account from which the transfer was sent."""
 
     amount: int
     """The transfer amount in USD cents."""
 
     approval: Optional[Approval]
@@ -132,17 +135,14 @@
     The destination American Bankers' Association (ABA) Routing Transit Number
     (RTN).
     """
 
     external_account_id: Optional[str]
     """The identifier of the External Account the transfer was made to, if any."""
 
-    id: str
-    """The Real Time Payments Transfer's identifier."""
-
     rejection: Optional[Rejection]
     """
     If the transfer is rejected by Real Time Payments or the destination financial
     institution, this will contain supplemental details.
     """
 
     remittance_information: str
```

### Comparing `increase-0.7.1/src/increase/types/real_time_payments_transfer_create_params.py` & `increase-0.8.0/src/increase/types/real_time_payments_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/real_time_payments_transfer_list_params.py` & `increase-0.8.0/src/increase/types/real_time_payments_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/routing_number.py` & `increase-0.8.0/src/increase/types/routing_number.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/routing_number_list_params.py` & `increase-0.8.0/src/increase/types/routing_number_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/shared_params/point_of_service_entry_mode.py` & `increase-0.8.0/src/increase/types/shared_params/point_of_service_entry_mode.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/simulations/__init__.py` & `increase-0.8.0/src/increase/types/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/simulations/ach_transfer_create_inbound_params.py` & `increase-0.8.0/src/increase/types/simulations/ach_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/simulations/ach_transfer_return_params.py` & `increase-0.8.0/src/increase/types/simulations/ach_transfer_return_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         "authorization_revoked_by_customer",
         "invalid_ach_routing_number",
         "file_record_edit_criteria",
         "enr_invalid_individual_name",
         "returned_per_odfi_request",
         "limited_participation_dfi",
         "incorrectly_coded_outbound_international_payment",
-        "other",
         "account_sold_to_another_dfi",
         "addenda_error",
         "beneficiary_or_account_holder_deceased",
         "customer_advised_not_within_authorization_terms",
         "corrected_return",
         "duplicate_entry",
         "duplicate_return",
```

### Comparing `increase-0.7.1/src/increase/types/simulations/ach_transfer_simulation.py` & `increase-0.8.0/src/increase/types/simulations/ach_transfer_simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,58 +5,514 @@
 from typing_extensions import Literal
 
 from ...types import shared
 from ..._models import BaseModel
 
 __all__ = [
     "ACHTransferSimulation",
+    "DeclinedTransaction",
+    "DeclinedTransactionSource",
+    "DeclinedTransactionSourceACHDecline",
+    "DeclinedTransactionSourceCardDecline",
+    "DeclinedTransactionSourceCardDeclineNetworkDetails",
+    "DeclinedTransactionSourceCardDeclineNetworkDetailsVisa",
+    "DeclinedTransactionSourceCheckDecline",
+    "DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline",
+    "DeclinedTransactionSourceInternationalACHDecline",
+    "DeclinedTransactionSourceWireDecline",
     "Transaction",
     "TransactionSource",
     "TransactionSourceAccountTransferIntention",
     "TransactionSourceACHTransferIntention",
     "TransactionSourceACHTransferRejection",
     "TransactionSourceACHTransferReturn",
     "TransactionSourceCardDisputeAcceptance",
     "TransactionSourceCardRefund",
-    "TransactionSourceCardSettlement",
     "TransactionSourceCardRevenuePayment",
+    "TransactionSourceCardSettlement",
     "TransactionSourceCheckDepositAcceptance",
     "TransactionSourceCheckDepositReturn",
+    "TransactionSourceCheckTransferDeposit",
     "TransactionSourceCheckTransferIntention",
-    "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferRejection",
+    "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferStopPaymentRequest",
     "TransactionSourceFeePayment",
     "TransactionSourceInboundACHTransfer",
     "TransactionSourceInboundCheck",
     "TransactionSourceInboundInternationalACHTransfer",
     "TransactionSourceInboundRealTimePaymentsTransferConfirmation",
-    "TransactionSourceInboundWireDrawdownPaymentReversal",
     "TransactionSourceInboundWireDrawdownPayment",
+    "TransactionSourceInboundWireDrawdownPaymentReversal",
     "TransactionSourceInboundWireReversal",
     "TransactionSourceInboundWireTransfer",
     "TransactionSourceInterestPayment",
     "TransactionSourceInternalSource",
     "TransactionSourceRealTimePaymentsTransferAcknowledgement",
     "TransactionSourceSampleFunds",
     "TransactionSourceWireTransferIntention",
     "TransactionSourceWireTransferRejection",
-    "DeclinedTransaction",
-    "DeclinedTransactionSource",
-    "DeclinedTransactionSourceACHDecline",
-    "DeclinedTransactionSourceCardDecline",
-    "DeclinedTransactionSourceCardDeclineNetworkDetails",
-    "DeclinedTransactionSourceCardDeclineNetworkDetailsVisa",
-    "DeclinedTransactionSourceCheckDecline",
-    "DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline",
-    "DeclinedTransactionSourceInternationalACHDecline",
-    "DeclinedTransactionSourceWireDecline",
 ]
 
 
+class DeclinedTransactionSourceACHDecline(BaseModel):
+    amount: int
+    """The declined amount in the minor unit of the destination account currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    originator_company_descriptive_date: Optional[str]
+
+    originator_company_discretionary_data: Optional[str]
+
+    originator_company_id: str
+
+    originator_company_name: str
+
+    reason: Literal[
+        "ach_route_canceled",
+        "ach_route_disabled",
+        "breaches_limit",
+        "credit_entry_refused_by_receiver",
+        "duplicate_return",
+        "entity_not_active",
+        "group_locked",
+        "insufficient_funds",
+        "misrouted_return",
+        "no_ach_route",
+        "originator_request",
+        "transaction_not_allowed",
+    ]
+    """Why the ACH transfer was declined."""
+
+    receiver_id_number: Optional[str]
+
+    receiver_name: Optional[str]
+
+    trace_number: str
+
+
+class DeclinedTransactionSourceCardDeclineNetworkDetailsVisa(BaseModel):
+    electronic_commerce_indicator: Optional[
+        Literal[
+            "mail_phone_order",
+            "recurring",
+            "installment",
+            "unknown_mail_phone_order",
+            "secure_electronic_commerce",
+            "non_authenticated_security_transaction_at_3ds_capable_merchant",
+            "non_authenticated_security_transaction",
+            "non_secure_transaction",
+        ]
+    ]
+    """
+    For electronic commerce transactions, this identifies the level of security used
+    in obtaining the customer's payment credential. For mail or telephone order
+    transactions, identifies the type of mail or telephone order.
+    """
+
+    point_of_service_entry_mode: Optional[shared.PointOfServiceEntryMode]
+    """
+    The method used to enter the cardholder's primary account number and card
+    expiration date
+    """
+
+
+class DeclinedTransactionSourceCardDeclineNetworkDetails(BaseModel):
+    visa: DeclinedTransactionSourceCardDeclineNetworkDetailsVisa
+    """Fields specific to the `visa` network"""
+
+
+class DeclinedTransactionSourceCardDecline(BaseModel):
+    amount: int
+    """The declined amount in the minor unit of the destination account currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
+    account currency.
+    """
+
+    digital_wallet_token_id: Optional[str]
+    """
+    If the authorization was attempted using a Digital Wallet Token (such as an
+    Apple Pay purchase), the identifier of the token that was used.
+    """
+
+    merchant_acceptor_id: str
+    """
+    The merchant identifier (commonly abbreviated as MID) of the merchant the card
+    is transacting with.
+    """
+
+    merchant_category_code: Optional[str]
+    """
+    The Merchant Category Code (commonly abbreviated as MCC) of the merchant the
+    card is transacting with.
+    """
+
+    merchant_city: Optional[str]
+    """The city the merchant resides in."""
+
+    merchant_country: Optional[str]
+    """The country the merchant resides in."""
+
+    merchant_descriptor: str
+    """The merchant descriptor of the merchant the card is transacting with."""
+
+    merchant_state: Optional[str]
+    """The state the merchant resides in."""
+
+    network: Literal["visa"]
+    """The payment network used to process this card authorization"""
+
+    network_details: DeclinedTransactionSourceCardDeclineNetworkDetails
+    """Fields specific to the `network`"""
+
+    real_time_decision_id: Optional[str]
+    """
+    The identifier of the Real-Time Decision sent to approve or decline this
+    transaction.
+    """
+
+    reason: Literal[
+        "card_not_active",
+        "entity_not_active",
+        "group_locked",
+        "insufficient_funds",
+        "cvv2_mismatch",
+        "transaction_not_allowed",
+        "breaches_internal_limit",
+        "breaches_limit",
+        "webhook_declined",
+        "webhook_timed_out",
+        "declined_by_stand_in_processing",
+        "invalid_physical_card",
+        "missing_original_authorization",
+    ]
+    """Why the transaction was declined."""
+
+
+class DeclinedTransactionSourceCheckDecline(BaseModel):
+    amount: int
+    """The declined amount in the minor unit of the destination account currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    auxiliary_on_us: Optional[str]
+
+    reason: Literal[
+        "ach_route_canceled",
+        "ach_route_disabled",
+        "breaches_limit",
+        "entity_not_active",
+        "group_locked",
+        "insufficient_funds",
+        "unable_to_locate_account",
+        "not_our_item",
+        "unable_to_process",
+        "refer_to_image",
+        "stop_payment_requested",
+        "returned",
+        "duplicate_presentment",
+        "not_authorized",
+        "altered_or_fictitious",
+    ]
+    """Why the check was declined."""
+
+
+class DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline(BaseModel):
+    amount: int
+    """The declined amount in the minor unit of the destination account currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    creditor_name: str
+    """The name the sender of the transfer specified as the recipient of the transfer."""
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code of the declined
+    transfer's currency. This will always be "USD" for a Real Time Payments
+    transfer.
+    """
+
+    debtor_account_number: str
+    """The account number of the account that sent the transfer."""
+
+    debtor_name: str
+    """The name provided by the sender of the transfer."""
+
+    debtor_routing_number: str
+    """The routing number of the account that sent the transfer."""
+
+    reason: Literal[
+        "account_number_canceled",
+        "account_number_disabled",
+        "account_restricted",
+        "group_locked",
+        "entity_not_active",
+        "real_time_payments_not_enabled",
+    ]
+    """Why the transfer was declined."""
+
+    remittance_information: Optional[str]
+    """Additional information included with the transfer."""
+
+    transaction_identification: str
+    """The Real Time Payments network identification of the declined transfer."""
+
+
+class DeclinedTransactionSourceInternationalACHDecline(BaseModel):
+    amount: int
+    """The declined amount in the minor unit of the destination account currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    destination_country_code: str
+
+    destination_currency_code: str
+
+    foreign_exchange_indicator: str
+
+    foreign_exchange_reference: Optional[str]
+
+    foreign_exchange_reference_indicator: str
+
+    foreign_payment_amount: int
+
+    foreign_trace_number: Optional[str]
+
+    international_transaction_type_code: str
+
+    originating_currency_code: str
+
+    originating_depository_financial_institution_branch_country: str
+
+    originating_depository_financial_institution_id: str
+
+    originating_depository_financial_institution_id_qualifier: str
+
+    originating_depository_financial_institution_name: str
+
+    originator_city: str
+
+    originator_company_entry_description: str
+
+    originator_country: str
+
+    originator_identification: str
+
+    originator_name: str
+
+    originator_postal_code: Optional[str]
+
+    originator_state_or_province: Optional[str]
+
+    originator_street_address: str
+
+    payment_related_information: Optional[str]
+
+    payment_related_information2: Optional[str]
+
+    receiver_city: str
+
+    receiver_country: str
+
+    receiver_identification_number: Optional[str]
+
+    receiver_postal_code: Optional[str]
+
+    receiver_state_or_province: Optional[str]
+
+    receiver_street_address: str
+
+    receiving_company_or_individual_name: str
+
+    receiving_depository_financial_institution_country: str
+
+    receiving_depository_financial_institution_id: str
+
+    receiving_depository_financial_institution_id_qualifier: str
+
+    receiving_depository_financial_institution_name: str
+
+    trace_number: str
+
+
+class DeclinedTransactionSourceWireDecline(BaseModel):
+    amount: int
+    """The declined amount in the minor unit of the destination account currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    beneficiary_address_line1: Optional[str]
+
+    beneficiary_address_line2: Optional[str]
+
+    beneficiary_address_line3: Optional[str]
+
+    beneficiary_name: Optional[str]
+
+    beneficiary_reference: Optional[str]
+
+    description: str
+
+    input_message_accountability_data: Optional[str]
+
+    originator_address_line1: Optional[str]
+
+    originator_address_line2: Optional[str]
+
+    originator_address_line3: Optional[str]
+
+    originator_name: Optional[str]
+
+    originator_to_beneficiary_information_line1: Optional[str]
+
+    originator_to_beneficiary_information_line2: Optional[str]
+
+    originator_to_beneficiary_information_line3: Optional[str]
+
+    originator_to_beneficiary_information_line4: Optional[str]
+
+    reason: Literal[
+        "account_number_canceled",
+        "account_number_disabled",
+        "entity_not_active",
+        "group_locked",
+        "no_account_number",
+        "transaction_not_allowed",
+    ]
+    """Why the wire transfer was declined."""
+
+
+class DeclinedTransactionSource(BaseModel):
+    ach_decline: Optional[DeclinedTransactionSourceACHDecline]
+    """A ACH Decline object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `ach_decline`.
+    """
+
+    card_decline: Optional[DeclinedTransactionSourceCardDecline]
+    """A Card Decline object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `card_decline`.
+    """
+
+    category: Literal[
+        "ach_decline",
+        "card_decline",
+        "check_decline",
+        "inbound_real_time_payments_transfer_decline",
+        "international_ach_decline",
+        "wire_decline",
+        "other",
+    ]
+    """The type of decline that took place.
+
+    We may add additional possible values for this enum over time; your application
+    should be able to handle such additions gracefully.
+    """
+
+    check_decline: Optional[DeclinedTransactionSourceCheckDecline]
+    """A Check Decline object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `check_decline`.
+    """
+
+    inbound_real_time_payments_transfer_decline: Optional[
+        DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline
+    ]
+    """A Inbound Real Time Payments Transfer Decline object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `inbound_real_time_payments_transfer_decline`.
+    """
+
+    international_ach_decline: Optional[DeclinedTransactionSourceInternationalACHDecline]
+    """A International ACH Decline object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `international_ach_decline`.
+    """
+
+    wire_decline: Optional[DeclinedTransactionSourceWireDecline]
+    """A Wire Decline object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `wire_decline`.
+    """
+
+
+class DeclinedTransaction(BaseModel):
+    id: str
+    """The Declined Transaction identifier."""
+
+    account_id: str
+    """The identifier for the Account the Declined Transaction belongs to."""
+
+    amount: int
+    """The Declined Transaction amount in the minor unit of its currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    created_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the
+    Transaction occured.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the Declined
+    Transaction's currency. This will match the currency on the Declined
+    Transcation's Account.
+    """
+
+    description: str
+    """This is the description the vendor provides."""
+
+    route_id: Optional[str]
+    """The identifier for the route this Declined Transaction came through.
+
+    Routes are things like cards and ACH details.
+    """
+
+    route_type: Optional[Literal["account_number", "card"]]
+    """The type of the route this Declined Transaction came through."""
+
+    source: DeclinedTransactionSource
+    """
+    This is an object giving more details on the network-level event that caused the
+    Declined Transaction. For example, for a card transaction this lists the
+    merchant's industry and location. Note that for backwards compatibility reasons,
+    additional undocumented keys may appear in this object. These should be treated
+    as deprecated and will be removed in the future.
+    """
+
+    type: Literal["declined_transaction"]
+    """A constant representing the object's type.
+
+    For this resource it will always be `declined_transaction`.
+    """
+
+
 class TransactionSourceAccountTransferIntention(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -129,15 +585,14 @@
         "authorization_revoked_by_customer",
         "invalid_ach_routing_number",
         "file_record_edit_criteria",
         "enr_invalid_individual_name",
         "returned_per_odfi_request",
         "limited_participation_dfi",
         "incorrectly_coded_outbound_international_payment",
-        "other",
         "account_sold_to_another_dfi",
         "addenda_error",
         "beneficiary_or_account_holder_deceased",
         "customer_advised_not_within_authorization_terms",
         "corrected_return",
         "duplicate_entry",
         "duplicate_return",
@@ -207,29 +662,29 @@
     """
     The identifier of the Transaction that was created to return the disputed funds
     to your account.
     """
 
 
 class TransactionSourceCardRefund(BaseModel):
+    id: str
+    """The Card Refund identifier."""
+
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
     """
 
-    id: str
-    """The Card Refund identifier."""
-
     merchant_acceptor_id: Optional[str]
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
 
     merchant_category_code: str
@@ -250,15 +705,41 @@
     type: Literal["card_refund"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_refund`.
     """
 
 
+class TransactionSourceCardRevenuePayment(BaseModel):
+    amount: int
+    """The amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
+    currency.
+    """
+
+    period_end: datetime
+    """The end of the period for which this transaction paid interest."""
+
+    period_start: datetime
+    """The start of the period for which this transaction paid interest."""
+
+    transacted_on_account_id: Optional[str]
+    """The account the card belonged to."""
+
+
 class TransactionSourceCardSettlement(BaseModel):
+    id: str
+    """The Card Settlement identifier."""
+
     amount: int
     """The amount in the minor unit of the transaction's settlement currency.
 
     For dollars, for example, this is cents.
     """
 
     card_authorization: Optional[str]
@@ -269,17 +750,14 @@
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's settlement currency.
     """
 
-    id: str
-    """The Card Settlement identifier."""
-
     merchant_acceptor_id: Optional[str]
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
 
     merchant_category_code: str
@@ -312,37 +790,14 @@
     type: Literal["card_settlement"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_settlement`.
     """
 
 
-class TransactionSourceCardRevenuePayment(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
-    currency.
-    """
-
-    period_end: datetime
-    """The end of the period for which this transaction paid interest."""
-
-    period_start: datetime
-    """The start of the period for which this transaction paid interest."""
-
-    transacted_on_account_id: Optional[str]
-    """The account the card belonged to."""
-
-
 class TransactionSourceCheckDepositAcceptance(BaseModel):
     account_number: str
     """The account number printed on the check."""
 
     amount: int
     """The amount to be deposited in the minor unit of the transaction's currency.
 
@@ -415,46 +870,74 @@
     transaction_id: str
     """
     The identifier of the transaction that reversed the original check deposit
     transaction.
     """
 
 
+class TransactionSourceCheckTransferDeposit(BaseModel):
+    back_image_file_id: Optional[str]
+    """
+    The identifier of the API File object containing an image of the back of the
+    deposited check.
+    """
+
+    deposited_at: datetime
+    """When the check was deposited."""
+
+    front_image_file_id: Optional[str]
+    """
+    The identifier of the API File object containing an image of the front of the
+    deposited check.
+    """
+
+    type: Literal["check_transfer_deposit"]
+    """A constant representing the object's type.
+
+    For this resource it will always be `check_transfer_deposit`.
+    """
+
+
 class TransactionSourceCheckTransferIntention(BaseModel):
-    address_city: str
+    address_city: Optional[str]
     """The city of the check's destination."""
 
-    address_line1: str
+    address_line1: Optional[str]
     """The street address of the check's destination."""
 
     address_line2: Optional[str]
     """The second line of the address of the check's destination."""
 
-    address_state: str
+    address_state: Optional[str]
     """The state of the check's destination."""
 
-    address_zip: str
+    address_zip: Optional[str]
     """The postal code of the check's destination."""
 
     amount: int
     """The transfer amount in USD cents."""
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the check's
     currency.
     """
 
-    recipient_name: str
+    recipient_name: Optional[str]
     """The name that will be printed on the check."""
 
     transfer_id: str
     """The identifier of the Check Transfer with which this is associated."""
 
 
+class TransactionSourceCheckTransferRejection(BaseModel):
+    transfer_id: str
+    """The identifier of the Check Transfer that led to this Transaction."""
+
+
 class TransactionSourceCheckTransferReturn(BaseModel):
     file_id: Optional[str]
     """If available, a document with additional information about the return."""
 
     reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"]
     """The reason why the check was returned."""
 
@@ -470,19 +953,14 @@
     returned check.
     """
 
     transfer_id: str
     """The identifier of the returned Check Transfer."""
 
 
-class TransactionSourceCheckTransferRejection(BaseModel):
-    transfer_id: str
-    """The identifier of the Check Transfer that led to this Transaction."""
-
-
 class TransactionSourceCheckTransferStopPaymentRequest(BaseModel):
     requested_at: datetime
     """The time the stop-payment was requested."""
 
     transaction_id: str
     """The transaction ID of the corresponding credit transaction."""
 
@@ -660,46 +1138,14 @@
     remittance_information: Optional[str]
     """Additional information included with the transfer."""
 
     transaction_identification: str
     """The Real Time Payments network identification of the transfer"""
 
 
-class TransactionSourceInboundWireDrawdownPaymentReversal(BaseModel):
-    amount: int
-    """The amount that was reversed."""
-
-    description: str
-    """The description on the reversal message from Fedwire."""
-
-    input_cycle_date: date
-    """The Fedwire cycle date for the wire reversal."""
-
-    input_message_accountability_data: str
-    """The Fedwire transaction identifier."""
-
-    input_sequence_number: str
-    """The Fedwire sequence number."""
-
-    input_source: str
-    """The Fedwire input source identifier."""
-
-    previous_message_input_cycle_date: date
-    """The Fedwire cycle date for the wire transfer that was reversed."""
-
-    previous_message_input_message_accountability_data: str
-    """The Fedwire transaction identifier for the wire transfer that was reversed."""
-
-    previous_message_input_sequence_number: str
-    """The Fedwire sequence number for the wire transfer that was reversed."""
-
-    previous_message_input_source: str
-    """The Fedwire input source identifier for the wire transfer that was reversed."""
-
-
 class TransactionSourceInboundWireDrawdownPayment(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -724,14 +1170,46 @@
     originator_address_line3: Optional[str]
 
     originator_name: Optional[str]
 
     originator_to_beneficiary_information: Optional[str]
 
 
+class TransactionSourceInboundWireDrawdownPaymentReversal(BaseModel):
+    amount: int
+    """The amount that was reversed."""
+
+    description: str
+    """The description on the reversal message from Fedwire."""
+
+    input_cycle_date: date
+    """The Fedwire cycle date for the wire reversal."""
+
+    input_message_accountability_data: str
+    """The Fedwire transaction identifier."""
+
+    input_sequence_number: str
+    """The Fedwire sequence number."""
+
+    input_source: str
+    """The Fedwire input source identifier."""
+
+    previous_message_input_cycle_date: date
+    """The Fedwire cycle date for the wire transfer that was reversed."""
+
+    previous_message_input_message_accountability_data: str
+    """The Fedwire transaction identifier for the wire transfer that was reversed."""
+
+    previous_message_input_sequence_number: str
+    """The Fedwire sequence number for the wire transfer that was reversed."""
+
+    previous_message_input_source: str
+    """The Fedwire input source identifier for the wire transfer that was reversed."""
+
+
 class TransactionSourceInboundWireReversal(BaseModel):
     amount: int
     """The amount that was reversed."""
 
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
@@ -975,30 +1453,31 @@
     category: Literal[
         "account_transfer_intention",
         "ach_transfer_intention",
         "ach_transfer_rejection",
         "ach_transfer_return",
         "card_dispute_acceptance",
         "card_refund",
-        "card_settlement",
         "card_revenue_payment",
+        "card_settlement",
         "check_deposit_acceptance",
         "check_deposit_return",
+        "check_transfer_deposit",
         "check_transfer_intention",
-        "check_transfer_return",
         "check_transfer_rejection",
+        "check_transfer_return",
         "check_transfer_stop_payment_request",
         "fee_payment",
         "inbound_ach_transfer",
         "inbound_ach_transfer_return_intention",
         "inbound_check",
         "inbound_international_ach_transfer",
         "inbound_real_time_payments_transfer_confirmation",
-        "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_drawdown_payment",
+        "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_reversal",
         "inbound_wire_transfer",
         "interest_payment",
         "internal_source",
         "real_time_payments_transfer_acknowledgement",
         "sample_funds",
         "wire_transfer_intention",
@@ -1021,14 +1500,21 @@
     check_deposit_return: Optional[TransactionSourceCheckDepositReturn]
     """A Check Deposit Return object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_deposit_return`.
     """
 
+    check_transfer_deposit: Optional[TransactionSourceCheckTransferDeposit]
+    """A Check Transfer Deposit object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `check_transfer_deposit`.
+    """
+
     check_transfer_intention: Optional[TransactionSourceCheckTransferIntention]
     """A Check Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_transfer_intention`.
     """
 
@@ -1158,14 +1644,17 @@
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_transfer_rejection`.
     """
 
 
 class Transaction(BaseModel):
+    id: str
+    """The Transaction identifier."""
+
     account_id: str
     """The identifier for the Account the Transaction belongs to."""
 
     amount: int
     """The Transaction amount in the minor unit of its currency.
 
     For dollars, for example, this is cents.
@@ -1187,17 +1676,14 @@
     description: str
     """For a Transaction related to a transfer, this is the description you provide.
 
     For a Transaction related to a payment, this is the description the vendor
     provides.
     """
 
-    id: str
-    """The Transaction identifier."""
-
     route_id: Optional[str]
     """The identifier for the route this Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
     route_type: Optional[Literal["account_number", "card"]]
@@ -1214,469 +1700,14 @@
     type: Literal["transaction"]
     """A constant representing the object's type.
 
     For this resource it will always be `transaction`.
     """
 
 
-class DeclinedTransactionSourceACHDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    originator_company_descriptive_date: Optional[str]
-
-    originator_company_discretionary_data: Optional[str]
-
-    originator_company_id: str
-
-    originator_company_name: str
-
-    reason: Literal[
-        "ach_route_canceled",
-        "ach_route_disabled",
-        "breaches_limit",
-        "credit_entry_refused_by_receiver",
-        "duplicate_return",
-        "entity_not_active",
-        "group_locked",
-        "insufficient_funds",
-        "misrouted_return",
-        "no_ach_route",
-        "originator_request",
-        "transaction_not_allowed",
-    ]
-    """Why the ACH transfer was declined."""
-
-    receiver_id_number: Optional[str]
-
-    receiver_name: Optional[str]
-
-    trace_number: str
-
-
-class DeclinedTransactionSourceCardDeclineNetworkDetailsVisa(BaseModel):
-    electronic_commerce_indicator: Optional[
-        Literal[
-            "mail_phone_order",
-            "recurring",
-            "installment",
-            "unknown_mail_phone_order",
-            "secure_electronic_commerce",
-            "non_authenticated_security_transaction_at_3ds_capable_merchant",
-            "non_authenticated_security_transaction",
-            "non_secure_transaction",
-        ]
-    ]
-    """
-    For electronic commerce transactions, this identifies the level of security used
-    in obtaining the customer's payment credential. For mail or telephone order
-    transactions, identifies the type of mail or telephone order.
-    """
-
-    point_of_service_entry_mode: Optional[shared.PointOfServiceEntryMode]
-    """
-    The method used to enter the cardholder's primary account number and card
-    expiration date
-    """
-
-
-class DeclinedTransactionSourceCardDeclineNetworkDetails(BaseModel):
-    visa: DeclinedTransactionSourceCardDeclineNetworkDetailsVisa
-    """Fields specific to the `visa` network"""
-
-
-class DeclinedTransactionSourceCardDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
-    account currency.
-    """
-
-    digital_wallet_token_id: Optional[str]
-    """
-    If the authorization was attempted using a Digital Wallet Token (such as an
-    Apple Pay purchase), the identifier of the token that was used.
-    """
-
-    merchant_acceptor_id: str
-    """
-    The merchant identifier (commonly abbreviated as MID) of the merchant the card
-    is transacting with.
-    """
-
-    merchant_category_code: Optional[str]
-    """
-    The Merchant Category Code (commonly abbreviated as MCC) of the merchant the
-    card is transacting with.
-    """
-
-    merchant_city: Optional[str]
-    """The city the merchant resides in."""
-
-    merchant_country: Optional[str]
-    """The country the merchant resides in."""
-
-    merchant_descriptor: str
-    """The merchant descriptor of the merchant the card is transacting with."""
-
-    merchant_state: Optional[str]
-    """The state the merchant resides in."""
-
-    network: Literal["visa"]
-    """The payment network used to process this card authorization"""
-
-    network_details: DeclinedTransactionSourceCardDeclineNetworkDetails
-    """Fields specific to the `network`"""
-
-    real_time_decision_id: Optional[str]
-    """
-    The identifier of the Real-Time Decision sent to approve or decline this
-    transaction.
-    """
-
-    reason: Literal[
-        "card_not_active",
-        "entity_not_active",
-        "group_locked",
-        "insufficient_funds",
-        "cvv2_mismatch",
-        "transaction_not_allowed",
-        "breaches_internal_limit",
-        "breaches_limit",
-        "webhook_declined",
-        "webhook_timed_out",
-        "declined_by_stand_in_processing",
-        "invalid_physical_card",
-        "missing_original_authorization",
-    ]
-    """Why the transaction was declined."""
-
-
-class DeclinedTransactionSourceCheckDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    auxiliary_on_us: Optional[str]
-
-    reason: Literal[
-        "ach_route_canceled",
-        "ach_route_disabled",
-        "breaches_limit",
-        "entity_not_active",
-        "group_locked",
-        "insufficient_funds",
-        "unable_to_locate_account",
-        "not_our_item",
-        "unable_to_process",
-        "refer_to_image",
-        "stop_payment_requested",
-        "returned",
-        "duplicate_presentment",
-        "not_authorized",
-        "altered_or_fictitious",
-    ]
-    """Why the check was declined."""
-
-
-class DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    creditor_name: str
-    """The name the sender of the transfer specified as the recipient of the transfer."""
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code of the declined
-    transfer's currency. This will always be "USD" for a Real Time Payments
-    transfer.
-    """
-
-    debtor_account_number: str
-    """The account number of the account that sent the transfer."""
-
-    debtor_name: str
-    """The name provided by the sender of the transfer."""
-
-    debtor_routing_number: str
-    """The routing number of the account that sent the transfer."""
-
-    reason: Literal[
-        "account_number_canceled",
-        "account_number_disabled",
-        "account_restricted",
-        "group_locked",
-        "entity_not_active",
-        "real_time_payments_not_enabled",
-    ]
-    """Why the transfer was declined."""
-
-    remittance_information: Optional[str]
-    """Additional information included with the transfer."""
-
-    transaction_identification: str
-    """The Real Time Payments network identification of the declined transfer."""
-
-
-class DeclinedTransactionSourceInternationalACHDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    destination_country_code: str
-
-    destination_currency_code: str
-
-    foreign_exchange_indicator: str
-
-    foreign_exchange_reference: Optional[str]
-
-    foreign_exchange_reference_indicator: str
-
-    foreign_payment_amount: int
-
-    foreign_trace_number: Optional[str]
-
-    international_transaction_type_code: str
-
-    originating_currency_code: str
-
-    originating_depository_financial_institution_branch_country: str
-
-    originating_depository_financial_institution_id: str
-
-    originating_depository_financial_institution_id_qualifier: str
-
-    originating_depository_financial_institution_name: str
-
-    originator_city: str
-
-    originator_company_entry_description: str
-
-    originator_country: str
-
-    originator_identification: str
-
-    originator_name: str
-
-    originator_postal_code: Optional[str]
-
-    originator_state_or_province: Optional[str]
-
-    originator_street_address: str
-
-    payment_related_information: Optional[str]
-
-    payment_related_information2: Optional[str]
-
-    receiver_city: str
-
-    receiver_country: str
-
-    receiver_identification_number: Optional[str]
-
-    receiver_postal_code: Optional[str]
-
-    receiver_state_or_province: Optional[str]
-
-    receiver_street_address: str
-
-    receiving_company_or_individual_name: str
-
-    receiving_depository_financial_institution_country: str
-
-    receiving_depository_financial_institution_id: str
-
-    receiving_depository_financial_institution_id_qualifier: str
-
-    receiving_depository_financial_institution_name: str
-
-    trace_number: str
-
-
-class DeclinedTransactionSourceWireDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    beneficiary_address_line1: Optional[str]
-
-    beneficiary_address_line2: Optional[str]
-
-    beneficiary_address_line3: Optional[str]
-
-    beneficiary_name: Optional[str]
-
-    beneficiary_reference: Optional[str]
-
-    description: str
-
-    input_message_accountability_data: Optional[str]
-
-    originator_address_line1: Optional[str]
-
-    originator_address_line2: Optional[str]
-
-    originator_address_line3: Optional[str]
-
-    originator_name: Optional[str]
-
-    originator_to_beneficiary_information_line1: Optional[str]
-
-    originator_to_beneficiary_information_line2: Optional[str]
-
-    originator_to_beneficiary_information_line3: Optional[str]
-
-    originator_to_beneficiary_information_line4: Optional[str]
-
-    reason: Literal[
-        "account_number_canceled",
-        "account_number_disabled",
-        "entity_not_active",
-        "group_locked",
-        "no_account_number",
-        "transaction_not_allowed",
-    ]
-    """Why the wire transfer was declined."""
-
-
-class DeclinedTransactionSource(BaseModel):
-    ach_decline: Optional[DeclinedTransactionSourceACHDecline]
-    """A ACH Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_decline`.
-    """
-
-    card_decline: Optional[DeclinedTransactionSourceCardDecline]
-    """A Card Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_decline`.
-    """
-
-    category: Literal[
-        "ach_decline",
-        "card_decline",
-        "check_decline",
-        "inbound_real_time_payments_transfer_decline",
-        "international_ach_decline",
-        "wire_decline",
-        "other",
-    ]
-    """The type of decline that took place.
-
-    We may add additional possible values for this enum over time; your application
-    should be able to handle such additions gracefully.
-    """
-
-    check_decline: Optional[DeclinedTransactionSourceCheckDecline]
-    """A Check Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_decline`.
-    """
-
-    inbound_real_time_payments_transfer_decline: Optional[
-        DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline
-    ]
-    """A Inbound Real Time Payments Transfer Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `inbound_real_time_payments_transfer_decline`.
-    """
-
-    international_ach_decline: Optional[DeclinedTransactionSourceInternationalACHDecline]
-    """A International ACH Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `international_ach_decline`.
-    """
-
-    wire_decline: Optional[DeclinedTransactionSourceWireDecline]
-    """A Wire Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_decline`.
-    """
-
-
-class DeclinedTransaction(BaseModel):
-    account_id: str
-    """The identifier for the Account the Declined Transaction belongs to."""
-
-    amount: int
-    """The Declined Transaction amount in the minor unit of its currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    created_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the
-    Transaction occured.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the Declined
-    Transaction's currency. This will match the currency on the Declined
-    Transcation's Account.
-    """
-
-    description: str
-    """This is the description the vendor provides."""
-
-    id: str
-    """The Declined Transaction identifier."""
-
-    route_id: Optional[str]
-    """The identifier for the route this Declined Transaction came through.
-
-    Routes are things like cards and ACH details.
-    """
-
-    route_type: Optional[Literal["account_number", "card"]]
-    """The type of the route this Declined Transaction came through."""
-
-    source: DeclinedTransactionSource
-    """
-    This is an object giving more details on the network-level event that caused the
-    Declined Transaction. For example, for a card transaction this lists the
-    merchant's industry and location. Note that for backwards compatibility reasons,
-    additional undocumented keys may appear in this object. These should be treated
-    as deprecated and will be removed in the future.
-    """
-
-    type: Literal["declined_transaction"]
-    """A constant representing the object's type.
-
-    For this resource it will always be `declined_transaction`.
-    """
-
-
 class ACHTransferSimulation(BaseModel):
     declined_transaction: Optional[DeclinedTransaction]
     """
     If the ACH Transfer attempt fails, this will contain the resulting
     [Declined Transaction](#declined-transactions) object. The Declined
     Transaction's `source` will be of `category: inbound_ach_transfer`.
     """
```

### Comparing `increase-0.7.1/src/increase/types/simulations/card_authorization_simulation.py` & `increase-0.8.0/src/increase/types/simulations/card_authorization_simulation.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,426 +5,39 @@
 from typing_extensions import Literal
 
 from ...types import shared
 from ..._models import BaseModel
 
 __all__ = [
     "CardAuthorizationSimulation",
+    "DeclinedTransaction",
+    "DeclinedTransactionSource",
+    "DeclinedTransactionSourceACHDecline",
+    "DeclinedTransactionSourceCardDecline",
+    "DeclinedTransactionSourceCardDeclineNetworkDetails",
+    "DeclinedTransactionSourceCardDeclineNetworkDetailsVisa",
+    "DeclinedTransactionSourceCheckDecline",
+    "DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline",
+    "DeclinedTransactionSourceInternationalACHDecline",
+    "DeclinedTransactionSourceWireDecline",
     "PendingTransaction",
     "PendingTransactionSource",
     "PendingTransactionSourceAccountTransferInstruction",
     "PendingTransactionSourceACHTransferInstruction",
     "PendingTransactionSourceCardAuthorization",
     "PendingTransactionSourceCardAuthorizationNetworkDetails",
     "PendingTransactionSourceCardAuthorizationNetworkDetailsVisa",
     "PendingTransactionSourceCheckDepositInstruction",
     "PendingTransactionSourceCheckTransferInstruction",
     "PendingTransactionSourceInboundFundsHold",
     "PendingTransactionSourceRealTimePaymentsTransferInstruction",
     "PendingTransactionSourceWireTransferInstruction",
-    "DeclinedTransaction",
-    "DeclinedTransactionSource",
-    "DeclinedTransactionSourceACHDecline",
-    "DeclinedTransactionSourceCardDecline",
-    "DeclinedTransactionSourceCardDeclineNetworkDetails",
-    "DeclinedTransactionSourceCardDeclineNetworkDetailsVisa",
-    "DeclinedTransactionSourceCheckDecline",
-    "DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline",
-    "DeclinedTransactionSourceInternationalACHDecline",
-    "DeclinedTransactionSourceWireDecline",
 ]
 
 
-class PendingTransactionSourceAccountTransferInstruction(BaseModel):
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
-    account currency.
-    """
-
-    transfer_id: str
-    """The identifier of the Account Transfer that led to this Pending Transaction."""
-
-
-class PendingTransactionSourceACHTransferInstruction(BaseModel):
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    transfer_id: str
-    """The identifier of the ACH Transfer that led to this Pending Transaction."""
-
-
-class PendingTransactionSourceCardAuthorizationNetworkDetailsVisa(BaseModel):
-    electronic_commerce_indicator: Optional[
-        Literal[
-            "mail_phone_order",
-            "recurring",
-            "installment",
-            "unknown_mail_phone_order",
-            "secure_electronic_commerce",
-            "non_authenticated_security_transaction_at_3ds_capable_merchant",
-            "non_authenticated_security_transaction",
-            "non_secure_transaction",
-        ]
-    ]
-    """
-    For electronic commerce transactions, this identifies the level of security used
-    in obtaining the customer's payment credential. For mail or telephone order
-    transactions, identifies the type of mail or telephone order.
-    """
-
-    point_of_service_entry_mode: Optional[shared.PointOfServiceEntryMode]
-    """
-    The method used to enter the cardholder's primary account number and card
-    expiration date
-    """
-
-
-class PendingTransactionSourceCardAuthorizationNetworkDetails(BaseModel):
-    visa: PendingTransactionSourceCardAuthorizationNetworkDetailsVisa
-    """Fields specific to the `visa` network"""
-
-
-class PendingTransactionSourceCardAuthorization(BaseModel):
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's currency.
-    """
-
-    digital_wallet_token_id: Optional[str]
-    """
-    If the authorization was made via a Digital Wallet Token (such as an Apple Pay
-    purchase), the identifier of the token that was used.
-    """
-
-    expires_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) when this authorization
-    will expire and the pending transaction will be released.
-    """
-
-    id: str
-    """The Card Authorization identifier."""
-
-    merchant_acceptor_id: str
-    """
-    The merchant identifier (commonly abbreviated as MID) of the merchant the card
-    is transacting with.
-    """
-
-    merchant_category_code: Optional[str]
-    """
-    The Merchant Category Code (commonly abbreviated as MCC) of the merchant the
-    card is transacting with.
-    """
-
-    merchant_city: Optional[str]
-    """The city the merchant resides in."""
-
-    merchant_country: Optional[str]
-    """The country the merchant resides in."""
-
-    merchant_descriptor: str
-    """The merchant descriptor of the merchant the card is transacting with."""
-
-    network: Literal["visa"]
-    """The payment network used to process this card authorization"""
-
-    network_details: PendingTransactionSourceCardAuthorizationNetworkDetails
-    """Fields specific to the `network`"""
-
-    pending_transaction_id: Optional[str]
-    """The identifier of the Pending Transaction associated with this Transaction."""
-
-    real_time_decision_id: Optional[str]
-    """
-    The identifier of the Real-Time Decision sent to approve or decline this
-    transaction.
-    """
-
-    type: Literal["card_authorization"]
-    """A constant representing the object's type.
-
-    For this resource it will always be `card_authorization`.
-    """
-
-
-class PendingTransactionSourceCheckDepositInstruction(BaseModel):
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    back_image_file_id: Optional[str]
-    """
-    The identifier of the File containing the image of the back of the check that
-    was deposited.
-    """
-
-    check_deposit_id: Optional[str]
-    """The identifier of the Check Deposit."""
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's currency.
-    """
-
-    front_image_file_id: str
-    """
-    The identifier of the File containing the image of the front of the check that
-    was deposited.
-    """
-
-
-class PendingTransactionSourceCheckTransferInstruction(BaseModel):
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the check's
-    currency.
-    """
-
-    transfer_id: str
-    """The identifier of the Check Transfer that led to this Pending Transaction."""
-
-
-class PendingTransactionSourceInboundFundsHold(BaseModel):
-    amount: int
-    """The held amount in the minor unit of the account's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    automatically_releases_at: datetime
-    """When the hold will be released automatically.
-
-    Certain conditions may cause it to be released before this time.
-    """
-
-    created_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the hold
-    was created.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the hold's
-    currency.
-    """
-
-    held_transaction_id: Optional[str]
-    """The ID of the Transaction for which funds were held."""
-
-    pending_transaction_id: Optional[str]
-    """The ID of the Pending Transaction representing the held funds."""
-
-    released_at: Optional[datetime]
-    """When the hold was released (if it has been released)."""
-
-    status: Literal["held", "complete"]
-    """The status of the hold."""
-
-
-class PendingTransactionSourceRealTimePaymentsTransferInstruction(BaseModel):
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    transfer_id: str
-    """
-    The identifier of the Real Time Payments Transfer that led to this Pending
-    Transaction.
-    """
-
-
-class PendingTransactionSourceWireTransferInstruction(BaseModel):
-    account_number: str
-
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    message_to_recipient: str
-
-    routing_number: str
-
-    transfer_id: str
-
-
-class PendingTransactionSource(BaseModel):
-    account_transfer_instruction: Optional[PendingTransactionSourceAccountTransferInstruction]
-    """A Account Transfer Instruction object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `account_transfer_instruction`.
-    """
-
-    ach_transfer_instruction: Optional[PendingTransactionSourceACHTransferInstruction]
-    """A ACH Transfer Instruction object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_transfer_instruction`.
-    """
-
-    card_authorization: Optional[PendingTransactionSourceCardAuthorization]
-    """A Card Authorization object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_authorization`.
-    """
-
-    category: Literal[
-        "account_transfer_instruction",
-        "ach_transfer_instruction",
-        "card_authorization",
-        "check_deposit_instruction",
-        "check_transfer_instruction",
-        "inbound_funds_hold",
-        "real_time_payments_transfer_instruction",
-        "wire_transfer_instruction",
-        "other",
-    ]
-    """The type of transaction that took place.
-
-    We may add additional possible values for this enum over time; your application
-    should be able to handle such additions gracefully.
-    """
-
-    check_deposit_instruction: Optional[PendingTransactionSourceCheckDepositInstruction]
-    """A Check Deposit Instruction object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_deposit_instruction`.
-    """
-
-    check_transfer_instruction: Optional[PendingTransactionSourceCheckTransferInstruction]
-    """A Check Transfer Instruction object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_transfer_instruction`.
-    """
-
-    inbound_funds_hold: Optional[PendingTransactionSourceInboundFundsHold]
-    """A Inbound Funds Hold object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `inbound_funds_hold`.
-    """
-
-    real_time_payments_transfer_instruction: Optional[PendingTransactionSourceRealTimePaymentsTransferInstruction]
-    """A Real Time Payments Transfer Instruction object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `real_time_payments_transfer_instruction`.
-    """
-
-    wire_transfer_instruction: Optional[PendingTransactionSourceWireTransferInstruction]
-    """A Wire Transfer Instruction object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_transfer_instruction`.
-    """
-
-
-class PendingTransaction(BaseModel):
-    account_id: str
-    """The identifier for the account this Pending Transaction belongs to."""
-
-    amount: int
-    """The Pending Transaction amount in the minor unit of its currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    completed_at: Optional[datetime]
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the Pending
-    Transaction was completed.
-    """
-
-    created_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the Pending
-    Transaction occured.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the Pending
-    Transaction's currency. This will match the currency on the Pending
-    Transcation's Account.
-    """
-
-    description: str
-    """
-    For a Pending Transaction related to a transfer, this is the description you
-    provide. For a Pending Transaction related to a payment, this is the description
-    the vendor provides.
-    """
-
-    id: str
-    """The Pending Transaction identifier."""
-
-    route_id: Optional[str]
-    """The identifier for the route this Pending Transaction came through.
-
-    Routes are things like cards and ACH details.
-    """
-
-    route_type: Optional[Literal["account_number", "card"]]
-    """The type of the route this Pending Transaction came through."""
-
-    source: PendingTransactionSource
-    """
-    This is an object giving more details on the network-level event that caused the
-    Pending Transaction. For example, for a card transaction this lists the
-    merchant's industry and location.
-    """
-
-    status: Literal["pending", "complete"]
-    """
-    Whether the Pending Transaction has been confirmed and has an associated
-    Transaction.
-    """
-
-    type: Literal["pending_transaction"]
-    """A constant representing the object's type.
-
-    For this resource it will always be `pending_transaction`.
-    """
-
-
 class DeclinedTransactionSourceACHDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -819,14 +432,17 @@
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_decline`.
     """
 
 
 class DeclinedTransaction(BaseModel):
+    id: str
+    """The Declined Transaction identifier."""
+
     account_id: str
     """The identifier for the Account the Declined Transaction belongs to."""
 
     amount: int
     """The Declined Transaction amount in the minor unit of its currency.
 
     For dollars, for example, this is cents.
@@ -844,17 +460,14 @@
     Transaction's currency. This will match the currency on the Declined
     Transcation's Account.
     """
 
     description: str
     """This is the description the vendor provides."""
 
-    id: str
-    """The Declined Transaction identifier."""
-
     route_id: Optional[str]
     """The identifier for the route this Declined Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
     route_type: Optional[Literal["account_number", "card"]]
@@ -872,14 +485,401 @@
     type: Literal["declined_transaction"]
     """A constant representing the object's type.
 
     For this resource it will always be `declined_transaction`.
     """
 
 
+class PendingTransactionSourceAccountTransferInstruction(BaseModel):
+    amount: int
+    """The pending amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
+    account currency.
+    """
+
+    transfer_id: str
+    """The identifier of the Account Transfer that led to this Pending Transaction."""
+
+
+class PendingTransactionSourceACHTransferInstruction(BaseModel):
+    amount: int
+    """The pending amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    transfer_id: str
+    """The identifier of the ACH Transfer that led to this Pending Transaction."""
+
+
+class PendingTransactionSourceCardAuthorizationNetworkDetailsVisa(BaseModel):
+    electronic_commerce_indicator: Optional[
+        Literal[
+            "mail_phone_order",
+            "recurring",
+            "installment",
+            "unknown_mail_phone_order",
+            "secure_electronic_commerce",
+            "non_authenticated_security_transaction_at_3ds_capable_merchant",
+            "non_authenticated_security_transaction",
+            "non_secure_transaction",
+        ]
+    ]
+    """
+    For electronic commerce transactions, this identifies the level of security used
+    in obtaining the customer's payment credential. For mail or telephone order
+    transactions, identifies the type of mail or telephone order.
+    """
+
+    point_of_service_entry_mode: Optional[shared.PointOfServiceEntryMode]
+    """
+    The method used to enter the cardholder's primary account number and card
+    expiration date
+    """
+
+
+class PendingTransactionSourceCardAuthorizationNetworkDetails(BaseModel):
+    visa: PendingTransactionSourceCardAuthorizationNetworkDetailsVisa
+    """Fields specific to the `visa` network"""
+
+
+class PendingTransactionSourceCardAuthorization(BaseModel):
+    id: str
+    """The Card Authorization identifier."""
+
+    amount: int
+    """The pending amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
+    transaction's currency.
+    """
+
+    digital_wallet_token_id: Optional[str]
+    """
+    If the authorization was made via a Digital Wallet Token (such as an Apple Pay
+    purchase), the identifier of the token that was used.
+    """
+
+    expires_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) when this authorization
+    will expire and the pending transaction will be released.
+    """
+
+    merchant_acceptor_id: str
+    """
+    The merchant identifier (commonly abbreviated as MID) of the merchant the card
+    is transacting with.
+    """
+
+    merchant_category_code: Optional[str]
+    """
+    The Merchant Category Code (commonly abbreviated as MCC) of the merchant the
+    card is transacting with.
+    """
+
+    merchant_city: Optional[str]
+    """The city the merchant resides in."""
+
+    merchant_country: Optional[str]
+    """The country the merchant resides in."""
+
+    merchant_descriptor: str
+    """The merchant descriptor of the merchant the card is transacting with."""
+
+    network: Literal["visa"]
+    """The payment network used to process this card authorization"""
+
+    network_details: PendingTransactionSourceCardAuthorizationNetworkDetails
+    """Fields specific to the `network`"""
+
+    pending_transaction_id: Optional[str]
+    """The identifier of the Pending Transaction associated with this Transaction."""
+
+    real_time_decision_id: Optional[str]
+    """
+    The identifier of the Real-Time Decision sent to approve or decline this
+    transaction.
+    """
+
+    type: Literal["card_authorization"]
+    """A constant representing the object's type.
+
+    For this resource it will always be `card_authorization`.
+    """
+
+
+class PendingTransactionSourceCheckDepositInstruction(BaseModel):
+    amount: int
+    """The pending amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    back_image_file_id: Optional[str]
+    """
+    The identifier of the File containing the image of the back of the check that
+    was deposited.
+    """
+
+    check_deposit_id: Optional[str]
+    """The identifier of the Check Deposit."""
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
+    transaction's currency.
+    """
+
+    front_image_file_id: str
+    """
+    The identifier of the File containing the image of the front of the check that
+    was deposited.
+    """
+
+
+class PendingTransactionSourceCheckTransferInstruction(BaseModel):
+    amount: int
+    """The pending amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the check's
+    currency.
+    """
+
+    transfer_id: str
+    """The identifier of the Check Transfer that led to this Pending Transaction."""
+
+
+class PendingTransactionSourceInboundFundsHold(BaseModel):
+    amount: int
+    """The held amount in the minor unit of the account's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    automatically_releases_at: datetime
+    """When the hold will be released automatically.
+
+    Certain conditions may cause it to be released before this time.
+    """
+
+    created_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the hold
+    was created.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the hold's
+    currency.
+    """
+
+    held_transaction_id: Optional[str]
+    """The ID of the Transaction for which funds were held."""
+
+    pending_transaction_id: Optional[str]
+    """The ID of the Pending Transaction representing the held funds."""
+
+    released_at: Optional[datetime]
+    """When the hold was released (if it has been released)."""
+
+    status: Literal["held", "complete"]
+    """The status of the hold."""
+
+
+class PendingTransactionSourceRealTimePaymentsTransferInstruction(BaseModel):
+    amount: int
+    """The pending amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    transfer_id: str
+    """
+    The identifier of the Real Time Payments Transfer that led to this Pending
+    Transaction.
+    """
+
+
+class PendingTransactionSourceWireTransferInstruction(BaseModel):
+    account_number: str
+
+    amount: int
+    """The pending amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    message_to_recipient: str
+
+    routing_number: str
+
+    transfer_id: str
+
+
+class PendingTransactionSource(BaseModel):
+    account_transfer_instruction: Optional[PendingTransactionSourceAccountTransferInstruction]
+    """A Account Transfer Instruction object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `account_transfer_instruction`.
+    """
+
+    ach_transfer_instruction: Optional[PendingTransactionSourceACHTransferInstruction]
+    """A ACH Transfer Instruction object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `ach_transfer_instruction`.
+    """
+
+    card_authorization: Optional[PendingTransactionSourceCardAuthorization]
+    """A Card Authorization object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `card_authorization`.
+    """
+
+    category: Literal[
+        "account_transfer_instruction",
+        "ach_transfer_instruction",
+        "card_authorization",
+        "check_deposit_instruction",
+        "check_transfer_instruction",
+        "inbound_funds_hold",
+        "real_time_payments_transfer_instruction",
+        "wire_transfer_instruction",
+        "other",
+    ]
+    """The type of transaction that took place.
+
+    We may add additional possible values for this enum over time; your application
+    should be able to handle such additions gracefully.
+    """
+
+    check_deposit_instruction: Optional[PendingTransactionSourceCheckDepositInstruction]
+    """A Check Deposit Instruction object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `check_deposit_instruction`.
+    """
+
+    check_transfer_instruction: Optional[PendingTransactionSourceCheckTransferInstruction]
+    """A Check Transfer Instruction object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `check_transfer_instruction`.
+    """
+
+    inbound_funds_hold: Optional[PendingTransactionSourceInboundFundsHold]
+    """A Inbound Funds Hold object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `inbound_funds_hold`.
+    """
+
+    real_time_payments_transfer_instruction: Optional[PendingTransactionSourceRealTimePaymentsTransferInstruction]
+    """A Real Time Payments Transfer Instruction object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `real_time_payments_transfer_instruction`.
+    """
+
+    wire_transfer_instruction: Optional[PendingTransactionSourceWireTransferInstruction]
+    """A Wire Transfer Instruction object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `wire_transfer_instruction`.
+    """
+
+
+class PendingTransaction(BaseModel):
+    id: str
+    """The Pending Transaction identifier."""
+
+    account_id: str
+    """The identifier for the account this Pending Transaction belongs to."""
+
+    amount: int
+    """The Pending Transaction amount in the minor unit of its currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    completed_at: Optional[datetime]
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the Pending
+    Transaction was completed.
+    """
+
+    created_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the Pending
+    Transaction occured.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the Pending
+    Transaction's currency. This will match the currency on the Pending
+    Transcation's Account.
+    """
+
+    description: str
+    """
+    For a Pending Transaction related to a transfer, this is the description you
+    provide. For a Pending Transaction related to a payment, this is the description
+    the vendor provides.
+    """
+
+    route_id: Optional[str]
+    """The identifier for the route this Pending Transaction came through.
+
+    Routes are things like cards and ACH details.
+    """
+
+    route_type: Optional[Literal["account_number", "card"]]
+    """The type of the route this Pending Transaction came through."""
+
+    source: PendingTransactionSource
+    """
+    This is an object giving more details on the network-level event that caused the
+    Pending Transaction. For example, for a card transaction this lists the
+    merchant's industry and location.
+    """
+
+    status: Literal["pending", "complete"]
+    """
+    Whether the Pending Transaction has been confirmed and has an associated
+    Transaction.
+    """
+
+    type: Literal["pending_transaction"]
+    """A constant representing the object's type.
+
+    For this resource it will always be `pending_transaction`.
+    """
+
+
 class CardAuthorizationSimulation(BaseModel):
     declined_transaction: Optional[DeclinedTransaction]
     """
     If the authorization attempt fails, this will contain the resulting
     [Declined Transaction](#declined-transactions) object. The Declined
     Transaction's `source` will be of `category: card_decline`.
     """
```

### Comparing `increase-0.7.1/src/increase/types/simulations/card_authorize_params.py` & `increase-0.8.0/src/increase/types/simulations/card_authorize_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/simulations/card_settlement_params.py` & `increase-0.8.0/src/increase/types/simulations/card_settlement_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/simulations/digital_wallet_token_request_create_response.py` & `increase-0.8.0/src/increase/types/simulations/digital_wallet_token_request_create_response.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py` & `increase-0.8.0/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,58 +5,514 @@
 from typing_extensions import Literal
 
 from ...types import shared
 from ..._models import BaseModel
 
 __all__ = [
     "InboundRealTimePaymentsTransferSimulationResult",
+    "DeclinedTransaction",
+    "DeclinedTransactionSource",
+    "DeclinedTransactionSourceACHDecline",
+    "DeclinedTransactionSourceCardDecline",
+    "DeclinedTransactionSourceCardDeclineNetworkDetails",
+    "DeclinedTransactionSourceCardDeclineNetworkDetailsVisa",
+    "DeclinedTransactionSourceCheckDecline",
+    "DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline",
+    "DeclinedTransactionSourceInternationalACHDecline",
+    "DeclinedTransactionSourceWireDecline",
     "Transaction",
     "TransactionSource",
     "TransactionSourceAccountTransferIntention",
     "TransactionSourceACHTransferIntention",
     "TransactionSourceACHTransferRejection",
     "TransactionSourceACHTransferReturn",
     "TransactionSourceCardDisputeAcceptance",
     "TransactionSourceCardRefund",
-    "TransactionSourceCardSettlement",
     "TransactionSourceCardRevenuePayment",
+    "TransactionSourceCardSettlement",
     "TransactionSourceCheckDepositAcceptance",
     "TransactionSourceCheckDepositReturn",
+    "TransactionSourceCheckTransferDeposit",
     "TransactionSourceCheckTransferIntention",
-    "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferRejection",
+    "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferStopPaymentRequest",
     "TransactionSourceFeePayment",
     "TransactionSourceInboundACHTransfer",
     "TransactionSourceInboundCheck",
     "TransactionSourceInboundInternationalACHTransfer",
     "TransactionSourceInboundRealTimePaymentsTransferConfirmation",
-    "TransactionSourceInboundWireDrawdownPaymentReversal",
     "TransactionSourceInboundWireDrawdownPayment",
+    "TransactionSourceInboundWireDrawdownPaymentReversal",
     "TransactionSourceInboundWireReversal",
     "TransactionSourceInboundWireTransfer",
     "TransactionSourceInterestPayment",
     "TransactionSourceInternalSource",
     "TransactionSourceRealTimePaymentsTransferAcknowledgement",
     "TransactionSourceSampleFunds",
     "TransactionSourceWireTransferIntention",
     "TransactionSourceWireTransferRejection",
-    "DeclinedTransaction",
-    "DeclinedTransactionSource",
-    "DeclinedTransactionSourceACHDecline",
-    "DeclinedTransactionSourceCardDecline",
-    "DeclinedTransactionSourceCardDeclineNetworkDetails",
-    "DeclinedTransactionSourceCardDeclineNetworkDetailsVisa",
-    "DeclinedTransactionSourceCheckDecline",
-    "DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline",
-    "DeclinedTransactionSourceInternationalACHDecline",
-    "DeclinedTransactionSourceWireDecline",
 ]
 
 
+class DeclinedTransactionSourceACHDecline(BaseModel):
+    amount: int
+    """The declined amount in the minor unit of the destination account currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    originator_company_descriptive_date: Optional[str]
+
+    originator_company_discretionary_data: Optional[str]
+
+    originator_company_id: str
+
+    originator_company_name: str
+
+    reason: Literal[
+        "ach_route_canceled",
+        "ach_route_disabled",
+        "breaches_limit",
+        "credit_entry_refused_by_receiver",
+        "duplicate_return",
+        "entity_not_active",
+        "group_locked",
+        "insufficient_funds",
+        "misrouted_return",
+        "no_ach_route",
+        "originator_request",
+        "transaction_not_allowed",
+    ]
+    """Why the ACH transfer was declined."""
+
+    receiver_id_number: Optional[str]
+
+    receiver_name: Optional[str]
+
+    trace_number: str
+
+
+class DeclinedTransactionSourceCardDeclineNetworkDetailsVisa(BaseModel):
+    electronic_commerce_indicator: Optional[
+        Literal[
+            "mail_phone_order",
+            "recurring",
+            "installment",
+            "unknown_mail_phone_order",
+            "secure_electronic_commerce",
+            "non_authenticated_security_transaction_at_3ds_capable_merchant",
+            "non_authenticated_security_transaction",
+            "non_secure_transaction",
+        ]
+    ]
+    """
+    For electronic commerce transactions, this identifies the level of security used
+    in obtaining the customer's payment credential. For mail or telephone order
+    transactions, identifies the type of mail or telephone order.
+    """
+
+    point_of_service_entry_mode: Optional[shared.PointOfServiceEntryMode]
+    """
+    The method used to enter the cardholder's primary account number and card
+    expiration date
+    """
+
+
+class DeclinedTransactionSourceCardDeclineNetworkDetails(BaseModel):
+    visa: DeclinedTransactionSourceCardDeclineNetworkDetailsVisa
+    """Fields specific to the `visa` network"""
+
+
+class DeclinedTransactionSourceCardDecline(BaseModel):
+    amount: int
+    """The declined amount in the minor unit of the destination account currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
+    account currency.
+    """
+
+    digital_wallet_token_id: Optional[str]
+    """
+    If the authorization was attempted using a Digital Wallet Token (such as an
+    Apple Pay purchase), the identifier of the token that was used.
+    """
+
+    merchant_acceptor_id: str
+    """
+    The merchant identifier (commonly abbreviated as MID) of the merchant the card
+    is transacting with.
+    """
+
+    merchant_category_code: Optional[str]
+    """
+    The Merchant Category Code (commonly abbreviated as MCC) of the merchant the
+    card is transacting with.
+    """
+
+    merchant_city: Optional[str]
+    """The city the merchant resides in."""
+
+    merchant_country: Optional[str]
+    """The country the merchant resides in."""
+
+    merchant_descriptor: str
+    """The merchant descriptor of the merchant the card is transacting with."""
+
+    merchant_state: Optional[str]
+    """The state the merchant resides in."""
+
+    network: Literal["visa"]
+    """The payment network used to process this card authorization"""
+
+    network_details: DeclinedTransactionSourceCardDeclineNetworkDetails
+    """Fields specific to the `network`"""
+
+    real_time_decision_id: Optional[str]
+    """
+    The identifier of the Real-Time Decision sent to approve or decline this
+    transaction.
+    """
+
+    reason: Literal[
+        "card_not_active",
+        "entity_not_active",
+        "group_locked",
+        "insufficient_funds",
+        "cvv2_mismatch",
+        "transaction_not_allowed",
+        "breaches_internal_limit",
+        "breaches_limit",
+        "webhook_declined",
+        "webhook_timed_out",
+        "declined_by_stand_in_processing",
+        "invalid_physical_card",
+        "missing_original_authorization",
+    ]
+    """Why the transaction was declined."""
+
+
+class DeclinedTransactionSourceCheckDecline(BaseModel):
+    amount: int
+    """The declined amount in the minor unit of the destination account currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    auxiliary_on_us: Optional[str]
+
+    reason: Literal[
+        "ach_route_canceled",
+        "ach_route_disabled",
+        "breaches_limit",
+        "entity_not_active",
+        "group_locked",
+        "insufficient_funds",
+        "unable_to_locate_account",
+        "not_our_item",
+        "unable_to_process",
+        "refer_to_image",
+        "stop_payment_requested",
+        "returned",
+        "duplicate_presentment",
+        "not_authorized",
+        "altered_or_fictitious",
+    ]
+    """Why the check was declined."""
+
+
+class DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline(BaseModel):
+    amount: int
+    """The declined amount in the minor unit of the destination account currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    creditor_name: str
+    """The name the sender of the transfer specified as the recipient of the transfer."""
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code of the declined
+    transfer's currency. This will always be "USD" for a Real Time Payments
+    transfer.
+    """
+
+    debtor_account_number: str
+    """The account number of the account that sent the transfer."""
+
+    debtor_name: str
+    """The name provided by the sender of the transfer."""
+
+    debtor_routing_number: str
+    """The routing number of the account that sent the transfer."""
+
+    reason: Literal[
+        "account_number_canceled",
+        "account_number_disabled",
+        "account_restricted",
+        "group_locked",
+        "entity_not_active",
+        "real_time_payments_not_enabled",
+    ]
+    """Why the transfer was declined."""
+
+    remittance_information: Optional[str]
+    """Additional information included with the transfer."""
+
+    transaction_identification: str
+    """The Real Time Payments network identification of the declined transfer."""
+
+
+class DeclinedTransactionSourceInternationalACHDecline(BaseModel):
+    amount: int
+    """The declined amount in the minor unit of the destination account currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    destination_country_code: str
+
+    destination_currency_code: str
+
+    foreign_exchange_indicator: str
+
+    foreign_exchange_reference: Optional[str]
+
+    foreign_exchange_reference_indicator: str
+
+    foreign_payment_amount: int
+
+    foreign_trace_number: Optional[str]
+
+    international_transaction_type_code: str
+
+    originating_currency_code: str
+
+    originating_depository_financial_institution_branch_country: str
+
+    originating_depository_financial_institution_id: str
+
+    originating_depository_financial_institution_id_qualifier: str
+
+    originating_depository_financial_institution_name: str
+
+    originator_city: str
+
+    originator_company_entry_description: str
+
+    originator_country: str
+
+    originator_identification: str
+
+    originator_name: str
+
+    originator_postal_code: Optional[str]
+
+    originator_state_or_province: Optional[str]
+
+    originator_street_address: str
+
+    payment_related_information: Optional[str]
+
+    payment_related_information2: Optional[str]
+
+    receiver_city: str
+
+    receiver_country: str
+
+    receiver_identification_number: Optional[str]
+
+    receiver_postal_code: Optional[str]
+
+    receiver_state_or_province: Optional[str]
+
+    receiver_street_address: str
+
+    receiving_company_or_individual_name: str
+
+    receiving_depository_financial_institution_country: str
+
+    receiving_depository_financial_institution_id: str
+
+    receiving_depository_financial_institution_id_qualifier: str
+
+    receiving_depository_financial_institution_name: str
+
+    trace_number: str
+
+
+class DeclinedTransactionSourceWireDecline(BaseModel):
+    amount: int
+    """The declined amount in the minor unit of the destination account currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    beneficiary_address_line1: Optional[str]
+
+    beneficiary_address_line2: Optional[str]
+
+    beneficiary_address_line3: Optional[str]
+
+    beneficiary_name: Optional[str]
+
+    beneficiary_reference: Optional[str]
+
+    description: str
+
+    input_message_accountability_data: Optional[str]
+
+    originator_address_line1: Optional[str]
+
+    originator_address_line2: Optional[str]
+
+    originator_address_line3: Optional[str]
+
+    originator_name: Optional[str]
+
+    originator_to_beneficiary_information_line1: Optional[str]
+
+    originator_to_beneficiary_information_line2: Optional[str]
+
+    originator_to_beneficiary_information_line3: Optional[str]
+
+    originator_to_beneficiary_information_line4: Optional[str]
+
+    reason: Literal[
+        "account_number_canceled",
+        "account_number_disabled",
+        "entity_not_active",
+        "group_locked",
+        "no_account_number",
+        "transaction_not_allowed",
+    ]
+    """Why the wire transfer was declined."""
+
+
+class DeclinedTransactionSource(BaseModel):
+    ach_decline: Optional[DeclinedTransactionSourceACHDecline]
+    """A ACH Decline object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `ach_decline`.
+    """
+
+    card_decline: Optional[DeclinedTransactionSourceCardDecline]
+    """A Card Decline object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `card_decline`.
+    """
+
+    category: Literal[
+        "ach_decline",
+        "card_decline",
+        "check_decline",
+        "inbound_real_time_payments_transfer_decline",
+        "international_ach_decline",
+        "wire_decline",
+        "other",
+    ]
+    """The type of decline that took place.
+
+    We may add additional possible values for this enum over time; your application
+    should be able to handle such additions gracefully.
+    """
+
+    check_decline: Optional[DeclinedTransactionSourceCheckDecline]
+    """A Check Decline object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `check_decline`.
+    """
+
+    inbound_real_time_payments_transfer_decline: Optional[
+        DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline
+    ]
+    """A Inbound Real Time Payments Transfer Decline object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `inbound_real_time_payments_transfer_decline`.
+    """
+
+    international_ach_decline: Optional[DeclinedTransactionSourceInternationalACHDecline]
+    """A International ACH Decline object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `international_ach_decline`.
+    """
+
+    wire_decline: Optional[DeclinedTransactionSourceWireDecline]
+    """A Wire Decline object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `wire_decline`.
+    """
+
+
+class DeclinedTransaction(BaseModel):
+    id: str
+    """The Declined Transaction identifier."""
+
+    account_id: str
+    """The identifier for the Account the Declined Transaction belongs to."""
+
+    amount: int
+    """The Declined Transaction amount in the minor unit of its currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    created_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the
+    Transaction occured.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the Declined
+    Transaction's currency. This will match the currency on the Declined
+    Transcation's Account.
+    """
+
+    description: str
+    """This is the description the vendor provides."""
+
+    route_id: Optional[str]
+    """The identifier for the route this Declined Transaction came through.
+
+    Routes are things like cards and ACH details.
+    """
+
+    route_type: Optional[Literal["account_number", "card"]]
+    """The type of the route this Declined Transaction came through."""
+
+    source: DeclinedTransactionSource
+    """
+    This is an object giving more details on the network-level event that caused the
+    Declined Transaction. For example, for a card transaction this lists the
+    merchant's industry and location. Note that for backwards compatibility reasons,
+    additional undocumented keys may appear in this object. These should be treated
+    as deprecated and will be removed in the future.
+    """
+
+    type: Literal["declined_transaction"]
+    """A constant representing the object's type.
+
+    For this resource it will always be `declined_transaction`.
+    """
+
+
 class TransactionSourceAccountTransferIntention(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -129,15 +585,14 @@
         "authorization_revoked_by_customer",
         "invalid_ach_routing_number",
         "file_record_edit_criteria",
         "enr_invalid_individual_name",
         "returned_per_odfi_request",
         "limited_participation_dfi",
         "incorrectly_coded_outbound_international_payment",
-        "other",
         "account_sold_to_another_dfi",
         "addenda_error",
         "beneficiary_or_account_holder_deceased",
         "customer_advised_not_within_authorization_terms",
         "corrected_return",
         "duplicate_entry",
         "duplicate_return",
@@ -207,29 +662,29 @@
     """
     The identifier of the Transaction that was created to return the disputed funds
     to your account.
     """
 
 
 class TransactionSourceCardRefund(BaseModel):
+    id: str
+    """The Card Refund identifier."""
+
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
     """
 
-    id: str
-    """The Card Refund identifier."""
-
     merchant_acceptor_id: Optional[str]
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
 
     merchant_category_code: str
@@ -250,15 +705,41 @@
     type: Literal["card_refund"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_refund`.
     """
 
 
+class TransactionSourceCardRevenuePayment(BaseModel):
+    amount: int
+    """The amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
+    currency.
+    """
+
+    period_end: datetime
+    """The end of the period for which this transaction paid interest."""
+
+    period_start: datetime
+    """The start of the period for which this transaction paid interest."""
+
+    transacted_on_account_id: Optional[str]
+    """The account the card belonged to."""
+
+
 class TransactionSourceCardSettlement(BaseModel):
+    id: str
+    """The Card Settlement identifier."""
+
     amount: int
     """The amount in the minor unit of the transaction's settlement currency.
 
     For dollars, for example, this is cents.
     """
 
     card_authorization: Optional[str]
@@ -269,17 +750,14 @@
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's settlement currency.
     """
 
-    id: str
-    """The Card Settlement identifier."""
-
     merchant_acceptor_id: Optional[str]
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
 
     merchant_category_code: str
@@ -312,37 +790,14 @@
     type: Literal["card_settlement"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_settlement`.
     """
 
 
-class TransactionSourceCardRevenuePayment(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
-    currency.
-    """
-
-    period_end: datetime
-    """The end of the period for which this transaction paid interest."""
-
-    period_start: datetime
-    """The start of the period for which this transaction paid interest."""
-
-    transacted_on_account_id: Optional[str]
-    """The account the card belonged to."""
-
-
 class TransactionSourceCheckDepositAcceptance(BaseModel):
     account_number: str
     """The account number printed on the check."""
 
     amount: int
     """The amount to be deposited in the minor unit of the transaction's currency.
 
@@ -415,46 +870,74 @@
     transaction_id: str
     """
     The identifier of the transaction that reversed the original check deposit
     transaction.
     """
 
 
+class TransactionSourceCheckTransferDeposit(BaseModel):
+    back_image_file_id: Optional[str]
+    """
+    The identifier of the API File object containing an image of the back of the
+    deposited check.
+    """
+
+    deposited_at: datetime
+    """When the check was deposited."""
+
+    front_image_file_id: Optional[str]
+    """
+    The identifier of the API File object containing an image of the front of the
+    deposited check.
+    """
+
+    type: Literal["check_transfer_deposit"]
+    """A constant representing the object's type.
+
+    For this resource it will always be `check_transfer_deposit`.
+    """
+
+
 class TransactionSourceCheckTransferIntention(BaseModel):
-    address_city: str
+    address_city: Optional[str]
     """The city of the check's destination."""
 
-    address_line1: str
+    address_line1: Optional[str]
     """The street address of the check's destination."""
 
     address_line2: Optional[str]
     """The second line of the address of the check's destination."""
 
-    address_state: str
+    address_state: Optional[str]
     """The state of the check's destination."""
 
-    address_zip: str
+    address_zip: Optional[str]
     """The postal code of the check's destination."""
 
     amount: int
     """The transfer amount in USD cents."""
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the check's
     currency.
     """
 
-    recipient_name: str
+    recipient_name: Optional[str]
     """The name that will be printed on the check."""
 
     transfer_id: str
     """The identifier of the Check Transfer with which this is associated."""
 
 
+class TransactionSourceCheckTransferRejection(BaseModel):
+    transfer_id: str
+    """The identifier of the Check Transfer that led to this Transaction."""
+
+
 class TransactionSourceCheckTransferReturn(BaseModel):
     file_id: Optional[str]
     """If available, a document with additional information about the return."""
 
     reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"]
     """The reason why the check was returned."""
 
@@ -470,19 +953,14 @@
     returned check.
     """
 
     transfer_id: str
     """The identifier of the returned Check Transfer."""
 
 
-class TransactionSourceCheckTransferRejection(BaseModel):
-    transfer_id: str
-    """The identifier of the Check Transfer that led to this Transaction."""
-
-
 class TransactionSourceCheckTransferStopPaymentRequest(BaseModel):
     requested_at: datetime
     """The time the stop-payment was requested."""
 
     transaction_id: str
     """The transaction ID of the corresponding credit transaction."""
 
@@ -660,46 +1138,14 @@
     remittance_information: Optional[str]
     """Additional information included with the transfer."""
 
     transaction_identification: str
     """The Real Time Payments network identification of the transfer"""
 
 
-class TransactionSourceInboundWireDrawdownPaymentReversal(BaseModel):
-    amount: int
-    """The amount that was reversed."""
-
-    description: str
-    """The description on the reversal message from Fedwire."""
-
-    input_cycle_date: date
-    """The Fedwire cycle date for the wire reversal."""
-
-    input_message_accountability_data: str
-    """The Fedwire transaction identifier."""
-
-    input_sequence_number: str
-    """The Fedwire sequence number."""
-
-    input_source: str
-    """The Fedwire input source identifier."""
-
-    previous_message_input_cycle_date: date
-    """The Fedwire cycle date for the wire transfer that was reversed."""
-
-    previous_message_input_message_accountability_data: str
-    """The Fedwire transaction identifier for the wire transfer that was reversed."""
-
-    previous_message_input_sequence_number: str
-    """The Fedwire sequence number for the wire transfer that was reversed."""
-
-    previous_message_input_source: str
-    """The Fedwire input source identifier for the wire transfer that was reversed."""
-
-
 class TransactionSourceInboundWireDrawdownPayment(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -724,14 +1170,46 @@
     originator_address_line3: Optional[str]
 
     originator_name: Optional[str]
 
     originator_to_beneficiary_information: Optional[str]
 
 
+class TransactionSourceInboundWireDrawdownPaymentReversal(BaseModel):
+    amount: int
+    """The amount that was reversed."""
+
+    description: str
+    """The description on the reversal message from Fedwire."""
+
+    input_cycle_date: date
+    """The Fedwire cycle date for the wire reversal."""
+
+    input_message_accountability_data: str
+    """The Fedwire transaction identifier."""
+
+    input_sequence_number: str
+    """The Fedwire sequence number."""
+
+    input_source: str
+    """The Fedwire input source identifier."""
+
+    previous_message_input_cycle_date: date
+    """The Fedwire cycle date for the wire transfer that was reversed."""
+
+    previous_message_input_message_accountability_data: str
+    """The Fedwire transaction identifier for the wire transfer that was reversed."""
+
+    previous_message_input_sequence_number: str
+    """The Fedwire sequence number for the wire transfer that was reversed."""
+
+    previous_message_input_source: str
+    """The Fedwire input source identifier for the wire transfer that was reversed."""
+
+
 class TransactionSourceInboundWireReversal(BaseModel):
     amount: int
     """The amount that was reversed."""
 
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
@@ -975,30 +1453,31 @@
     category: Literal[
         "account_transfer_intention",
         "ach_transfer_intention",
         "ach_transfer_rejection",
         "ach_transfer_return",
         "card_dispute_acceptance",
         "card_refund",
-        "card_settlement",
         "card_revenue_payment",
+        "card_settlement",
         "check_deposit_acceptance",
         "check_deposit_return",
+        "check_transfer_deposit",
         "check_transfer_intention",
-        "check_transfer_return",
         "check_transfer_rejection",
+        "check_transfer_return",
         "check_transfer_stop_payment_request",
         "fee_payment",
         "inbound_ach_transfer",
         "inbound_ach_transfer_return_intention",
         "inbound_check",
         "inbound_international_ach_transfer",
         "inbound_real_time_payments_transfer_confirmation",
-        "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_drawdown_payment",
+        "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_reversal",
         "inbound_wire_transfer",
         "interest_payment",
         "internal_source",
         "real_time_payments_transfer_acknowledgement",
         "sample_funds",
         "wire_transfer_intention",
@@ -1021,14 +1500,21 @@
     check_deposit_return: Optional[TransactionSourceCheckDepositReturn]
     """A Check Deposit Return object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_deposit_return`.
     """
 
+    check_transfer_deposit: Optional[TransactionSourceCheckTransferDeposit]
+    """A Check Transfer Deposit object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `check_transfer_deposit`.
+    """
+
     check_transfer_intention: Optional[TransactionSourceCheckTransferIntention]
     """A Check Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_transfer_intention`.
     """
 
@@ -1158,14 +1644,17 @@
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_transfer_rejection`.
     """
 
 
 class Transaction(BaseModel):
+    id: str
+    """The Transaction identifier."""
+
     account_id: str
     """The identifier for the Account the Transaction belongs to."""
 
     amount: int
     """The Transaction amount in the minor unit of its currency.
 
     For dollars, for example, this is cents.
@@ -1187,17 +1676,14 @@
     description: str
     """For a Transaction related to a transfer, this is the description you provide.
 
     For a Transaction related to a payment, this is the description the vendor
     provides.
     """
 
-    id: str
-    """The Transaction identifier."""
-
     route_id: Optional[str]
     """The identifier for the route this Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
     route_type: Optional[Literal["account_number", "card"]]
@@ -1214,469 +1700,14 @@
     type: Literal["transaction"]
     """A constant representing the object's type.
 
     For this resource it will always be `transaction`.
     """
 
 
-class DeclinedTransactionSourceACHDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    originator_company_descriptive_date: Optional[str]
-
-    originator_company_discretionary_data: Optional[str]
-
-    originator_company_id: str
-
-    originator_company_name: str
-
-    reason: Literal[
-        "ach_route_canceled",
-        "ach_route_disabled",
-        "breaches_limit",
-        "credit_entry_refused_by_receiver",
-        "duplicate_return",
-        "entity_not_active",
-        "group_locked",
-        "insufficient_funds",
-        "misrouted_return",
-        "no_ach_route",
-        "originator_request",
-        "transaction_not_allowed",
-    ]
-    """Why the ACH transfer was declined."""
-
-    receiver_id_number: Optional[str]
-
-    receiver_name: Optional[str]
-
-    trace_number: str
-
-
-class DeclinedTransactionSourceCardDeclineNetworkDetailsVisa(BaseModel):
-    electronic_commerce_indicator: Optional[
-        Literal[
-            "mail_phone_order",
-            "recurring",
-            "installment",
-            "unknown_mail_phone_order",
-            "secure_electronic_commerce",
-            "non_authenticated_security_transaction_at_3ds_capable_merchant",
-            "non_authenticated_security_transaction",
-            "non_secure_transaction",
-        ]
-    ]
-    """
-    For electronic commerce transactions, this identifies the level of security used
-    in obtaining the customer's payment credential. For mail or telephone order
-    transactions, identifies the type of mail or telephone order.
-    """
-
-    point_of_service_entry_mode: Optional[shared.PointOfServiceEntryMode]
-    """
-    The method used to enter the cardholder's primary account number and card
-    expiration date
-    """
-
-
-class DeclinedTransactionSourceCardDeclineNetworkDetails(BaseModel):
-    visa: DeclinedTransactionSourceCardDeclineNetworkDetailsVisa
-    """Fields specific to the `visa` network"""
-
-
-class DeclinedTransactionSourceCardDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
-    account currency.
-    """
-
-    digital_wallet_token_id: Optional[str]
-    """
-    If the authorization was attempted using a Digital Wallet Token (such as an
-    Apple Pay purchase), the identifier of the token that was used.
-    """
-
-    merchant_acceptor_id: str
-    """
-    The merchant identifier (commonly abbreviated as MID) of the merchant the card
-    is transacting with.
-    """
-
-    merchant_category_code: Optional[str]
-    """
-    The Merchant Category Code (commonly abbreviated as MCC) of the merchant the
-    card is transacting with.
-    """
-
-    merchant_city: Optional[str]
-    """The city the merchant resides in."""
-
-    merchant_country: Optional[str]
-    """The country the merchant resides in."""
-
-    merchant_descriptor: str
-    """The merchant descriptor of the merchant the card is transacting with."""
-
-    merchant_state: Optional[str]
-    """The state the merchant resides in."""
-
-    network: Literal["visa"]
-    """The payment network used to process this card authorization"""
-
-    network_details: DeclinedTransactionSourceCardDeclineNetworkDetails
-    """Fields specific to the `network`"""
-
-    real_time_decision_id: Optional[str]
-    """
-    The identifier of the Real-Time Decision sent to approve or decline this
-    transaction.
-    """
-
-    reason: Literal[
-        "card_not_active",
-        "entity_not_active",
-        "group_locked",
-        "insufficient_funds",
-        "cvv2_mismatch",
-        "transaction_not_allowed",
-        "breaches_internal_limit",
-        "breaches_limit",
-        "webhook_declined",
-        "webhook_timed_out",
-        "declined_by_stand_in_processing",
-        "invalid_physical_card",
-        "missing_original_authorization",
-    ]
-    """Why the transaction was declined."""
-
-
-class DeclinedTransactionSourceCheckDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    auxiliary_on_us: Optional[str]
-
-    reason: Literal[
-        "ach_route_canceled",
-        "ach_route_disabled",
-        "breaches_limit",
-        "entity_not_active",
-        "group_locked",
-        "insufficient_funds",
-        "unable_to_locate_account",
-        "not_our_item",
-        "unable_to_process",
-        "refer_to_image",
-        "stop_payment_requested",
-        "returned",
-        "duplicate_presentment",
-        "not_authorized",
-        "altered_or_fictitious",
-    ]
-    """Why the check was declined."""
-
-
-class DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    creditor_name: str
-    """The name the sender of the transfer specified as the recipient of the transfer."""
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code of the declined
-    transfer's currency. This will always be "USD" for a Real Time Payments
-    transfer.
-    """
-
-    debtor_account_number: str
-    """The account number of the account that sent the transfer."""
-
-    debtor_name: str
-    """The name provided by the sender of the transfer."""
-
-    debtor_routing_number: str
-    """The routing number of the account that sent the transfer."""
-
-    reason: Literal[
-        "account_number_canceled",
-        "account_number_disabled",
-        "account_restricted",
-        "group_locked",
-        "entity_not_active",
-        "real_time_payments_not_enabled",
-    ]
-    """Why the transfer was declined."""
-
-    remittance_information: Optional[str]
-    """Additional information included with the transfer."""
-
-    transaction_identification: str
-    """The Real Time Payments network identification of the declined transfer."""
-
-
-class DeclinedTransactionSourceInternationalACHDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    destination_country_code: str
-
-    destination_currency_code: str
-
-    foreign_exchange_indicator: str
-
-    foreign_exchange_reference: Optional[str]
-
-    foreign_exchange_reference_indicator: str
-
-    foreign_payment_amount: int
-
-    foreign_trace_number: Optional[str]
-
-    international_transaction_type_code: str
-
-    originating_currency_code: str
-
-    originating_depository_financial_institution_branch_country: str
-
-    originating_depository_financial_institution_id: str
-
-    originating_depository_financial_institution_id_qualifier: str
-
-    originating_depository_financial_institution_name: str
-
-    originator_city: str
-
-    originator_company_entry_description: str
-
-    originator_country: str
-
-    originator_identification: str
-
-    originator_name: str
-
-    originator_postal_code: Optional[str]
-
-    originator_state_or_province: Optional[str]
-
-    originator_street_address: str
-
-    payment_related_information: Optional[str]
-
-    payment_related_information2: Optional[str]
-
-    receiver_city: str
-
-    receiver_country: str
-
-    receiver_identification_number: Optional[str]
-
-    receiver_postal_code: Optional[str]
-
-    receiver_state_or_province: Optional[str]
-
-    receiver_street_address: str
-
-    receiving_company_or_individual_name: str
-
-    receiving_depository_financial_institution_country: str
-
-    receiving_depository_financial_institution_id: str
-
-    receiving_depository_financial_institution_id_qualifier: str
-
-    receiving_depository_financial_institution_name: str
-
-    trace_number: str
-
-
-class DeclinedTransactionSourceWireDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    beneficiary_address_line1: Optional[str]
-
-    beneficiary_address_line2: Optional[str]
-
-    beneficiary_address_line3: Optional[str]
-
-    beneficiary_name: Optional[str]
-
-    beneficiary_reference: Optional[str]
-
-    description: str
-
-    input_message_accountability_data: Optional[str]
-
-    originator_address_line1: Optional[str]
-
-    originator_address_line2: Optional[str]
-
-    originator_address_line3: Optional[str]
-
-    originator_name: Optional[str]
-
-    originator_to_beneficiary_information_line1: Optional[str]
-
-    originator_to_beneficiary_information_line2: Optional[str]
-
-    originator_to_beneficiary_information_line3: Optional[str]
-
-    originator_to_beneficiary_information_line4: Optional[str]
-
-    reason: Literal[
-        "account_number_canceled",
-        "account_number_disabled",
-        "entity_not_active",
-        "group_locked",
-        "no_account_number",
-        "transaction_not_allowed",
-    ]
-    """Why the wire transfer was declined."""
-
-
-class DeclinedTransactionSource(BaseModel):
-    ach_decline: Optional[DeclinedTransactionSourceACHDecline]
-    """A ACH Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_decline`.
-    """
-
-    card_decline: Optional[DeclinedTransactionSourceCardDecline]
-    """A Card Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_decline`.
-    """
-
-    category: Literal[
-        "ach_decline",
-        "card_decline",
-        "check_decline",
-        "inbound_real_time_payments_transfer_decline",
-        "international_ach_decline",
-        "wire_decline",
-        "other",
-    ]
-    """The type of decline that took place.
-
-    We may add additional possible values for this enum over time; your application
-    should be able to handle such additions gracefully.
-    """
-
-    check_decline: Optional[DeclinedTransactionSourceCheckDecline]
-    """A Check Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `check_decline`.
-    """
-
-    inbound_real_time_payments_transfer_decline: Optional[
-        DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline
-    ]
-    """A Inbound Real Time Payments Transfer Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `inbound_real_time_payments_transfer_decline`.
-    """
-
-    international_ach_decline: Optional[DeclinedTransactionSourceInternationalACHDecline]
-    """A International ACH Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `international_ach_decline`.
-    """
-
-    wire_decline: Optional[DeclinedTransactionSourceWireDecline]
-    """A Wire Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_decline`.
-    """
-
-
-class DeclinedTransaction(BaseModel):
-    account_id: str
-    """The identifier for the Account the Declined Transaction belongs to."""
-
-    amount: int
-    """The Declined Transaction amount in the minor unit of its currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    created_at: datetime
-    """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the
-    Transaction occured.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the Declined
-    Transaction's currency. This will match the currency on the Declined
-    Transcation's Account.
-    """
-
-    description: str
-    """This is the description the vendor provides."""
-
-    id: str
-    """The Declined Transaction identifier."""
-
-    route_id: Optional[str]
-    """The identifier for the route this Declined Transaction came through.
-
-    Routes are things like cards and ACH details.
-    """
-
-    route_type: Optional[Literal["account_number", "card"]]
-    """The type of the route this Declined Transaction came through."""
-
-    source: DeclinedTransactionSource
-    """
-    This is an object giving more details on the network-level event that caused the
-    Declined Transaction. For example, for a card transaction this lists the
-    merchant's industry and location. Note that for backwards compatibility reasons,
-    additional undocumented keys may appear in this object. These should be treated
-    as deprecated and will be removed in the future.
-    """
-
-    type: Literal["declined_transaction"]
-    """A constant representing the object's type.
-
-    For this resource it will always be `declined_transaction`.
-    """
-
-
 class InboundRealTimePaymentsTransferSimulationResult(BaseModel):
     declined_transaction: Optional[DeclinedTransaction]
     """
     If the Real Time Payments Transfer attempt fails, this will contain the
     resulting [Declined Transaction](#declined-transactions) object. The Declined
     Transaction's `source` will be of
     `category: inbound_real_time_payments_transfer_decline`.
```

### Comparing `increase-0.7.1/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py` & `increase-0.8.0/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/simulations/interest_payment_simulation_result.py` & `increase-0.8.0/src/increase/types/simulations/interest_payment_simulation_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,29 +12,30 @@
     "TransactionSource",
     "TransactionSourceAccountTransferIntention",
     "TransactionSourceACHTransferIntention",
     "TransactionSourceACHTransferRejection",
     "TransactionSourceACHTransferReturn",
     "TransactionSourceCardDisputeAcceptance",
     "TransactionSourceCardRefund",
-    "TransactionSourceCardSettlement",
     "TransactionSourceCardRevenuePayment",
+    "TransactionSourceCardSettlement",
     "TransactionSourceCheckDepositAcceptance",
     "TransactionSourceCheckDepositReturn",
+    "TransactionSourceCheckTransferDeposit",
     "TransactionSourceCheckTransferIntention",
-    "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferRejection",
+    "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferStopPaymentRequest",
     "TransactionSourceFeePayment",
     "TransactionSourceInboundACHTransfer",
     "TransactionSourceInboundCheck",
     "TransactionSourceInboundInternationalACHTransfer",
     "TransactionSourceInboundRealTimePaymentsTransferConfirmation",
-    "TransactionSourceInboundWireDrawdownPaymentReversal",
     "TransactionSourceInboundWireDrawdownPayment",
+    "TransactionSourceInboundWireDrawdownPaymentReversal",
     "TransactionSourceInboundWireReversal",
     "TransactionSourceInboundWireTransfer",
     "TransactionSourceInterestPayment",
     "TransactionSourceInternalSource",
     "TransactionSourceRealTimePaymentsTransferAcknowledgement",
     "TransactionSourceSampleFunds",
     "TransactionSourceWireTransferIntention",
@@ -118,15 +119,14 @@
         "authorization_revoked_by_customer",
         "invalid_ach_routing_number",
         "file_record_edit_criteria",
         "enr_invalid_individual_name",
         "returned_per_odfi_request",
         "limited_participation_dfi",
         "incorrectly_coded_outbound_international_payment",
-        "other",
         "account_sold_to_another_dfi",
         "addenda_error",
         "beneficiary_or_account_holder_deceased",
         "customer_advised_not_within_authorization_terms",
         "corrected_return",
         "duplicate_entry",
         "duplicate_return",
@@ -196,29 +196,29 @@
     """
     The identifier of the Transaction that was created to return the disputed funds
     to your account.
     """
 
 
 class TransactionSourceCardRefund(BaseModel):
+    id: str
+    """The Card Refund identifier."""
+
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
     """
 
-    id: str
-    """The Card Refund identifier."""
-
     merchant_acceptor_id: Optional[str]
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
 
     merchant_category_code: str
@@ -239,15 +239,41 @@
     type: Literal["card_refund"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_refund`.
     """
 
 
+class TransactionSourceCardRevenuePayment(BaseModel):
+    amount: int
+    """The amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
+    currency.
+    """
+
+    period_end: datetime
+    """The end of the period for which this transaction paid interest."""
+
+    period_start: datetime
+    """The start of the period for which this transaction paid interest."""
+
+    transacted_on_account_id: Optional[str]
+    """The account the card belonged to."""
+
+
 class TransactionSourceCardSettlement(BaseModel):
+    id: str
+    """The Card Settlement identifier."""
+
     amount: int
     """The amount in the minor unit of the transaction's settlement currency.
 
     For dollars, for example, this is cents.
     """
 
     card_authorization: Optional[str]
@@ -258,17 +284,14 @@
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's settlement currency.
     """
 
-    id: str
-    """The Card Settlement identifier."""
-
     merchant_acceptor_id: Optional[str]
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
 
     merchant_category_code: str
@@ -301,37 +324,14 @@
     type: Literal["card_settlement"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_settlement`.
     """
 
 
-class TransactionSourceCardRevenuePayment(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
-    currency.
-    """
-
-    period_end: datetime
-    """The end of the period for which this transaction paid interest."""
-
-    period_start: datetime
-    """The start of the period for which this transaction paid interest."""
-
-    transacted_on_account_id: Optional[str]
-    """The account the card belonged to."""
-
-
 class TransactionSourceCheckDepositAcceptance(BaseModel):
     account_number: str
     """The account number printed on the check."""
 
     amount: int
     """The amount to be deposited in the minor unit of the transaction's currency.
 
@@ -404,46 +404,74 @@
     transaction_id: str
     """
     The identifier of the transaction that reversed the original check deposit
     transaction.
     """
 
 
+class TransactionSourceCheckTransferDeposit(BaseModel):
+    back_image_file_id: Optional[str]
+    """
+    The identifier of the API File object containing an image of the back of the
+    deposited check.
+    """
+
+    deposited_at: datetime
+    """When the check was deposited."""
+
+    front_image_file_id: Optional[str]
+    """
+    The identifier of the API File object containing an image of the front of the
+    deposited check.
+    """
+
+    type: Literal["check_transfer_deposit"]
+    """A constant representing the object's type.
+
+    For this resource it will always be `check_transfer_deposit`.
+    """
+
+
 class TransactionSourceCheckTransferIntention(BaseModel):
-    address_city: str
+    address_city: Optional[str]
     """The city of the check's destination."""
 
-    address_line1: str
+    address_line1: Optional[str]
     """The street address of the check's destination."""
 
     address_line2: Optional[str]
     """The second line of the address of the check's destination."""
 
-    address_state: str
+    address_state: Optional[str]
     """The state of the check's destination."""
 
-    address_zip: str
+    address_zip: Optional[str]
     """The postal code of the check's destination."""
 
     amount: int
     """The transfer amount in USD cents."""
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the check's
     currency.
     """
 
-    recipient_name: str
+    recipient_name: Optional[str]
     """The name that will be printed on the check."""
 
     transfer_id: str
     """The identifier of the Check Transfer with which this is associated."""
 
 
+class TransactionSourceCheckTransferRejection(BaseModel):
+    transfer_id: str
+    """The identifier of the Check Transfer that led to this Transaction."""
+
+
 class TransactionSourceCheckTransferReturn(BaseModel):
     file_id: Optional[str]
     """If available, a document with additional information about the return."""
 
     reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"]
     """The reason why the check was returned."""
 
@@ -459,19 +487,14 @@
     returned check.
     """
 
     transfer_id: str
     """The identifier of the returned Check Transfer."""
 
 
-class TransactionSourceCheckTransferRejection(BaseModel):
-    transfer_id: str
-    """The identifier of the Check Transfer that led to this Transaction."""
-
-
 class TransactionSourceCheckTransferStopPaymentRequest(BaseModel):
     requested_at: datetime
     """The time the stop-payment was requested."""
 
     transaction_id: str
     """The transaction ID of the corresponding credit transaction."""
 
@@ -649,46 +672,14 @@
     remittance_information: Optional[str]
     """Additional information included with the transfer."""
 
     transaction_identification: str
     """The Real Time Payments network identification of the transfer"""
 
 
-class TransactionSourceInboundWireDrawdownPaymentReversal(BaseModel):
-    amount: int
-    """The amount that was reversed."""
-
-    description: str
-    """The description on the reversal message from Fedwire."""
-
-    input_cycle_date: date
-    """The Fedwire cycle date for the wire reversal."""
-
-    input_message_accountability_data: str
-    """The Fedwire transaction identifier."""
-
-    input_sequence_number: str
-    """The Fedwire sequence number."""
-
-    input_source: str
-    """The Fedwire input source identifier."""
-
-    previous_message_input_cycle_date: date
-    """The Fedwire cycle date for the wire transfer that was reversed."""
-
-    previous_message_input_message_accountability_data: str
-    """The Fedwire transaction identifier for the wire transfer that was reversed."""
-
-    previous_message_input_sequence_number: str
-    """The Fedwire sequence number for the wire transfer that was reversed."""
-
-    previous_message_input_source: str
-    """The Fedwire input source identifier for the wire transfer that was reversed."""
-
-
 class TransactionSourceInboundWireDrawdownPayment(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -713,14 +704,46 @@
     originator_address_line3: Optional[str]
 
     originator_name: Optional[str]
 
     originator_to_beneficiary_information: Optional[str]
 
 
+class TransactionSourceInboundWireDrawdownPaymentReversal(BaseModel):
+    amount: int
+    """The amount that was reversed."""
+
+    description: str
+    """The description on the reversal message from Fedwire."""
+
+    input_cycle_date: date
+    """The Fedwire cycle date for the wire reversal."""
+
+    input_message_accountability_data: str
+    """The Fedwire transaction identifier."""
+
+    input_sequence_number: str
+    """The Fedwire sequence number."""
+
+    input_source: str
+    """The Fedwire input source identifier."""
+
+    previous_message_input_cycle_date: date
+    """The Fedwire cycle date for the wire transfer that was reversed."""
+
+    previous_message_input_message_accountability_data: str
+    """The Fedwire transaction identifier for the wire transfer that was reversed."""
+
+    previous_message_input_sequence_number: str
+    """The Fedwire sequence number for the wire transfer that was reversed."""
+
+    previous_message_input_source: str
+    """The Fedwire input source identifier for the wire transfer that was reversed."""
+
+
 class TransactionSourceInboundWireReversal(BaseModel):
     amount: int
     """The amount that was reversed."""
 
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
@@ -964,30 +987,31 @@
     category: Literal[
         "account_transfer_intention",
         "ach_transfer_intention",
         "ach_transfer_rejection",
         "ach_transfer_return",
         "card_dispute_acceptance",
         "card_refund",
-        "card_settlement",
         "card_revenue_payment",
+        "card_settlement",
         "check_deposit_acceptance",
         "check_deposit_return",
+        "check_transfer_deposit",
         "check_transfer_intention",
-        "check_transfer_return",
         "check_transfer_rejection",
+        "check_transfer_return",
         "check_transfer_stop_payment_request",
         "fee_payment",
         "inbound_ach_transfer",
         "inbound_ach_transfer_return_intention",
         "inbound_check",
         "inbound_international_ach_transfer",
         "inbound_real_time_payments_transfer_confirmation",
-        "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_drawdown_payment",
+        "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_reversal",
         "inbound_wire_transfer",
         "interest_payment",
         "internal_source",
         "real_time_payments_transfer_acknowledgement",
         "sample_funds",
         "wire_transfer_intention",
@@ -1010,14 +1034,21 @@
     check_deposit_return: Optional[TransactionSourceCheckDepositReturn]
     """A Check Deposit Return object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_deposit_return`.
     """
 
+    check_transfer_deposit: Optional[TransactionSourceCheckTransferDeposit]
+    """A Check Transfer Deposit object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `check_transfer_deposit`.
+    """
+
     check_transfer_intention: Optional[TransactionSourceCheckTransferIntention]
     """A Check Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_transfer_intention`.
     """
 
@@ -1147,14 +1178,17 @@
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_transfer_rejection`.
     """
 
 
 class Transaction(BaseModel):
+    id: str
+    """The Transaction identifier."""
+
     account_id: str
     """The identifier for the Account the Transaction belongs to."""
 
     amount: int
     """The Transaction amount in the minor unit of its currency.
 
     For dollars, for example, this is cents.
@@ -1176,17 +1210,14 @@
     description: str
     """For a Transaction related to a transfer, this is the description you provide.
 
     For a Transaction related to a payment, this is the description the vendor
     provides.
     """
 
-    id: str
-    """The Transaction identifier."""
-
     route_id: Optional[str]
     """The identifier for the route this Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
     route_type: Optional[Literal["account_number", "card"]]
```

### Comparing `increase-0.7.1/src/increase/types/simulations/real_time_payments_transfer_complete_params.py` & `increase-0.8.0/src/increase/types/simulations/real_time_payments_transfer_complete_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py` & `increase-0.8.0/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/simulations/wire_transfer_create_inbound_params.py` & `increase-0.8.0/src/increase/types/simulations/wire_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/simulations/wire_transfer_simulation.py` & `increase-0.8.0/src/increase/types/simulations/wire_transfer_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,29 +12,30 @@
     "TransactionSource",
     "TransactionSourceAccountTransferIntention",
     "TransactionSourceACHTransferIntention",
     "TransactionSourceACHTransferRejection",
     "TransactionSourceACHTransferReturn",
     "TransactionSourceCardDisputeAcceptance",
     "TransactionSourceCardRefund",
-    "TransactionSourceCardSettlement",
     "TransactionSourceCardRevenuePayment",
+    "TransactionSourceCardSettlement",
     "TransactionSourceCheckDepositAcceptance",
     "TransactionSourceCheckDepositReturn",
+    "TransactionSourceCheckTransferDeposit",
     "TransactionSourceCheckTransferIntention",
-    "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferRejection",
+    "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferStopPaymentRequest",
     "TransactionSourceFeePayment",
     "TransactionSourceInboundACHTransfer",
     "TransactionSourceInboundCheck",
     "TransactionSourceInboundInternationalACHTransfer",
     "TransactionSourceInboundRealTimePaymentsTransferConfirmation",
-    "TransactionSourceInboundWireDrawdownPaymentReversal",
     "TransactionSourceInboundWireDrawdownPayment",
+    "TransactionSourceInboundWireDrawdownPaymentReversal",
     "TransactionSourceInboundWireReversal",
     "TransactionSourceInboundWireTransfer",
     "TransactionSourceInterestPayment",
     "TransactionSourceInternalSource",
     "TransactionSourceRealTimePaymentsTransferAcknowledgement",
     "TransactionSourceSampleFunds",
     "TransactionSourceWireTransferIntention",
@@ -118,15 +119,14 @@
         "authorization_revoked_by_customer",
         "invalid_ach_routing_number",
         "file_record_edit_criteria",
         "enr_invalid_individual_name",
         "returned_per_odfi_request",
         "limited_participation_dfi",
         "incorrectly_coded_outbound_international_payment",
-        "other",
         "account_sold_to_another_dfi",
         "addenda_error",
         "beneficiary_or_account_holder_deceased",
         "customer_advised_not_within_authorization_terms",
         "corrected_return",
         "duplicate_entry",
         "duplicate_return",
@@ -196,29 +196,29 @@
     """
     The identifier of the Transaction that was created to return the disputed funds
     to your account.
     """
 
 
 class TransactionSourceCardRefund(BaseModel):
+    id: str
+    """The Card Refund identifier."""
+
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
     """
 
-    id: str
-    """The Card Refund identifier."""
-
     merchant_acceptor_id: Optional[str]
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
 
     merchant_category_code: str
@@ -239,15 +239,41 @@
     type: Literal["card_refund"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_refund`.
     """
 
 
+class TransactionSourceCardRevenuePayment(BaseModel):
+    amount: int
+    """The amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
+    currency.
+    """
+
+    period_end: datetime
+    """The end of the period for which this transaction paid interest."""
+
+    period_start: datetime
+    """The start of the period for which this transaction paid interest."""
+
+    transacted_on_account_id: Optional[str]
+    """The account the card belonged to."""
+
+
 class TransactionSourceCardSettlement(BaseModel):
+    id: str
+    """The Card Settlement identifier."""
+
     amount: int
     """The amount in the minor unit of the transaction's settlement currency.
 
     For dollars, for example, this is cents.
     """
 
     card_authorization: Optional[str]
@@ -258,17 +284,14 @@
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's settlement currency.
     """
 
-    id: str
-    """The Card Settlement identifier."""
-
     merchant_acceptor_id: Optional[str]
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
 
     merchant_category_code: str
@@ -301,37 +324,14 @@
     type: Literal["card_settlement"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_settlement`.
     """
 
 
-class TransactionSourceCardRevenuePayment(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
-    currency.
-    """
-
-    period_end: datetime
-    """The end of the period for which this transaction paid interest."""
-
-    period_start: datetime
-    """The start of the period for which this transaction paid interest."""
-
-    transacted_on_account_id: Optional[str]
-    """The account the card belonged to."""
-
-
 class TransactionSourceCheckDepositAcceptance(BaseModel):
     account_number: str
     """The account number printed on the check."""
 
     amount: int
     """The amount to be deposited in the minor unit of the transaction's currency.
 
@@ -404,46 +404,74 @@
     transaction_id: str
     """
     The identifier of the transaction that reversed the original check deposit
     transaction.
     """
 
 
+class TransactionSourceCheckTransferDeposit(BaseModel):
+    back_image_file_id: Optional[str]
+    """
+    The identifier of the API File object containing an image of the back of the
+    deposited check.
+    """
+
+    deposited_at: datetime
+    """When the check was deposited."""
+
+    front_image_file_id: Optional[str]
+    """
+    The identifier of the API File object containing an image of the front of the
+    deposited check.
+    """
+
+    type: Literal["check_transfer_deposit"]
+    """A constant representing the object's type.
+
+    For this resource it will always be `check_transfer_deposit`.
+    """
+
+
 class TransactionSourceCheckTransferIntention(BaseModel):
-    address_city: str
+    address_city: Optional[str]
     """The city of the check's destination."""
 
-    address_line1: str
+    address_line1: Optional[str]
     """The street address of the check's destination."""
 
     address_line2: Optional[str]
     """The second line of the address of the check's destination."""
 
-    address_state: str
+    address_state: Optional[str]
     """The state of the check's destination."""
 
-    address_zip: str
+    address_zip: Optional[str]
     """The postal code of the check's destination."""
 
     amount: int
     """The transfer amount in USD cents."""
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the check's
     currency.
     """
 
-    recipient_name: str
+    recipient_name: Optional[str]
     """The name that will be printed on the check."""
 
     transfer_id: str
     """The identifier of the Check Transfer with which this is associated."""
 
 
+class TransactionSourceCheckTransferRejection(BaseModel):
+    transfer_id: str
+    """The identifier of the Check Transfer that led to this Transaction."""
+
+
 class TransactionSourceCheckTransferReturn(BaseModel):
     file_id: Optional[str]
     """If available, a document with additional information about the return."""
 
     reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"]
     """The reason why the check was returned."""
 
@@ -459,19 +487,14 @@
     returned check.
     """
 
     transfer_id: str
     """The identifier of the returned Check Transfer."""
 
 
-class TransactionSourceCheckTransferRejection(BaseModel):
-    transfer_id: str
-    """The identifier of the Check Transfer that led to this Transaction."""
-
-
 class TransactionSourceCheckTransferStopPaymentRequest(BaseModel):
     requested_at: datetime
     """The time the stop-payment was requested."""
 
     transaction_id: str
     """The transaction ID of the corresponding credit transaction."""
 
@@ -649,46 +672,14 @@
     remittance_information: Optional[str]
     """Additional information included with the transfer."""
 
     transaction_identification: str
     """The Real Time Payments network identification of the transfer"""
 
 
-class TransactionSourceInboundWireDrawdownPaymentReversal(BaseModel):
-    amount: int
-    """The amount that was reversed."""
-
-    description: str
-    """The description on the reversal message from Fedwire."""
-
-    input_cycle_date: date
-    """The Fedwire cycle date for the wire reversal."""
-
-    input_message_accountability_data: str
-    """The Fedwire transaction identifier."""
-
-    input_sequence_number: str
-    """The Fedwire sequence number."""
-
-    input_source: str
-    """The Fedwire input source identifier."""
-
-    previous_message_input_cycle_date: date
-    """The Fedwire cycle date for the wire transfer that was reversed."""
-
-    previous_message_input_message_accountability_data: str
-    """The Fedwire transaction identifier for the wire transfer that was reversed."""
-
-    previous_message_input_sequence_number: str
-    """The Fedwire sequence number for the wire transfer that was reversed."""
-
-    previous_message_input_source: str
-    """The Fedwire input source identifier for the wire transfer that was reversed."""
-
-
 class TransactionSourceInboundWireDrawdownPayment(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -713,14 +704,46 @@
     originator_address_line3: Optional[str]
 
     originator_name: Optional[str]
 
     originator_to_beneficiary_information: Optional[str]
 
 
+class TransactionSourceInboundWireDrawdownPaymentReversal(BaseModel):
+    amount: int
+    """The amount that was reversed."""
+
+    description: str
+    """The description on the reversal message from Fedwire."""
+
+    input_cycle_date: date
+    """The Fedwire cycle date for the wire reversal."""
+
+    input_message_accountability_data: str
+    """The Fedwire transaction identifier."""
+
+    input_sequence_number: str
+    """The Fedwire sequence number."""
+
+    input_source: str
+    """The Fedwire input source identifier."""
+
+    previous_message_input_cycle_date: date
+    """The Fedwire cycle date for the wire transfer that was reversed."""
+
+    previous_message_input_message_accountability_data: str
+    """The Fedwire transaction identifier for the wire transfer that was reversed."""
+
+    previous_message_input_sequence_number: str
+    """The Fedwire sequence number for the wire transfer that was reversed."""
+
+    previous_message_input_source: str
+    """The Fedwire input source identifier for the wire transfer that was reversed."""
+
+
 class TransactionSourceInboundWireReversal(BaseModel):
     amount: int
     """The amount that was reversed."""
 
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
@@ -964,30 +987,31 @@
     category: Literal[
         "account_transfer_intention",
         "ach_transfer_intention",
         "ach_transfer_rejection",
         "ach_transfer_return",
         "card_dispute_acceptance",
         "card_refund",
-        "card_settlement",
         "card_revenue_payment",
+        "card_settlement",
         "check_deposit_acceptance",
         "check_deposit_return",
+        "check_transfer_deposit",
         "check_transfer_intention",
-        "check_transfer_return",
         "check_transfer_rejection",
+        "check_transfer_return",
         "check_transfer_stop_payment_request",
         "fee_payment",
         "inbound_ach_transfer",
         "inbound_ach_transfer_return_intention",
         "inbound_check",
         "inbound_international_ach_transfer",
         "inbound_real_time_payments_transfer_confirmation",
-        "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_drawdown_payment",
+        "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_reversal",
         "inbound_wire_transfer",
         "interest_payment",
         "internal_source",
         "real_time_payments_transfer_acknowledgement",
         "sample_funds",
         "wire_transfer_intention",
@@ -1010,14 +1034,21 @@
     check_deposit_return: Optional[TransactionSourceCheckDepositReturn]
     """A Check Deposit Return object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_deposit_return`.
     """
 
+    check_transfer_deposit: Optional[TransactionSourceCheckTransferDeposit]
+    """A Check Transfer Deposit object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `check_transfer_deposit`.
+    """
+
     check_transfer_intention: Optional[TransactionSourceCheckTransferIntention]
     """A Check Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_transfer_intention`.
     """
 
@@ -1147,14 +1178,17 @@
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_transfer_rejection`.
     """
 
 
 class Transaction(BaseModel):
+    id: str
+    """The Transaction identifier."""
+
     account_id: str
     """The identifier for the Account the Transaction belongs to."""
 
     amount: int
     """The Transaction amount in the minor unit of its currency.
 
     For dollars, for example, this is cents.
@@ -1176,17 +1210,14 @@
     description: str
     """For a Transaction related to a transfer, this is the description you provide.
 
     For a Transaction related to a payment, this is the description the vendor
     provides.
     """
 
-    id: str
-    """The Transaction identifier."""
-
     route_id: Optional[str]
     """The identifier for the route this Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
     route_type: Optional[Literal["account_number", "card"]]
```

### Comparing `increase-0.7.1/src/increase/types/transaction.py` & `increase-0.8.0/src/increase/types/transaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,29 +11,30 @@
     "Source",
     "SourceAccountTransferIntention",
     "SourceACHTransferIntention",
     "SourceACHTransferRejection",
     "SourceACHTransferReturn",
     "SourceCardDisputeAcceptance",
     "SourceCardRefund",
-    "SourceCardSettlement",
     "SourceCardRevenuePayment",
+    "SourceCardSettlement",
     "SourceCheckDepositAcceptance",
     "SourceCheckDepositReturn",
+    "SourceCheckTransferDeposit",
     "SourceCheckTransferIntention",
-    "SourceCheckTransferReturn",
     "SourceCheckTransferRejection",
+    "SourceCheckTransferReturn",
     "SourceCheckTransferStopPaymentRequest",
     "SourceFeePayment",
     "SourceInboundACHTransfer",
     "SourceInboundCheck",
     "SourceInboundInternationalACHTransfer",
     "SourceInboundRealTimePaymentsTransferConfirmation",
-    "SourceInboundWireDrawdownPaymentReversal",
     "SourceInboundWireDrawdownPayment",
+    "SourceInboundWireDrawdownPaymentReversal",
     "SourceInboundWireReversal",
     "SourceInboundWireTransfer",
     "SourceInterestPayment",
     "SourceInternalSource",
     "SourceRealTimePaymentsTransferAcknowledgement",
     "SourceSampleFunds",
     "SourceWireTransferIntention",
@@ -117,15 +118,14 @@
         "authorization_revoked_by_customer",
         "invalid_ach_routing_number",
         "file_record_edit_criteria",
         "enr_invalid_individual_name",
         "returned_per_odfi_request",
         "limited_participation_dfi",
         "incorrectly_coded_outbound_international_payment",
-        "other",
         "account_sold_to_another_dfi",
         "addenda_error",
         "beneficiary_or_account_holder_deceased",
         "customer_advised_not_within_authorization_terms",
         "corrected_return",
         "duplicate_entry",
         "duplicate_return",
@@ -195,29 +195,29 @@
     """
     The identifier of the Transaction that was created to return the disputed funds
     to your account.
     """
 
 
 class SourceCardRefund(BaseModel):
+    id: str
+    """The Card Refund identifier."""
+
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
     """
 
-    id: str
-    """The Card Refund identifier."""
-
     merchant_acceptor_id: Optional[str]
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
 
     merchant_category_code: str
@@ -238,15 +238,41 @@
     type: Literal["card_refund"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_refund`.
     """
 
 
+class SourceCardRevenuePayment(BaseModel):
+    amount: int
+    """The amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
+    currency.
+    """
+
+    period_end: datetime
+    """The end of the period for which this transaction paid interest."""
+
+    period_start: datetime
+    """The start of the period for which this transaction paid interest."""
+
+    transacted_on_account_id: Optional[str]
+    """The account the card belonged to."""
+
+
 class SourceCardSettlement(BaseModel):
+    id: str
+    """The Card Settlement identifier."""
+
     amount: int
     """The amount in the minor unit of the transaction's settlement currency.
 
     For dollars, for example, this is cents.
     """
 
     card_authorization: Optional[str]
@@ -257,17 +283,14 @@
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's settlement currency.
     """
 
-    id: str
-    """The Card Settlement identifier."""
-
     merchant_acceptor_id: Optional[str]
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
 
     merchant_category_code: str
@@ -300,37 +323,14 @@
     type: Literal["card_settlement"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_settlement`.
     """
 
 
-class SourceCardRevenuePayment(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
-    currency.
-    """
-
-    period_end: datetime
-    """The end of the period for which this transaction paid interest."""
-
-    period_start: datetime
-    """The start of the period for which this transaction paid interest."""
-
-    transacted_on_account_id: Optional[str]
-    """The account the card belonged to."""
-
-
 class SourceCheckDepositAcceptance(BaseModel):
     account_number: str
     """The account number printed on the check."""
 
     amount: int
     """The amount to be deposited in the minor unit of the transaction's currency.
 
@@ -403,46 +403,74 @@
     transaction_id: str
     """
     The identifier of the transaction that reversed the original check deposit
     transaction.
     """
 
 
+class SourceCheckTransferDeposit(BaseModel):
+    back_image_file_id: Optional[str]
+    """
+    The identifier of the API File object containing an image of the back of the
+    deposited check.
+    """
+
+    deposited_at: datetime
+    """When the check was deposited."""
+
+    front_image_file_id: Optional[str]
+    """
+    The identifier of the API File object containing an image of the front of the
+    deposited check.
+    """
+
+    type: Literal["check_transfer_deposit"]
+    """A constant representing the object's type.
+
+    For this resource it will always be `check_transfer_deposit`.
+    """
+
+
 class SourceCheckTransferIntention(BaseModel):
-    address_city: str
+    address_city: Optional[str]
     """The city of the check's destination."""
 
-    address_line1: str
+    address_line1: Optional[str]
     """The street address of the check's destination."""
 
     address_line2: Optional[str]
     """The second line of the address of the check's destination."""
 
-    address_state: str
+    address_state: Optional[str]
     """The state of the check's destination."""
 
-    address_zip: str
+    address_zip: Optional[str]
     """The postal code of the check's destination."""
 
     amount: int
     """The transfer amount in USD cents."""
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the check's
     currency.
     """
 
-    recipient_name: str
+    recipient_name: Optional[str]
     """The name that will be printed on the check."""
 
     transfer_id: str
     """The identifier of the Check Transfer with which this is associated."""
 
 
+class SourceCheckTransferRejection(BaseModel):
+    transfer_id: str
+    """The identifier of the Check Transfer that led to this Transaction."""
+
+
 class SourceCheckTransferReturn(BaseModel):
     file_id: Optional[str]
     """If available, a document with additional information about the return."""
 
     reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"]
     """The reason why the check was returned."""
 
@@ -458,19 +486,14 @@
     returned check.
     """
 
     transfer_id: str
     """The identifier of the returned Check Transfer."""
 
 
-class SourceCheckTransferRejection(BaseModel):
-    transfer_id: str
-    """The identifier of the Check Transfer that led to this Transaction."""
-
-
 class SourceCheckTransferStopPaymentRequest(BaseModel):
     requested_at: datetime
     """The time the stop-payment was requested."""
 
     transaction_id: str
     """The transaction ID of the corresponding credit transaction."""
 
@@ -648,46 +671,14 @@
     remittance_information: Optional[str]
     """Additional information included with the transfer."""
 
     transaction_identification: str
     """The Real Time Payments network identification of the transfer"""
 
 
-class SourceInboundWireDrawdownPaymentReversal(BaseModel):
-    amount: int
-    """The amount that was reversed."""
-
-    description: str
-    """The description on the reversal message from Fedwire."""
-
-    input_cycle_date: date
-    """The Fedwire cycle date for the wire reversal."""
-
-    input_message_accountability_data: str
-    """The Fedwire transaction identifier."""
-
-    input_sequence_number: str
-    """The Fedwire sequence number."""
-
-    input_source: str
-    """The Fedwire input source identifier."""
-
-    previous_message_input_cycle_date: date
-    """The Fedwire cycle date for the wire transfer that was reversed."""
-
-    previous_message_input_message_accountability_data: str
-    """The Fedwire transaction identifier for the wire transfer that was reversed."""
-
-    previous_message_input_sequence_number: str
-    """The Fedwire sequence number for the wire transfer that was reversed."""
-
-    previous_message_input_source: str
-    """The Fedwire input source identifier for the wire transfer that was reversed."""
-
-
 class SourceInboundWireDrawdownPayment(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -712,14 +703,46 @@
     originator_address_line3: Optional[str]
 
     originator_name: Optional[str]
 
     originator_to_beneficiary_information: Optional[str]
 
 
+class SourceInboundWireDrawdownPaymentReversal(BaseModel):
+    amount: int
+    """The amount that was reversed."""
+
+    description: str
+    """The description on the reversal message from Fedwire."""
+
+    input_cycle_date: date
+    """The Fedwire cycle date for the wire reversal."""
+
+    input_message_accountability_data: str
+    """The Fedwire transaction identifier."""
+
+    input_sequence_number: str
+    """The Fedwire sequence number."""
+
+    input_source: str
+    """The Fedwire input source identifier."""
+
+    previous_message_input_cycle_date: date
+    """The Fedwire cycle date for the wire transfer that was reversed."""
+
+    previous_message_input_message_accountability_data: str
+    """The Fedwire transaction identifier for the wire transfer that was reversed."""
+
+    previous_message_input_sequence_number: str
+    """The Fedwire sequence number for the wire transfer that was reversed."""
+
+    previous_message_input_source: str
+    """The Fedwire input source identifier for the wire transfer that was reversed."""
+
+
 class SourceInboundWireReversal(BaseModel):
     amount: int
     """The amount that was reversed."""
 
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
@@ -963,30 +986,31 @@
     category: Literal[
         "account_transfer_intention",
         "ach_transfer_intention",
         "ach_transfer_rejection",
         "ach_transfer_return",
         "card_dispute_acceptance",
         "card_refund",
-        "card_settlement",
         "card_revenue_payment",
+        "card_settlement",
         "check_deposit_acceptance",
         "check_deposit_return",
+        "check_transfer_deposit",
         "check_transfer_intention",
-        "check_transfer_return",
         "check_transfer_rejection",
+        "check_transfer_return",
         "check_transfer_stop_payment_request",
         "fee_payment",
         "inbound_ach_transfer",
         "inbound_ach_transfer_return_intention",
         "inbound_check",
         "inbound_international_ach_transfer",
         "inbound_real_time_payments_transfer_confirmation",
-        "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_drawdown_payment",
+        "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_reversal",
         "inbound_wire_transfer",
         "interest_payment",
         "internal_source",
         "real_time_payments_transfer_acknowledgement",
         "sample_funds",
         "wire_transfer_intention",
@@ -1009,14 +1033,21 @@
     check_deposit_return: Optional[SourceCheckDepositReturn]
     """A Check Deposit Return object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_deposit_return`.
     """
 
+    check_transfer_deposit: Optional[SourceCheckTransferDeposit]
+    """A Check Transfer Deposit object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `check_transfer_deposit`.
+    """
+
     check_transfer_intention: Optional[SourceCheckTransferIntention]
     """A Check Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_transfer_intention`.
     """
 
@@ -1144,14 +1175,17 @@
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_transfer_rejection`.
     """
 
 
 class Transaction(BaseModel):
+    id: str
+    """The Transaction identifier."""
+
     account_id: str
     """The identifier for the Account the Transaction belongs to."""
 
     amount: int
     """The Transaction amount in the minor unit of its currency.
 
     For dollars, for example, this is cents.
@@ -1173,17 +1207,14 @@
     description: str
     """For a Transaction related to a transfer, this is the description you provide.
 
     For a Transaction related to a payment, this is the description the vendor
     provides.
     """
 
-    id: str
-    """The Transaction identifier."""
-
     route_id: Optional[str]
     """The identifier for the route this Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
     route_type: Optional[Literal["account_number", "card"]]
```

### Comparing `increase-0.7.1/src/increase/types/transaction_list_params.py` & `increase-0.8.0/src/increase/types/transaction_list_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,30 +42,31 @@
             Literal[
                 "account_transfer_intention",
                 "ach_transfer_intention",
                 "ach_transfer_rejection",
                 "ach_transfer_return",
                 "card_dispute_acceptance",
                 "card_refund",
-                "card_settlement",
                 "card_revenue_payment",
+                "card_settlement",
                 "check_deposit_acceptance",
                 "check_deposit_return",
+                "check_transfer_deposit",
                 "check_transfer_intention",
-                "check_transfer_return",
                 "check_transfer_rejection",
+                "check_transfer_return",
                 "check_transfer_stop_payment_request",
                 "fee_payment",
                 "inbound_ach_transfer",
                 "inbound_ach_transfer_return_intention",
                 "inbound_check",
                 "inbound_international_ach_transfer",
                 "inbound_real_time_payments_transfer_confirmation",
-                "inbound_wire_drawdown_payment_reversal",
                 "inbound_wire_drawdown_payment",
+                "inbound_wire_drawdown_payment_reversal",
                 "inbound_wire_reversal",
                 "inbound_wire_transfer",
                 "interest_payment",
                 "internal_source",
                 "real_time_payments_transfer_acknowledgement",
                 "sample_funds",
                 "wire_transfer_intention",
```

### Comparing `increase-0.7.1/src/increase/types/wire_drawdown_request.py` & `increase-0.8.0/src/increase/types/wire_drawdown_request.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     """
     The input message accountability data (IMAD) uniquely identifying the submission
     with Fedwire.
     """
 
 
 class WireDrawdownRequest(BaseModel):
+    id: str
+    """The Wire drawdown request identifier."""
+
     account_number_id: str
     """
     The Account Number to which the recipient of this request is being requested to
     send funds.
     """
 
     amount: int
@@ -34,17 +37,14 @@
 
     fulfillment_transaction_id: Optional[str]
     """
     If the recipient fulfills the drawdown request by sending funds, then this will
     be the identifier of the corresponding Transaction.
     """
 
-    id: str
-    """The Wire drawdown request identifier."""
-
     message_to_recipient: str
     """The message the recipient will see as part of the drawdown request."""
 
     recipient_account_number: str
     """The drawdown request's recipient's account number."""
 
     recipient_address_line1: Optional[str]
```

### Comparing `increase-0.7.1/src/increase/types/wire_drawdown_request_create_params.py` & `increase-0.8.0/src/increase/types/wire_drawdown_request_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/wire_transfer.py` & `increase-0.8.0/src/increase/types/wire_transfer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -95,14 +95,17 @@
     """The accountability data for the submission."""
 
     submitted_at: datetime
     """When this wire transfer was submitted to Fedwire."""
 
 
 class WireTransfer(BaseModel):
+    id: str
+    """The wire transfer's identifier."""
+
     account_id: str
     """The Account to which the transfer belongs."""
 
     account_number: str
     """The destination account number."""
 
     amount: int
@@ -143,17 +146,14 @@
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transfer's
     currency. For wire transfers this is always equal to `usd`.
     """
 
     external_account_id: Optional[str]
     """The identifier of the External Account the transfer was made to, if any."""
 
-    id: str
-    """The wire transfer's identifier."""
-
     message_to_recipient: Optional[str]
     """The message that will show on the recipient's bank statement."""
 
     network: Literal["wire"]
     """The transfer's network."""
 
     reversal: Optional[Reversal]
```

### Comparing `increase-0.7.1/src/increase/types/wire_transfer_create_params.py` & `increase-0.8.0/src/increase/types/wire_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/src/increase/types/wire_transfer_list_params.py` & `increase-0.8.0/src/increase/types/wire_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.1/PKG-INFO` & `increase-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: increase
-Version: 0.7.1
+Version: 0.8.0
 Summary: Client library for the increase API
 Home-page: https://github.com/increase/increase-python
 License: Apache-2.0
 Author: Increase
 Author-email: dev-feedback@increase.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -148,15 +148,15 @@
 Or just work directly with the returned data:
 
 ```python
 first_page = await increase.accounts.list()
 
 print(f"next page cursor: {first_page.next_cursor}")  # => "next page cursor: ..."
 for account in first_page.data:
-    print(account.created_at)
+    print(account.id)
 
 # Remove `await` for non-async usage.
 ```
 
 ## Nested params
 
 Nested parameters are dictionaries, typed using `TypedDict`, for example:
@@ -325,7 +325,8 @@
 please reach out if you rely on any undocumented behavior.
 
 We are keen for your feedback; please open an [issue](https://www.github.com/increase/increase-python/issues) with questions, bugs, or suggestions.
 
 ## Requirements
 
 Python 3.7 or higher.
+
```

