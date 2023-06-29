# Comparing `tmp/oslo.messaging-9.7.2.tar.gz` & `tmp/oslo.messaging-9.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oslo.messaging-9.7.2.tar", last modified: Fri Jun 14 04:02:46 2019, max compression
+gzip compressed data, was "dist/oslo.messaging-9.8.0.tar", last modified: Thu Jul 18 02:40:29 2019, max compression
```

## Comparing `oslo.messaging-9.7.2.tar` & `oslo.messaging-9.8.0.tar`

### file list

```diff
@@ -1,221 +1,221 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7885 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/.zuul.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1030 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/setup.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      973 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/README.rst
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)      591 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/setup-test-env-kafka.sh
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2202 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/PKG-INFO
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1003 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/etc/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      739 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/etc/routing_notifier.yaml.sample
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      547 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/CONTRIBUTING.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1646 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/lower-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/tools/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    25119 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/tools/messages_length.yaml
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1420 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/tools/setup-test-env-amqp1.sh
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      393 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/tools/functions.sh
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)    29606 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/tools/simulator.py
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1386 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/tools/test-setup.sh
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      105 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/.coveragerc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo_messaging/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18999 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/transport.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo_messaging/hacking/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11876 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/hacking/checks.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/hacking/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4616 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/pool.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18174 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/impl_amqp1.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/kafka_driver/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3128 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/kafka_driver/kafka_options.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/kafka_driver/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4171 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/amqp.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    19979 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/common.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/amqp1_driver/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14524 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/amqp1_driver/eventloop.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11174 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/amqp1_driver/addressing.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10847 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/amqp1_driver/opts.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    55238 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/amqp1_driver/controller.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/amqp1_driver/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    62897 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/amqp1_driver/oslo_messaging_amqp_driver_overview.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9364 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/impl_fake.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15916 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/impl_kafka.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    54905 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/impl_rabbit.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    25491 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    27253 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_drivers/amqpdriver.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1299 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/exceptions.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4399 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/target.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17021 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/server.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1730 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo_messaging/notify/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3132 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/notify/messaging.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3238 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/notify/filter.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11969 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/notify/listener.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2780 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/notify/logger.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1781 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/notify/_impl_log.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3961 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/notify/middleware.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5218 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/notify/_impl_routing.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6201 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/notify/dispatcher.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      817 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/notify/_impl_noop.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1811 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/notify/log_handler.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1062 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/notify/_impl_test.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1125 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/notify/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17476 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/notify/notifier.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5381 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/conffixture.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3098 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/opts.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1005 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/dispatcher.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo_messaging/tests/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3481 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/test_config_opts_proxy.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3901 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/test_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2260 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/test_opts.py
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)    13330 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/test_transport.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11158 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/test_exception_serialization.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8291 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/test_urls.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo_messaging/tests/notify/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20975 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/notify/test_listener.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2534 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/notify/test_log_handler.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5635 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/notify/test_logger.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8624 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/notify/test_middleware.py
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)    23361 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/notify/test_notifier.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/notify/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9719 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/notify/test_dispatcher.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo_messaging/tests/drivers/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    96679 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/drivers/test_amqp_driver.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3614 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/drivers/test_pool.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6969 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/drivers/test_impl_kafka.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/drivers/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    41530 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/drivers/test_impl_rabbit.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo_messaging/tests/functional/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4786 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/functional/test_rabbitmq.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo_messaging/tests/functional/notify/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3074 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/functional/notify/test_logger.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/functional/notify/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14456 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/functional/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/functional/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20322 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/functional/test_functional.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6962 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/test_target.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3393 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/test_fixture.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2668 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2119 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/test_expected_exceptions.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      962 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo_messaging/tests/rpc/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/rpc/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    35523 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/rpc/test_server.py
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)    13117 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/rpc/test_dispatcher.py
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)    21585 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/tests/rpc/test_client.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      694 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/version.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      769 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo_messaging/rpc/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1956 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/rpc/transport.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21404 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/rpc/client.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9467 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/rpc/server.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10727 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/rpc/dispatcher.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1124 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/rpc/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2473 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/oslo_messaging/serializer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    68360 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/ChangeLog
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11690 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/LICENSE
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/playbooks/oslo.messaging-telemetry-dsvm-integration-kafka/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2779 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/playbooks/oslo.messaging-telemetry-dsvm-integration-kafka/run.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2409 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/playbooks/oslo.messaging-telemetry-dsvm-integration-kafka/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/playbooks/oslo.messaging-src-grenade-dsvm/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1860 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/playbooks/oslo.messaging-src-grenade-dsvm/run.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/playbooks/oslo.messaging-src-grenade-dsvm/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/playbooks/oslo.messaging-telemetry-dsvm-integration-amqp1/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2852 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/playbooks/oslo.messaging-telemetry-dsvm-integration-amqp1/run.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2409 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/playbooks/oslo.messaging-telemetry-dsvm-integration-amqp1/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/playbooks/oslo.messaging-telemetry-dsvm-integration-rabbit/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2544 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/playbooks/oslo.messaging-telemetry-dsvm-integration-rabbit/run.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2409 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/playbooks/oslo.messaging-telemetry-dsvm-integration-rabbit/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/playbooks/oslo.messaging-src-grenade-dsvm-multinode/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1940 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/playbooks/oslo.messaging-src-grenade-dsvm-multinode/run.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/playbooks/oslo.messaging-src-grenade-dsvm-multinode/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/releasenotes/source/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      110 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/source/unreleased.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      145 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/source/stein.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2315 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/source/conf.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      145 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/source/rocky.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/releasenotes/source/_templates/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/source/_templates/.placeholder
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      140 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/source/newton.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6137 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      147 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/source/queens.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      136 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/source/ocata.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      199 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/releasenotes/source/_static/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/source/_static/.placeholder
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      143 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/source/pike.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/releasenotes/notes/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      792 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/removal-deprecated-options-6d4c5db90525c52d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      223 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/connection_ttl-2cf0fe6e1ab8c73c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      300 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/use-extras-for-optional-deps-2a00e8007ef7a629.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      111 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/fix-access_policy-deafult-a6954a147cb002b0.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      463 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/RPC-call-monitoring-7977f047d069769a.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      499 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/kafka-client-library-change-fe16d5a34550db7f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      285 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/remove-pika-1bae204ced2521a3.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      343 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/get_rpc_transport-4aa3511ad9754a60.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      615 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/rabbit-no-wait-for-ack-9e5de3e1320d7660.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      297 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/remove-ZeroMQ-driver-e9e0bbbb7bd4f5e6.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      179 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/retry-support-07996ef04dda9482.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      267 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/blocking-executor-deprecated-895146c1c3bf2f51.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       57 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/add_reno-3b4ae0789e9c45b4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      272 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/deprecate-ZeroMQ-driver-a8af25aaba867c5b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      140 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/remove-RequestContextSerializer-234c0496a7e0376b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      657 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/bump-amqp-version-due-to-tls-issue-e877b152eb101c15.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      210 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/option-rabbitmq-max_retries-has-been-deprecated-471f66a9e6d672a2.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      300 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/releasenotes/notes/pika-driver-has-been-deprecated-e2407fa53c91fe5c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      940 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/test-requirements.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      887 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/requirements.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       16 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo.messaging.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      993 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo.messaging.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo.messaging.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo.messaging.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7024 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo.messaging.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo.messaging.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo.messaging.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo.messaging.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/oslo.messaging.egg-info/pbr.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/doc/source/user/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       32 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/user/history.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2170 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/user/FAQ.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      143 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/user/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1469 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/doc/source/contributor/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1641 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/contributor/driver-dev-guide.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      191 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/contributor/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2161 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/contributor/supported-messaging-drivers.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       84 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/contributor/contributing.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/doc/source/admin/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9396 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/admin/kafka.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      115 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/admin/drivers.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    24479 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/admin/AMQP1.0.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      113 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/admin/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/doc/source/configuration/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      158 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/configuration/conffixture.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      349 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/configuration/opts.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       96 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/doc/source/reference/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      340 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/reference/notifier.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1086 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/reference/executors.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      275 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/reference/notification_driver.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      245 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/reference/notification_listener.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      652 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/reference/transport.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2234 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/reference/target.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      139 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/reference/serializer.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      482 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/reference/server.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      139 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/reference/rpcclient.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      516 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/reference/exceptions.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      223 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/reference/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      366 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/source/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      598 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/doc/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8487 2019-06-14 04:02:46.000000 oslo.messaging-9.7.2/AUTHORS
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       55 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/.stestr.conf
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3511 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/tox.ini
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      120 2019-06-14 04:01:47.000000 oslo.messaging-9.7.2/HACKING.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/removal-deprecated-options-6d4c5db90525c52d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/fix-access_policy-deafult-a6954a147cb002b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/remove-ZeroMQ-driver-e9e0bbbb7bd4f5e6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/blocking-executor-deprecated-895146c1c3bf2f51.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/retry-support-07996ef04dda9482.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/connection_ttl-2cf0fe6e1ab8c73c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/use-extras-for-optional-deps-2a00e8007ef7a629.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/pika-driver-has-been-deprecated-e2407fa53c91fe5c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/remove-pika-1bae204ced2521a3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/add_reno-3b4ae0789e9c45b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/option-rabbitmq-max_retries-has-been-deprecated-471f66a9e6d672a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/RPC-call-monitoring-7977f047d069769a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/remove-RequestContextSerializer-234c0496a7e0376b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/rabbit-no-wait-for-ack-9e5de3e1320d7660.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/bump-amqp-version-due-to-tls-issue-e877b152eb101c15.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/kafka-client-library-change-fe16d5a34550db7f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/deprecate-ZeroMQ-driver-a8af25aaba867c5b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/notes/get_rpc_transport-4aa3511ad9754a60.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2315 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/source/pike.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/source/_templates/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6137 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/source/_static/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2073 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8529 2019-07-18 02:40:28.000000 oslo.messaging-9.8.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2241 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11690 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1646 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/oslo.messaging.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2073 2019-07-18 02:40:28.000000 oslo.messaging-9.8.0/oslo.messaging.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-07-18 02:40:28.000000 oslo.messaging-9.8.0/oslo.messaging.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      993 2019-07-18 02:40:28.000000 oslo.messaging-9.8.0/oslo.messaging.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2019-07-18 02:40:28.000000 oslo.messaging-9.8.0/oslo.messaging.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2019-07-18 02:40:28.000000 oslo.messaging-9.8.0/oslo.messaging.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2019-07-18 02:40:28.000000 oslo.messaging-9.8.0/oslo.messaging.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-07-18 02:40:28.000000 oslo.messaging-9.8.0/oslo.messaging.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7024 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/oslo.messaging.egg-info/SOURCES.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      595 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/setup-test-env-kafka.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/oslo_messaging/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5381 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/conffixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3098 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1685 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1730 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4616 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19980 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18382 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/impl_amqp1.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9471 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/impl_fake.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/amqp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27437 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/amqpdriver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25772 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15940 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/impl_kafka.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/kafka_driver/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/kafka_driver/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3128 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/kafka_driver/kafka_options.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/amqp1_driver/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10847 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/amqp1_driver/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14524 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/amqp1_driver/eventloop.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    55238 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/amqp1_driver/controller.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    62897 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/amqp1_driver/oslo_messaging_amqp_driver_overview.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/amqp1_driver/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11174 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/amqp1_driver/addressing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    55886 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/_drivers/impl_rabbit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1005 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/dispatcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4399 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/target.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2473 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/serializer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17021 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      694 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/oslo_messaging/rpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10727 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/rpc/dispatcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9467 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/rpc/server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1956 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/rpc/transport.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22163 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/rpc/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1124 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/rpc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19320 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/transport.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/oslo_messaging/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11876 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/hacking/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/oslo_messaging/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2260 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/test_opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/oslo_messaging/tests/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    96679 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/drivers/test_amqp_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3614 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/drivers/test_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6969 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/drivers/test_impl_kafka.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41588 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/drivers/test_impl_rabbit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8291 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/test_urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/oslo_messaging/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22036 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/functional/test_functional.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4786 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/functional/test_rabbitmq.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14600 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/functional/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/oslo_messaging/tests/functional/notify/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/functional/notify/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3074 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/functional/notify/test_logger.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3901 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2119 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/test_expected_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6962 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/test_target.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3481 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/test_config_opts_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3393 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/test_fixture.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/oslo_messaging/tests/rpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35523 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/rpc/test_server.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    23337 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/rpc/test_client.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    13117 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/rpc/test_dispatcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/rpc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2668 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    13461 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/test_transport.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11158 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/test_exception_serialization.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/oslo_messaging/tests/notify/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20975 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/notify/test_listener.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    23361 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/notify/test_notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2534 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/notify/test_log_handler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9719 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/notify/test_dispatcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/notify/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8624 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/notify/test_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5635 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/tests/notify/test_logger.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/oslo_messaging/notify/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3132 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/notify/messaging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1062 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/notify/_impl_test.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2780 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/notify/logger.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17476 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/notify/notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6201 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/notify/dispatcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11969 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/notify/listener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5218 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/notify/_impl_routing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1781 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/notify/_impl_log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3961 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/notify/middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/notify/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3238 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/notify/filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1811 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/notify/log_handler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/oslo_messaging/notify/_impl_noop.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    68647 2019-07-18 02:40:28.000000 oslo.messaging-9.8.0/ChangeLog
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/admin/drivers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9400 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/admin/kafka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24479 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/admin/AMQP1.0.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1086 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/reference/executors.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/reference/transport.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/reference/exceptions.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/reference/notification_listener.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/reference/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/reference/server.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2234 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/reference/target.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/reference/notifier.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/reference/serializer.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/reference/notification_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/reference/rpcclient.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1469 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/configuration/opts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/configuration/conffixture.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2170 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/user/FAQ.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2161 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/contributor/supported-messaging-drivers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1641 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/contributor/driver-dev-guide.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/etc/routing_notifier.yaml.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3511 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      973 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1003 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/bindep.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7858 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25119 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/tools/messages_length.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/tools/functions.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1420 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/tools/setup-test-env-amqp1.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1386 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/tools/test-setup.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    29606 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/tools/simulator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/playbooks/oslo.messaging-telemetry-dsvm-integration-amqp1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2852 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/playbooks/oslo.messaging-telemetry-dsvm-integration-amqp1/run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2409 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/playbooks/oslo.messaging-telemetry-dsvm-integration-amqp1/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/playbooks/oslo.messaging-telemetry-dsvm-integration-rabbit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2544 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/playbooks/oslo.messaging-telemetry-dsvm-integration-rabbit/run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2409 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/playbooks/oslo.messaging-telemetry-dsvm-integration-rabbit/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/playbooks/oslo.messaging-telemetry-dsvm-integration-kafka/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2779 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/playbooks/oslo.messaging-telemetry-dsvm-integration-kafka/run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2409 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/playbooks/oslo.messaging-telemetry-dsvm-integration-kafka/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/playbooks/oslo.messaging-src-grenade-dsvm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1860 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/playbooks/oslo.messaging-src-grenade-dsvm/run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/playbooks/oslo.messaging-src-grenade-dsvm/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-07-18 02:40:29.000000 oslo.messaging-9.8.0/playbooks/oslo.messaging-src-grenade-dsvm-multinode/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1940 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/playbooks/oslo.messaging-src-grenade-dsvm-multinode/run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/playbooks/oslo.messaging-src-grenade-dsvm-multinode/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      887 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2019-07-18 02:38:45.000000 oslo.messaging-9.8.0/.stestr.conf
```

### Comparing `oslo.messaging-9.7.2/.zuul.yaml` & `oslo.messaging-9.8.0/.zuul.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -216,16 +216,15 @@
     templates:
       - check-requirements
       - lib-forward-testing
       - lib-forward-testing-python3
       - openstack-cover-jobs
       - openstack-lower-constraints-jobs
       - openstack-python-jobs
-      - openstack-python36-jobs
-      - openstack-python37-jobs
+      - openstack-python3-train-jobs
       - periodic-stable-jobs
       - publish-openstack-docs-pti
       - release-notes-jobs-python3
     check:
       jobs:
         - oslo.messaging-tox-py27-func-rabbit
         - oslo.messaging-tox-py27-func-amqp1:
```

### Comparing `oslo.messaging-9.7.2/setup.py` & `oslo.messaging-9.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/README.rst` & `oslo.messaging-9.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/setup-test-env-kafka.sh` & `oslo.messaging-9.8.0/setup-test-env-kafka.sh`

 * *Files 3% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 
 if [[ -z "$(which kafka-server-start)" ]] && [[ -z $(which kafka-server-start.sh) ]]; then
     DATADIR=$(mktemp -d /tmp/OSLOMSG-KAFKA.XXXXX)
     trap "clean_exit $DATADIR" EXIT
 
     tarball=kafka_${SCALA_VERSION}-${KAFKA_VERSION}.tgz
 
-    wget http://www.apache.org/dist/kafka/${KAFKA_VERSION}/$tarball -O $DATADIR/$tarball
+    wget http://archive.apache.org/dist/kafka/${KAFKA_VERSION}/$tarball -O $DATADIR/$tarball
     tar -xzf $DATADIR/$tarball -C $DATADIR
     export PATH=$DATADIR/kafka_${SCALA_VERSION}-${KAFKA_VERSION}/bin:$PATH
 fi
 
 pifpaf run kafka -- $*
```

### Comparing `oslo.messaging-9.7.2/setup.cfg` & `oslo.messaging-9.8.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 2
 	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.7
 
 [extras]
 amqp1 = 
 	pyngus>=2.2.0 # Apache-2.0
 kafka = 
 	confluent-kafka>=0.11.6 # Apache-2.0
```

### Comparing `oslo.messaging-9.7.2/PKG-INFO` & `oslo.messaging-9.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslo.messaging
-Version: 9.7.2
+Version: 9.8.0
 Summary: Oslo Messaging API
 Home-page: https://docs.openstack.org/oslo.messaging/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -43,10 +43,11 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: kafka
-Provides-Extra: test
 Provides-Extra: amqp1
+Provides-Extra: test
```

### Comparing `oslo.messaging-9.7.2/bindep.txt` & `oslo.messaging-9.8.0/bindep.txt`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/etc/routing_notifier.yaml.sample` & `oslo.messaging-9.8.0/etc/routing_notifier.yaml.sample`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/CONTRIBUTING.rst` & `oslo.messaging-9.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/lower-constraints.txt` & `oslo.messaging-9.8.0/lower-constraints.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 GitPython==1.0.1
 greenlet==0.4.10
 hacking==0.12.0
 imagesize==0.7.1
 iso8601==0.1.11
 Jinja2==2.10
 keystoneauth1==3.4.0
-kombu==4.0.0
+kombu==4.6.1
 linecache2==1.0.0
 MarkupSafe==1.0
 mccabe==0.2.1
 mock==2.0.0
 monotonic==0.6
 mox3==0.20.0
 msgpack-python==0.4.0
```

### Comparing `oslo.messaging-9.7.2/tools/messages_length.yaml` & `oslo.messaging-9.8.0/tools/messages_length.yaml`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/tools/setup-test-env-amqp1.sh` & `oslo.messaging-9.8.0/tools/setup-test-env-amqp1.sh`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/tools/simulator.py` & `oslo.messaging-9.8.0/tools/simulator.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/tools/test-setup.sh` & `oslo.messaging-9.8.0/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/transport.py` & `oslo.messaging-9.8.0/oslo_messaging/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 __all__ = [
     'DriverLoadFailure',
     'InvalidTransportURL',
     'Transport',
     'TransportHost',
     'TransportURL',
+    'TransportOptions',
     'get_transport',
     'set_transport_defaults',
 ]
 
 LOG = logging.getLogger(__name__)
 
 _transport_opts = [
@@ -112,23 +113,24 @@
         self.conf = driver.conf
         self._driver = driver
 
     def _require_driver_features(self, requeue=False):
         self._driver.require_features(requeue=requeue)
 
     def _send(self, target, ctxt, message, wait_for_reply=None, timeout=None,
-              call_monitor_timeout=None, retry=None):
+              call_monitor_timeout=None, retry=None, transport_options=None):
         if not target.topic:
             raise exceptions.InvalidTarget('A topic is required to send',
                                            target)
         return self._driver.send(target, ctxt, message,
                                  wait_for_reply=wait_for_reply,
                                  timeout=timeout,
                                  call_monitor_timeout=call_monitor_timeout,
-                                 retry=retry)
+                                 retry=retry,
+                                 transport_options=transport_options)
 
     def _send_notification(self, target, ctxt, message, version, retry=None):
         if not target.topic:
             raise exceptions.InvalidTarget('A topic is required to send',
                                            target)
         self._driver.send_notification(target, ctxt, message, version,
                                        retry=retry)
@@ -272,14 +274,24 @@
             v = getattr(self, a)
             if v:
                 attrs.append((a, repr(v)))
         values = ', '.join(['%s=%s' % i for i in attrs])
         return '<TransportHost ' + values + '>'
 
 
+class TransportOptions(object):
+
+    def __init__(self, at_least_once=False):
+        self._at_least_once = at_least_once
+
+    @property
+    def at_least_once(self):
+        return self._at_least_once
+
+
 class TransportURL(object):
 
     """A parsed transport URL.
 
     Transport URLs take the form::
 
       driver://[user:pass@]host:port[,[userN:passN@]hostN:portN]/virtual_host?query
```

### Comparing `oslo.messaging-9.7.2/oslo_messaging/hacking/checks.py` & `oslo.messaging-9.8.0/oslo_messaging/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/_drivers/pool.py` & `oslo.messaging-9.8.0/oslo_messaging/_drivers/pool.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/_drivers/impl_amqp1.py` & `oslo.messaging-9.8.0/oslo_messaging/_drivers/impl_amqp1.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,15 +295,15 @@
             return func(self, *args, **kws)
         return wrap
 
     @_ensure_connect_called
     def send(self, target, ctxt, message,
              wait_for_reply=False,
              timeout=None, call_monitor_timeout=None,
-             retry=None):
+             retry=None, transport_options=None):
         """Send a message to the given target.
 
         :param target: destination for message
         :type target: oslo_messaging.Target
         :param ctxt: message context
         :type ctxt: dict
         :param message: message payload
@@ -318,14 +318,17 @@
             remote side is still executing.
         :type call_monitor_timeout: float
         :param retry: (optional) maximum re-send attempts on recoverable error
                       None or -1 means to retry forever
                       0 means no retry
                       N means N retries
         :type retry: int
+        :param transport_options: transport-specific options to apply to the
+                                  sending of the message (TBD)
+        :type transport_options: dictionary
         """
         request = marshal_request(message, ctxt, None,
                                   call_monitor_timeout)
         if timeout:
             expire = compute_timeout(timeout)
             request.ttl = timeout
             request.expiry_time = compute_timeout(timeout)
```

### Comparing `oslo.messaging-9.7.2/oslo_messaging/_drivers/kafka_driver/kafka_options.py` & `oslo.messaging-9.8.0/oslo_messaging/_drivers/kafka_driver/kafka_options.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/_drivers/amqp.py` & `oslo.messaging-9.8.0/oslo_messaging/_drivers/amqp.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/_drivers/common.py` & `oslo.messaging-9.8.0/oslo_messaging/_drivers/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,15 @@
 # The code inside a connection class is not concurrency safe.
 # Using one Connection class instance for doing both, will result
 # of eventlet complaining of multiple greenthreads that read/write the
 # same fd concurrently... because 'send' and 'listen' run in different
 # greenthread.
 # So, a connection cannot be shared between thread/greenthread and
 # this two variables permit to define the purpose of the connection
-# to allow drivers to add special handling if needed (like heatbeat).
+# to allow drivers to add special handling if needed (like heartbeat).
 # amqp drivers create 3 kind of connections:
 # * driver.listen*(): each call create a new 'PURPOSE_LISTEN' connection
 # * driver.send*(): a pool of 'PURPOSE_SEND' connections is used
 # * driver internally have another 'PURPOSE_LISTEN' connection dedicated
 #   to wait replies of rpc call
 PURPOSE_LISTEN = 'listen'
 PURPOSE_SEND = 'send'
```

### Comparing `oslo.messaging-9.7.2/oslo_messaging/_drivers/amqp1_driver/eventloop.py` & `oslo.messaging-9.8.0/oslo_messaging/_drivers/amqp1_driver/eventloop.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/_drivers/amqp1_driver/addressing.py` & `oslo.messaging-9.8.0/oslo_messaging/_drivers/amqp1_driver/addressing.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/_drivers/amqp1_driver/opts.py` & `oslo.messaging-9.8.0/oslo_messaging/_drivers/amqp1_driver/opts.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/_drivers/amqp1_driver/controller.py` & `oslo.messaging-9.8.0/oslo_messaging/_drivers/amqp1_driver/controller.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/_drivers/amqp1_driver/oslo_messaging_amqp_driver_overview.rst` & `oslo.messaging-9.8.0/oslo_messaging/_drivers/amqp1_driver/oslo_messaging_amqp_driver_overview.rst`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/_drivers/impl_fake.py` & `oslo.messaging-9.8.0/oslo_messaging/_drivers/impl_fake.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,15 +184,16 @@
         jsonutils has some extra logic to automatically convert objects to
         primitive types so that they can be serialized.  We want to catch all
         cases where non-primitive types make it into this code and treat it as
         an error.
         """
         json.dumps(message)
 
-    def _send(self, target, ctxt, message, wait_for_reply=None, timeout=None):
+    def _send(self, target, ctxt, message, wait_for_reply=None, timeout=None,
+              transport_options=None):
         self._check_serialize(message)
 
         exchange = self._exchange_manager.get_exchange(target.exchange)
 
         reply_q = None
         if wait_for_reply:
             reply_q = moves.queue.Queue()
@@ -212,18 +213,19 @@
             except moves.queue.Empty:
                 raise oslo_messaging.MessagingTimeout(
                     'No reply on topic %s' % target.topic)
 
         return None
 
     def send(self, target, ctxt, message, wait_for_reply=None, timeout=None,
-             call_monitor_timeout=None, retry=None):
+             call_monitor_timeout=None, retry=None, transport_options=None):
         # NOTE(sileht): retry doesn't need to be implemented, the fake
         # transport always works
-        return self._send(target, ctxt, message, wait_for_reply, timeout)
+        return self._send(target, ctxt, message, wait_for_reply, timeout,
+                          transport_options)
 
     def send_notification(self, target, ctxt, message, version, retry=None):
         # NOTE(sileht): retry doesn't need to be implemented, the fake
         # transport always works
         self._send(target, ctxt, message)
 
     def listen(self, target, batch_size, batch_timeout):
```

### Comparing `oslo.messaging-9.7.2/oslo_messaging/_drivers/impl_kafka.py` & `oslo.messaging-9.8.0/oslo_messaging/_drivers/impl_kafka.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,15 +395,15 @@
         self.pconn.close()
         for c in self.listeners:
             c.close()
         self.listeners = []
         LOG.info("Kafka messaging driver shutdown")
 
     def send(self, target, ctxt, message, wait_for_reply=None, timeout=None,
-             call_monitor_timeout=None, retry=None):
+             call_monitor_timeout=None, retry=None, transport_options=None):
         raise NotImplementedError(
             'The RPC implementation for Kafka is not implemented')
 
     def send_notification(self, target, ctxt, message, version, retry=None):
         """Send notification to Kafka brokers
 
         :param target: Message destination target
```

### Comparing `oslo.messaging-9.7.2/oslo_messaging/_drivers/impl_rabbit.py` & `oslo.messaging-9.8.0/oslo_messaging/_drivers/impl_rabbit.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 from oslo_messaging._drivers import pool
 from oslo_messaging import _utils
 from oslo_messaging import exceptions
 
 # NOTE(sileht): don't exists in py2 socket module
 TCP_USER_TIMEOUT = 18
 
-
 rabbit_opts = [
     cfg.BoolOpt('ssl',
                 default=False,
                 deprecated_name='rabbit_use_ssl',
                 help='Connect over SSL.'),
     cfg.StrOpt('ssl_version',
                default='',
@@ -531,15 +530,15 @@
 
         # NOTE(sileht): kombu recommend to run heartbeat_check every
         # seconds, but we use a lock around the kombu connection
         # so, to not lock to much this lock to most of the time do nothing
         # expected waiting the events drain, we start heartbeat_check and
         # retrieve the server heartbeat packet only two times more than
         # the minimum required for the heartbeat works
-        # (heatbeat_timeout/heartbeat_rate/2.0, default kombu
+        # (heartbeat_timeout/heartbeat_rate/2.0, default kombu
         # heartbeat_rate is 2)
         self._heartbeat_wait_timeout = (
             float(self.heartbeat_timeout_threshold) /
             float(self.heartbeat_rate) / 2.0)
         self._heartbeat_support_log_emitted = False
 
         # NOTE(sileht): just ensure the connection is setuped at startup
@@ -556,15 +555,15 @@
         LOG.debug('[%(connection_id)s] Connected to AMQP server on '
                   '%(hostname)s:%(port)s via [%(transport)s] client with'
                   ' port %(client_port)s.',
                   self._get_connection_info())
 
         # NOTE(sileht): value chosen according the best practice from kombu
         # http://kombu.readthedocs.org/en/latest/reference/kombu.common.html#kombu.common.eventloop
-        # For heatbeat, we can set a bigger timeout, and check we receive the
+        # For heartbeat, we can set a bigger timeout, and check we receive the
         # heartbeat packets regulary
         if self._heartbeat_supported_and_enabled():
             self._poll_timeout = self._heartbeat_wait_timeout
         else:
             self._poll_timeout = 1
 
         if self._url.startswith('memory://'):
@@ -753,27 +752,36 @@
             ret, channel = autoretry_method()
             self._set_current_channel(channel)
             return ret
         except rpc_amqp.AMQPDestinationNotFound:
             # NOTE(sileht): we must reraise this without
             # trigger error_callback
             raise
+        except exceptions.MessageUndeliverable:
+            # NOTE(gsantomaggio): we must reraise this without
+            # trigger error_callback
+            raise
         except Exception as exc:
             error_callback and error_callback(exc)
             self._set_current_channel(None)
             # NOTE(sileht): number of retry exceeded and the connection
             # is still broken
             info = {'err_str': exc, 'retry': retry}
             info.update(self.connection.info())
             msg = ('Unable to connect to AMQP server on '
                    '%(hostname)s:%(port)s after %(retry)s '
                    'tries: %(err_str)s' % info)
             LOG.error(msg)
             raise exceptions.MessageDeliveryFailure(msg)
 
+    @staticmethod
+    def on_return(exception, exchange, routing_key, message):
+        raise exceptions.MessageUndeliverable(exception, exchange, routing_key,
+                                              message)
+
     def _set_current_channel(self, new_channel):
         """Change the channel to use.
 
         NOTE(sileht): Must be called within the connection lock
         """
         if new_channel == self.channel:
             return
@@ -784,15 +792,16 @@
             self.connection.maybe_close_channel(self.channel)
 
         self.channel = new_channel
 
         if new_channel is not None:
             if self.purpose == rpc_common.PURPOSE_LISTEN:
                 self._set_qos(new_channel)
-            self._producer = kombu.messaging.Producer(new_channel)
+            self._producer = kombu.messaging.Producer(new_channel,
+                                                      on_return=self.on_return)
             for consumer in self._consumers:
                 consumer.declare(self)
 
     def _set_qos(self, channel):
         """Set QoS prefetch count on the channel"""
         if self.rabbit_qos_prefetch_count > 0:
             channel.basic_qos(0,
@@ -949,15 +958,15 @@
                             ConnectRefuseError,
                             OSError,
                             kombu.exceptions.OperationalError) as exc:
                         LOG.info("A recoverable connection/channel error "
                                  "occurred, trying to reconnect: %s", exc)
                         self.ensure_connection()
                 except Exception:
-                    LOG.warning("Unexpected error during heartbeart "
+                    LOG.warning("Unexpected error during heartbeat "
                                 "thread processing, retrying...")
                     LOG.debug('Exception', exc_info=True)
 
             self._heartbeat_exit_event.wait(
                 timeout=self._heartbeat_wait_timeout)
         self._heartbeat_exit_event.clear()
 
@@ -1100,24 +1109,25 @@
                             callback=callback,
                             rabbit_ha_queues=self.rabbit_ha_queues,
                             rabbit_queue_ttl=self.rabbit_transient_queues_ttl)
 
         self.declare_consumer(consumer)
 
     def _ensure_publishing(self, method, exchange, msg, routing_key=None,
-                           timeout=None, retry=None):
+                           timeout=None, retry=None, transport_options=None):
         """Send to a publisher based on the publisher class."""
 
         def _error_callback(exc):
             log_info = {'topic': exchange.name, 'err_str': exc}
             LOG.error("Failed to publish message to topic "
                       "'%(topic)s': %(err_str)s", log_info)
             LOG.debug('Exception', exc_info=exc)
 
-        method = functools.partial(method, exchange, msg, routing_key, timeout)
+        method = functools.partial(method, exchange, msg, routing_key,
+                                   timeout, transport_options)
 
         with self._connection_lock:
             self.ensure(method, retry=retry, error_callback=_error_callback)
 
     def _get_connection_info(self, conn_error=False):
         # Bug #1745166: set 'conn_error' true if this is being called when the
         # connection is in a known error state.  Otherwise attempting to access
@@ -1131,38 +1141,43 @@
                 hasattr(self.channel.connection, 'sock') and
                 self.channel.connection.sock):
             client_port = self.channel.connection.sock.getsockname()[1]
         info.update({'client_port': client_port,
                      'connection_id': self.connection_id})
         return info
 
-    def _publish(self, exchange, msg, routing_key=None, timeout=None):
+    def _publish(self, exchange, msg, routing_key=None, timeout=None,
+                 transport_options=None):
         """Publish a message."""
 
         if not (exchange.passive or exchange.name in self._declared_exchanges):
                 exchange(self.channel).declare()
                 self._declared_exchanges.add(exchange.name)
 
         log_info = {'msg': msg,
                     'who': exchange or 'default',
-                    'key': routing_key}
+                    'key': routing_key,
+                    'transport_options': str(transport_options)}
         LOG.trace('Connection._publish: sending message %(msg)s to'
                   ' %(who)s with routing key %(key)s', log_info)
-
         # NOTE(sileht): no need to wait more, caller expects
         # a answer before timeout is reached
         with self._transport_socket_timeout(timeout):
-            self._producer.publish(msg,
-                                   exchange=exchange,
-                                   routing_key=routing_key,
-                                   expiration=timeout,
-                                   compression=self.kombu_compression)
+            self._producer.publish(
+                msg,
+                mandatory=transport_options.at_least_once if
+                transport_options else False,
+                exchange=exchange,
+                routing_key=routing_key,
+                expiration=timeout,
+                compression=self.kombu_compression)
 
     def _publish_and_creates_default_queue(self, exchange, msg,
-                                           routing_key=None, timeout=None):
+                                           routing_key=None, timeout=None,
+                                           transport_options=None):
         """Publisher that declares a default queue
 
         When the exchange is missing instead of silently creates an exchange
         not binded to a queue, this publisher creates a default queue
         named with the routing_key
 
         This is mainly used to not miss notification in case of nobody consumes
@@ -1191,23 +1206,24 @@
             queue.declare()
             self._declared_queues.add(queue_indentifier)
 
         self._publish(exchange, msg, routing_key=routing_key, timeout=timeout)
 
     def _publish_and_raises_on_missing_exchange(self, exchange, msg,
                                                 routing_key=None,
-                                                timeout=None):
+                                                timeout=None,
+                                                transport_options=None):
         """Publisher that raises exception if exchange is missing."""
         if not exchange.passive:
             raise RuntimeError("_publish_and_retry_on_missing_exchange() must "
                                "be called with an passive exchange.")
 
         try:
             self._publish(exchange, msg, routing_key=routing_key,
-                          timeout=timeout)
+                          timeout=timeout, transport_options=transport_options)
             return
         except self.connection.channel_errors as exc:
             if exc.code == 404:
                 # NOTE(noelbk/sileht):
                 # If rabbit dies, the consumer can be disconnected before the
                 # publisher sends, and if the consumer hasn't declared the
                 # queue, the publisher's will send a message to an exchange
@@ -1226,25 +1242,27 @@
                                          durable=False,
                                          auto_delete=True,
                                          passive=True)
 
         self._ensure_publishing(self._publish_and_raises_on_missing_exchange,
                                 exchange, msg, routing_key=msg_id)
 
-    def topic_send(self, exchange_name, topic, msg, timeout=None, retry=None):
+    def topic_send(self, exchange_name, topic, msg, timeout=None, retry=None,
+                   transport_options=None):
         """Send a 'topic' message."""
         exchange = kombu.entity.Exchange(
             name=exchange_name,
             type='topic',
             durable=self.amqp_durable_queues,
             auto_delete=self.amqp_auto_delete)
 
         self._ensure_publishing(self._publish, exchange, msg,
                                 routing_key=topic, timeout=timeout,
-                                retry=retry)
+                                retry=retry,
+                                transport_options=transport_options)
 
     def fanout_send(self, topic, msg, retry=None):
         """Send a 'fanout' message."""
         exchange = kombu.entity.Exchange(name='%s_fanout' % topic,
                                          type='fanout',
                                          durable=False,
                                          auto_delete=True)
```

### Comparing `oslo.messaging-9.7.2/oslo_messaging/_drivers/base.py` & `oslo.messaging-9.8.0/oslo_messaging/_drivers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import threading
 
 from oslo_config import cfg
 from oslo_utils import excutils
 from oslo_utils import timeutils
 import six
 
-
 from oslo_messaging import exceptions
 
 base_opts = [
     cfg.IntOpt('rpc_conn_pool_size', default=30,
                deprecated_group='DEFAULT',
                help='Size of RPC connection pool.'),
     cfg.IntOpt('conn_pool_min_size', default=2,
@@ -37,14 +36,15 @@
 def batch_poll_helper(func):
     """Decorator to poll messages in batch
 
     This decorator is used to add message batching support to a
     :py:meth:`PollStyleListener.poll` implementation that only polls for a
     single message per call.
     """
+
     def wrapper(in_self, timeout=None, batch_size=1, batch_timeout=None):
         incomings = []
         driver_prefetch = in_self.prefetch_size
         if driver_prefetch > 0:
             batch_size = min(batch_size, driver_prefetch)
         timeout = batch_timeout or timeout
 
@@ -53,14 +53,15 @@
                 message = func(in_self, timeout=watch.leftover(True))
                 if message is not None:
                     incomings.append(message)
                 if len(incomings) == batch_size or message is None:
                     break
 
         return incomings
+
     return wrapper
 
 
 class TransportDriverError(exceptions.MessagingException):
     """Base class for transport driver specific exceptions."""
 
 
@@ -240,17 +241,17 @@
         processing
     :type batch_timeout: float
     :param prefetch_size: defines how many messages we want to prefetch
         from the messaging backend in a single request. May not be honored by
         all backend implementations.
     :type prefetch_size: int
     """
+
     def __init__(self, batch_size, batch_timeout,
                  prefetch_size=-1):
-
         self.on_incoming_callback = None
         self.batch_timeout = batch_timeout
         self.prefetch_size = prefetch_size
         if prefetch_size > 0:
             batch_size = min(batch_size, prefetch_size)
         self.batch_size = batch_size
 
@@ -279,14 +280,15 @@
         """
 
 
 class PollStyleListenerAdapter(Listener):
     """A Listener that uses a PollStyleListener for message transfer. A
     dedicated thread is created to do message polling.
     """
+
     def __init__(self, poll_style_listener, batch_size, batch_timeout):
         super(PollStyleListenerAdapter, self).__init__(
             batch_size, batch_timeout, poll_style_listener.prefetch_size
         )
         self._poll_style_listener = poll_style_listener
         self._listen_thread = threading.Thread(target=self._runner)
         self._listen_thread.daemon = True
@@ -360,15 +362,15 @@
         if requeue:
             raise NotImplementedError('Message requeueing not supported by '
                                       'this transport driver')
 
     @abc.abstractmethod
     def send(self, target, ctxt, message,
              wait_for_reply=None, timeout=None, call_monitor_timeout=None,
-             retry=None):
+             retry=None, transport_options=None):
         """Send a message to the given target and optionally wait for a reply.
         This method is used by the RPC client when sending RPC requests to a
         server.
 
         The driver must use the *topic*, *exchange*, and *server* (if present)
         attributes of the *target* to construct the backend-native message
         address. The message address must match the format used by
@@ -430,14 +432,18 @@
         :type timeout: float
         :param call_monitor_timeout: Maximum time the client will wait for the
             call to complete or receive a message heartbeat indicating the
             remote side is still executing.
         :type call_monitor_timeout: float
         :param retry: maximum message send attempts permitted
         :type retry: int
+        :param transport_options: additional parameters to configure the driver
+                                  for example to send parameters as "mandatory"
+                                  flag in RabbitMQ
+        :type transport_options: dictionary
         :returns: A reply message or None if no reply expected
         :raises: :py:exc:`MessagingException`, any exception thrown by the
             remote server when executing the RPC call.
         """
 
     @abc.abstractmethod
     def send_notification(self, target, ctxt, message, version, retry):
```

### Comparing `oslo.messaging-9.7.2/oslo_messaging/_drivers/amqpdriver.py` & `oslo.messaging-9.8.0/oslo_messaging/_drivers/amqpdriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -576,15 +576,15 @@
             self._reply_q = reply_q
             self._reply_q_conn = conn
 
         return self._reply_q
 
     def _send(self, target, ctxt, message,
               wait_for_reply=None, timeout=None, call_monitor_timeout=None,
-              envelope=True, notify=False, retry=None):
+              envelope=True, notify=False, retry=None, transport_options=None):
 
         msg = message
 
         if wait_for_reply:
             msg_id = uuid.uuid4().hex
             msg.update({'_msg_id': msg_id})
             msg.update({'_reply_q': self._get_reply_q()})
@@ -622,30 +622,32 @@
                     exchange = self._get_exchange(target)
                     if target.server:
                         topic = '%s.%s' % (target.topic, target.server)
                     LOG.debug(log_msg + "exchange '%(exchange)s'"
                               " topic '%(topic)s'", {'exchange': exchange,
                                                      'topic': topic})
                     conn.topic_send(exchange_name=exchange, topic=topic,
-                                    msg=msg, timeout=timeout, retry=retry)
+                                    msg=msg, timeout=timeout, retry=retry,
+                                    transport_options=transport_options)
 
             if wait_for_reply:
                 result = self._waiter.wait(msg_id, timeout,
                                            call_monitor_timeout)
                 if isinstance(result, Exception):
                     raise result
                 return result
         finally:
             if wait_for_reply:
                 self._waiter.unlisten(msg_id)
 
     def send(self, target, ctxt, message, wait_for_reply=None, timeout=None,
-             call_monitor_timeout=None, retry=None):
+             call_monitor_timeout=None, retry=None, transport_options=None):
         return self._send(target, ctxt, message, wait_for_reply, timeout,
-                          call_monitor_timeout, retry=retry)
+                          call_monitor_timeout, retry=retry,
+                          transport_options=transport_options)
 
     def send_notification(self, target, ctxt, message, version, retry=None):
         return self._send(target, ctxt, message,
                           envelope=(version == 2.0), notify=True, retry=retry)
 
     def listen(self, target, batch_size, batch_timeout):
         conn = self._get_connection(rpc_common.PURPOSE_LISTEN)
```

### Comparing `oslo.messaging-9.7.2/oslo_messaging/exceptions.py` & `oslo.messaging-9.8.0/oslo_messaging/exceptions.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import six
 
 __all__ = ['MessagingException', 'MessagingTimeout', 'MessageDeliveryFailure',
-           'InvalidTarget']
+           'InvalidTarget', 'MessageUndeliverable']
 
 
 class MessagingException(Exception):
     """Base class for exceptions."""
 
 
 class MessagingTimeout(MessagingException):
@@ -34,7 +34,18 @@
 class InvalidTarget(MessagingException, ValueError):
     """Raised if a target does not meet certain pre-conditions."""
 
     def __init__(self, msg, target):
         msg = msg + ":" + six.text_type(target)
         super(InvalidTarget, self).__init__(msg)
         self.target = target
+
+
+class MessageUndeliverable(Exception):
+    """Raised if message is not routed with mandatory flag"""
+
+    def __init__(self, exception, exchange, routing_key, message):
+        super(MessageUndeliverable, self).__init__()
+        self.exception = exception
+        self.exchange = exchange
+        self.routing_key = routing_key
+        self.message = message
```

### Comparing `oslo.messaging-9.7.2/oslo_messaging/target.py` & `oslo.messaging-9.8.0/oslo_messaging/target.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/server.py` & `oslo.messaging-9.8.0/oslo_messaging/server.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/_utils.py` & `oslo.messaging-9.8.0/oslo_messaging/_utils.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/notify/messaging.py` & `oslo.messaging-9.8.0/oslo_messaging/notify/messaging.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/notify/filter.py` & `oslo.messaging-9.8.0/oslo_messaging/notify/filter.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/notify/listener.py` & `oslo.messaging-9.8.0/oslo_messaging/notify/listener.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/notify/logger.py` & `oslo.messaging-9.8.0/oslo_messaging/notify/logger.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/notify/_impl_log.py` & `oslo.messaging-9.8.0/oslo_messaging/notify/_impl_log.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/notify/middleware.py` & `oslo.messaging-9.8.0/oslo_messaging/notify/middleware.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/notify/_impl_routing.py` & `oslo.messaging-9.8.0/oslo_messaging/notify/_impl_routing.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/notify/dispatcher.py` & `oslo.messaging-9.8.0/oslo_messaging/notify/dispatcher.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/notify/_impl_noop.py` & `oslo.messaging-9.8.0/oslo_messaging/notify/_impl_noop.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/notify/log_handler.py` & `oslo.messaging-9.8.0/oslo_messaging/notify/log_handler.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/notify/_impl_test.py` & `oslo.messaging-9.8.0/oslo_messaging/notify/_impl_test.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/notify/__init__.py` & `oslo.messaging-9.8.0/oslo_messaging/notify/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/notify/notifier.py` & `oslo.messaging-9.8.0/oslo_messaging/notify/notifier.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/conffixture.py` & `oslo.messaging-9.8.0/oslo_messaging/conffixture.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/opts.py` & `oslo.messaging-9.8.0/oslo_messaging/opts.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/dispatcher.py` & `oslo.messaging-9.8.0/oslo_messaging/dispatcher.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/test_config_opts_proxy.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/test_config_opts_proxy.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/test_utils.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/test_opts.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/test_opts.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/test_transport.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/test_transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,16 @@
 
         t._driver.send.assert_called_once_with(self._target,
                                                'ctxt',
                                                'message',
                                                wait_for_reply=None,
                                                timeout=None,
                                                call_monitor_timeout=None,
-                                               retry=None)
+                                               retry=None,
+                                               transport_options=None)
 
     def test_send_all_args(self):
         t = transport.Transport(_FakeDriver(cfg.CONF))
 
         t._driver.send = mock.Mock()
 
         t._send(self._target, 'ctxt', 'message',
@@ -246,15 +247,16 @@
         t._driver.send.\
             assert_called_once_with(self._target,
                                     'ctxt',
                                     'message',
                                     wait_for_reply='wait_for_reply',
                                     timeout='timeout',
                                     call_monitor_timeout='cm_timeout',
-                                    retry='retry')
+                                    retry='retry',
+                                    transport_options=None)
 
     def test_send_notification(self):
         t = transport.Transport(_FakeDriver(cfg.CONF))
 
         t._driver.send_notification = mock.Mock()
 
         t._send_notification(self._target, 'ctxt', 'message', version=1.0)
```

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/test_exception_serialization.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/test_exception_serialization.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/test_urls.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/notify/test_listener.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/notify/test_listener.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/notify/test_log_handler.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/notify/test_log_handler.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/notify/test_logger.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/notify/test_logger.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/notify/test_middleware.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/notify/test_middleware.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/notify/test_notifier.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/notify/test_notifier.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/notify/test_dispatcher.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/notify/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/drivers/test_amqp_driver.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/drivers/test_amqp_driver.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/drivers/test_pool.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/drivers/test_pool.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/drivers/test_impl_kafka.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/drivers/test_impl_kafka.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/drivers/test_impl_rabbit.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/drivers/test_impl_rabbit.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,27 +195,29 @@
             conn._publish(exchange_mock, 'msg', routing_key='routing_key',
                           timeout=1)
 
         fake_publish.assert_called_with(
             'msg', expiration=1,
             exchange=exchange_mock,
             compression=self.conf.oslo_messaging_rabbit.kombu_compression,
+            mandatory=False,
             routing_key='routing_key')
 
     @mock.patch('kombu.messaging.Producer.publish')
     def test_send_no_timeout(self, fake_publish):
         transport = oslo_messaging.get_transport(self.conf,
                                                  'kombu+memory:////')
         exchange_mock = mock.Mock()
         with transport._driver._get_connection(
                 driver_common.PURPOSE_SEND) as pool_conn:
             conn = pool_conn.connection
             conn._publish(exchange_mock, 'msg', routing_key='routing_key')
         fake_publish.assert_called_with(
             'msg', expiration=None,
+            mandatory=False,
             compression=self.conf.oslo_messaging_rabbit.kombu_compression,
             exchange=exchange_mock,
             routing_key='routing_key')
 
     def test_declared_queue_publisher(self):
         transport = oslo_messaging.get_transport(self.conf,
                                                  'kombu+memory:////')
```

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/functional/test_rabbitmq.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/functional/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/functional/notify/test_logger.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/functional/notify/test_logger.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/functional/utils.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/functional/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,18 +222,23 @@
     def __call__(self, **kwargs):
         self.context['time'] = time.ctime()
         self.context['cast'] = True
         self.client.cast(self.context, self.method, **kwargs)
 
 
 class ClientStub(object):
-    def __init__(self, transport, target, cast=False, name=None, **kwargs):
+    def __init__(self, transport, target, cast=False, name=None,
+                 transport_options=None, **kwargs):
         self.name = name or "functional-tests"
         self.cast = cast
-        self.client = oslo_messaging.RPCClient(transport, target, **kwargs)
+        self.client = oslo_messaging.RPCClient(
+            transport=transport,
+            target=target,
+            transport_options=transport_options,
+            **kwargs)
 
     def __getattr__(self, name):
         context = {"application": self.name}
         if self.cast:
             return RpcCast(self.client, name, context)
         else:
             return RpcCall(self.client, name, context)
```

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/functional/test_functional.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/functional/test_functional.py`

 * *Files 6% similar despite different names*

```diff
@@ -148,14 +148,48 @@
         with concurrent.futures.ThreadPoolExecutor(max_workers=2) as executor:
             future = executor.submit(client.long_running_task, seconds=10)
             executor.submit(short_periodical_tasks)
             self.assertRaises(oslo_messaging.MessagingTimeout, future.result)
 
         self.assertEqual(10, server.endpoint.ival)
 
+    def test_mandatory_call(self):
+        if not self.url.startswith("rabbit://"):
+            self.skipTest("backend does not support call monitoring")
+
+        transport = self.useFixture(utils.RPCTransportFixture(self.conf,
+                                                              self.url))
+        target = oslo_messaging.Target(topic='topic_' + str(uuid.uuid4()),
+                                       server='server_' + str(uuid.uuid4()))
+
+        # test for mandatory flag using transport-options, see:
+        # https://blueprints.launchpad.net/oslo.messaging/+spec/transport-options
+        # first test with `at_least_once=False` raises a "MessagingTimeout"
+        # error since there is no control if the queue actually exists.
+        # (Default behavior)
+        options = oslo_messaging.TransportOptions(at_least_once=False)
+        client1 = utils.ClientStub(transport.transport, target,
+                                   cast=False, timeout=1,
+                                   transport_options=options)
+
+        self.assertRaises(oslo_messaging.MessagingTimeout,
+                          client1.delay)
+
+        # second test with `at_least_once=True` raises a "MessageUndeliverable"
+        # caused by mandatory flag.
+        # the MessageUndeliverable error is raised immediately without waiting
+        # any timeout
+        options2 = oslo_messaging.TransportOptions(at_least_once=True)
+        client2 = utils.ClientStub(transport.transport, target,
+                                   cast=False, timeout=60,
+                                   transport_options=options2)
+
+        self.assertRaises(oslo_messaging.MessageUndeliverable,
+                          client2.delay)
+
     def test_monitor_long_call(self):
         if not (self.url.startswith("rabbit://") or
                 self.url.startswith("amqp://")):
             self.skipTest("backend does not support call monitoring")
 
         transport = self.useFixture(utils.RPCTransportFixture(self.conf,
                                                               self.url))
```

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/test_target.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/test_fixture.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/utils.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/utils.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/test_expected_exceptions.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/test_expected_exceptions.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/__init__.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/rpc/test_server.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/rpc/test_server.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/rpc/test_dispatcher.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/rpc/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/tests/rpc/test_client.py` & `oslo.messaging-9.8.0/oslo_messaging/tests/rpc/test_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,30 +38,61 @@
          dict(call=True,
               ctxt=dict(user='testuser', project='testtenant'),
               args=dict(bar='blaa', foobar=11.01))),
     ]
 
     def test_cast_call(self):
         self.config(rpc_response_timeout=None)
+        transport_options = oslo_messaging.TransportOptions()
+        transport = oslo_messaging.get_rpc_transport(self.conf, url='fake:')
+        client = oslo_messaging.RPCClient(transport, oslo_messaging.Target(),
+                                          transport_options=transport_options)
+
+        transport._send = mock.Mock()
+
+        msg = dict(method='foo', args=self.args)
+        kwargs = {'retry': None, 'transport_options': transport_options}
+        if self.call:
+            kwargs['wait_for_reply'] = True
+            kwargs['timeout'] = None
+            kwargs['call_monitor_timeout'] = None
+
+        method = client.call if self.call else client.cast
+        method(self.ctxt, 'foo', **self.args)
+        self.assertFalse(transport_options.at_least_once)
+        transport._send.assert_called_once_with(oslo_messaging.Target(),
+                                                self.ctxt,
+                                                msg,
+                                                **kwargs)
+
+    def test_cast_call_with_transport_options(self):
+        self.config(rpc_response_timeout=None)
 
         transport = oslo_messaging.get_rpc_transport(self.conf, url='fake:')
-        client = oslo_messaging.RPCClient(transport, oslo_messaging.Target())
+
+        transport_options = oslo_messaging.TransportOptions(at_least_once=True)
+        client = oslo_messaging.RPCClient(
+            transport,
+            oslo_messaging.Target(),
+            transport_options=transport_options)
 
         transport._send = mock.Mock()
 
         msg = dict(method='foo', args=self.args)
-        kwargs = {'retry': None}
+        kwargs = {'retry': None,
+                  'transport_options': transport_options}
         if self.call:
             kwargs['wait_for_reply'] = True
             kwargs['timeout'] = None
             kwargs['call_monitor_timeout'] = None
 
         method = client.call if self.call else client.cast
         method(self.ctxt, 'foo', **self.args)
 
+        self.assertTrue(transport_options.at_least_once)
         transport._send.assert_called_once_with(oslo_messaging.Target(),
                                                 self.ctxt,
                                                 msg,
                                                 **kwargs)
 
 
 class TestCastToTarget(test_utils.BaseTestCase):
@@ -199,15 +230,16 @@
             if self.double_prepare:
                 client = client.prepare(**self.prepare)
         client.cast({}, 'foo')
 
         transport._send.assert_called_once_with(expect_target,
                                                 {},
                                                 msg,
-                                                retry=None)
+                                                retry=None,
+                                                transport_options=None)
 
 
 TestCastToTarget.generate_scenarios()
 
 
 _notset = object()
 
@@ -241,15 +273,15 @@
                                           timeout=self.ctor,
                                           call_monitor_timeout=self.cm)
 
         transport._send = mock.Mock()
 
         msg = dict(method='foo', args={})
         kwargs = dict(wait_for_reply=True, timeout=self.expect, retry=None,
-                      call_monitor_timeout=self.cm)
+                      call_monitor_timeout=self.cm, transport_options=None)
 
         if self.prepare is not _notset:
             client = client.prepare(timeout=self.prepare)
         client.call({}, 'foo')
 
         transport._send.assert_called_once_with(oslo_messaging.Target(),
                                                 {},
@@ -273,15 +305,16 @@
         client = oslo_messaging.RPCClient(transport, oslo_messaging.Target(),
                                           retry=self.ctor)
 
         transport._send = mock.Mock()
 
         msg = dict(method='foo', args={})
         kwargs = dict(wait_for_reply=True, timeout=60,
-                      retry=self.expect, call_monitor_timeout=None)
+                      retry=self.expect, call_monitor_timeout=None,
+                      transport_options=None)
 
         if self.prepare is not _notset:
             client = client.prepare(retry=self.prepare)
         client.call({}, 'foo')
 
         transport._send.assert_called_once_with(oslo_messaging.Target(),
                                                 {},
@@ -330,16 +363,16 @@
         transport = oslo_messaging.get_rpc_transport(self.conf, url='fake:')
         serializer = msg_serializer.NoOpSerializer()
 
         client = oslo_messaging.RPCClient(transport, oslo_messaging.Target(),
                                           serializer=serializer)
 
         transport._send = mock.Mock()
-
-        kwargs = dict(wait_for_reply=True, timeout=None) if self.call else {}
+        kwargs = dict(wait_for_reply=True,
+                      timeout=None) if self.call else {}
         kwargs['retry'] = None
         if self.call:
             kwargs['call_monitor_timeout'] = None
 
         transport._send.return_value = self.retval
 
         serializer.serialize_entity = mock.Mock()
@@ -363,14 +396,15 @@
         retval = method(self.ctxt, 'foo', **self.args)
         if self.retval is not None:
             self.assertEqual('d' + self.retval, retval)
 
         transport._send.assert_called_once_with(oslo_messaging.Target(),
                                                 dict(user='alice'),
                                                 msg,
+                                                transport_options=None,
                                                 **kwargs)
         expected_calls = [mock.call(self.ctxt, arg) for arg in self.args]
         self.assertEqual(expected_calls,
                          serializer.serialize_entity.mock_calls)
         if self.call:
             serializer.deserialize_entity.assert_called_once_with(self.ctxt,
                                                                   self.retval)
@@ -462,15 +496,17 @@
         try:
             method({}, 'foo')
         except Exception as ex:
             self.assertIsInstance(ex, oslo_messaging.RPCVersionCapError, ex)
             self.assertFalse(self.success)
         else:
             self.assertTrue(self.success)
-            transport._send.assert_called_once_with(target, {}, msg, **kwargs)
+            transport._send.assert_called_once_with(target, {}, msg,
+                                                    transport_options=None,
+                                                    **kwargs)
 
 TestVersionCap.generate_scenarios()
 
 
 class TestCanSendVersion(test_utils.BaseTestCase):
 
     scenarios = [
```

### Comparing `oslo.messaging-9.7.2/oslo_messaging/version.py` & `oslo.messaging-9.8.0/oslo_messaging/version.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/__init__.py` & `oslo.messaging-9.8.0/oslo_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/rpc/transport.py` & `oslo.messaging-9.8.0/oslo_messaging/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/rpc/client.py` & `oslo.messaging-9.8.0/oslo_messaging/rpc/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Copyright 2010 United States Government as represented by the
 # Administrator of the National Aeronautics and Space Administration.
 # All Rights Reserved.
 # Copyright 2013 Red Hat, Inc.
 #
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
@@ -41,15 +40,14 @@
     cfg.IntOpt('rpc_response_timeout',
                default=60,
                help='Seconds to wait for a response from a call.'),
 ]
 
 
 class RemoteError(exceptions.MessagingException):
-
     """Signifies that a remote endpoint method has raised an exception.
 
     Contains a string representation of the type of the original exception,
     the value of the original exception, and the traceback.  These are
     sent to the parent as a joined string so printing the exception
     contains all of the relevant info.
     """
@@ -90,24 +88,25 @@
 @six.add_metaclass(abc.ABCMeta)
 class _BaseCallContext(object):
 
     _marker = object()
 
     def __init__(self, transport, target, serializer,
                  timeout=None, version_cap=None, retry=None,
-                 call_monitor_timeout=None):
+                 call_monitor_timeout=None, transport_options=None):
         self.conf = transport.conf
 
         self.transport = transport
         self.target = target
         self.serializer = serializer
         self.timeout = timeout
         self.call_monitor_timeout = call_monitor_timeout
         self.retry = retry
         self.version_cap = version_cap
+        self.transport_options = transport_options
 
         super(_BaseCallContext, self).__init__()
 
     def _make_message(self, ctxt, method, args):
         msg = dict(method=method)
 
         msg['args'] = dict()
@@ -146,15 +145,17 @@
         """Invoke a method and return immediately. See RPCClient.cast()."""
         msg = self._make_message(ctxt, method, kwargs)
         msg_ctxt = self.serializer.serialize_context(ctxt)
 
         self._check_version_cap(msg.get('version'))
 
         try:
-            self.transport._send(self.target, msg_ctxt, msg, retry=self.retry)
+            self.transport._send(self.target, msg_ctxt, msg,
+                                 retry=self.retry,
+                                 transport_options=self.transport_options)
         except driver_base.TransportDriverError as ex:
             raise ClientSendError(self.target, ex)
 
     def call(self, ctxt, method, **kwargs):
         """Invoke a method and wait for a reply. See RPCClient.call()."""
         if self.target.fanout:
             raise exceptions.InvalidTarget('A call cannot be used with fanout',
@@ -168,41 +169,42 @@
             timeout = self.conf.rpc_response_timeout
 
         cm_timeout = self.call_monitor_timeout
 
         self._check_version_cap(msg.get('version'))
 
         try:
-            result = self.transport._send(self.target, msg_ctxt, msg,
-                                          wait_for_reply=True, timeout=timeout,
-                                          call_monitor_timeout=cm_timeout,
-                                          retry=self.retry)
+            result = \
+                self.transport._send(self.target, msg_ctxt, msg,
+                                     wait_for_reply=True, timeout=timeout,
+                                     call_monitor_timeout=cm_timeout,
+                                     retry=self.retry,
+                                     transport_options=self.transport_options)
         except driver_base.TransportDriverError as ex:
             raise ClientSendError(self.target, ex)
 
         return self.serializer.deserialize_entity(ctxt, result)
 
     @abc.abstractmethod
     def prepare(self, exchange=_marker, topic=_marker, namespace=_marker,
                 version=_marker, server=_marker, fanout=_marker,
                 timeout=_marker, version_cap=_marker, retry=_marker,
                 call_monitor_timeout=_marker):
         """Prepare a method invocation context. See RPCClient.prepare()."""
 
 
 class _CallContext(_BaseCallContext):
-
     _marker = _BaseCallContext._marker
 
     @classmethod
     def _prepare(cls, call_context,
                  exchange=_marker, topic=_marker, namespace=_marker,
                  version=_marker, server=_marker, fanout=_marker,
                  timeout=_marker, version_cap=_marker, retry=_marker,
-                 call_monitor_timeout=_marker):
+                 call_monitor_timeout=_marker, transport_options=_marker):
         cls._check_version(version)
         kwargs = dict(
             exchange=exchange,
             topic=topic,
             namespace=namespace,
             version=version,
             server=server,
@@ -215,33 +217,34 @@
             timeout = call_context.timeout
         if version_cap is cls._marker:
             version_cap = call_context.version_cap
         if retry is cls._marker:
             retry = call_context.retry
         if call_monitor_timeout is cls._marker:
             call_monitor_timeout = call_context.call_monitor_timeout
+        if transport_options is cls._marker:
+            transport_options = call_context.transport_options
 
         return _CallContext(call_context.transport, target,
                             call_context.serializer,
                             timeout, version_cap, retry,
-                            call_monitor_timeout)
+                            call_monitor_timeout, transport_options)
 
     def prepare(self, exchange=_marker, topic=_marker, namespace=_marker,
                 version=_marker, server=_marker, fanout=_marker,
                 timeout=_marker, version_cap=_marker, retry=_marker,
                 call_monitor_timeout=_marker):
         return _CallContext._prepare(self,
                                      exchange, topic, namespace,
                                      version, server, fanout,
                                      timeout, version_cap, retry,
                                      call_monitor_timeout)
 
 
 class RPCClient(_BaseCallContext):
-
     """A class for invoking methods on remote RPC servers.
 
     The RPCClient class is responsible for sending method invocations to and
     receiving return values from remote RPC servers via a messaging transport.
 
     Two RPC patterns are supported: RPC calls and RPC casts.
 
@@ -322,15 +325,15 @@
             LOG.error("Failed to send ping message")
     """
 
     _marker = _BaseCallContext._marker
 
     def __init__(self, transport, target,
                  timeout=None, version_cap=None, serializer=None, retry=None,
-                 call_monitor_timeout=None):
+                 call_monitor_timeout=None, transport_options=None):
         """Construct an RPC client.
 
         :param transport: a messaging transport handle
         :type transport: Transport
         :param target: the default target for invocations
         :type target: Target
         :param timeout: an optional default timeout (in seconds) for call()s
@@ -358,23 +361,23 @@
         if not isinstance(transport, msg_transport.RPCTransport):
             LOG.warning("Using notification transport for RPC. Please use "
                         "get_rpc_transport to obtain an RPC transport "
                         "instance.")
 
         super(RPCClient, self).__init__(
             transport, target, serializer, timeout, version_cap, retry,
-            call_monitor_timeout
+            call_monitor_timeout, transport_options
         )
 
         self.conf.register_opts(_client_opts)
 
     def prepare(self, exchange=_marker, topic=_marker, namespace=_marker,
                 version=_marker, server=_marker, fanout=_marker,
                 timeout=_marker, version_cap=_marker, retry=_marker,
-                call_monitor_timeout=_marker):
+                call_monitor_timeout=_marker, transport_options=_marker):
         """Prepare a method invocation context.
 
         Use this method to override client properties for an individual method
         invocation. For example::
 
             def test(self, ctxt, arg):
                 cctxt = self.prepare(version='2.5')
@@ -397,27 +400,31 @@
         :param version_cap: raise a RPCVersionCapError version exceeds this cap
         :type version_cap: str
         :param retry: an optional connection retries configuration:
                       None or -1 means to retry forever.
                       0 means no retry is attempted.
                       N means attempt at most N retries.
         :type retry: int
+        :param transport_options: additional parameters to configure the driver
+                                  for example to send parameters as "mandatory"
+                                  flag in RabbitMQ
+        :type transport_options: dictionary
         :param call_monitor_timeout: an optional timeout (in seconds) for
                                      active call heartbeating. If specified,
                                      requires the server to heartbeat
                                      long-running calls at this interval
                                      (less than the overall timeout
                                      parameter).
         :type call_monitor_timeout: int
         """
         return _CallContext._prepare(self,
                                      exchange, topic, namespace,
                                      version, server, fanout,
                                      timeout, version_cap, retry,
-                                     call_monitor_timeout)
+                                     call_monitor_timeout, transport_options)
 
     def cast(self, ctxt, method, **kwargs):
         """Invoke a method without blocking for a return value.
 
         The cast() method is used to invoke an RPC method that does not return
         a value.  cast() RPC requests may be broadcast to all Servers listening
         on a given topic by setting the fanout Target property to ``True``.
```

### Comparing `oslo.messaging-9.7.2/oslo_messaging/rpc/server.py` & `oslo.messaging-9.8.0/oslo_messaging/rpc/server.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/rpc/dispatcher.py` & `oslo.messaging-9.8.0/oslo_messaging/rpc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/rpc/__init__.py` & `oslo.messaging-9.8.0/oslo_messaging/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo_messaging/serializer.py` & `oslo.messaging-9.8.0/oslo_messaging/serializer.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/ChangeLog` & `oslo.messaging-9.8.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 CHANGES
 =======
 
+9.8.0
+-----
+
+* Add Python 3 Train unit tests
+* Implement mandatory flag for RabbitMQ driver
+* Implement the transport options
+* Add the "transport\_options" parameter to the amqp1 and kafka drivers
+* fix typos
+* Add transport\_options parameter
+* Download kafka from archive.apache.org
+
 9.7.2
 -----
 
 
 9.7.1
 -----
```

### Comparing `oslo.messaging-9.7.2/LICENSE` & `oslo.messaging-9.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/playbooks/oslo.messaging-telemetry-dsvm-integration-kafka/run.yaml` & `oslo.messaging-9.8.0/playbooks/oslo.messaging-telemetry-dsvm-integration-kafka/run.yaml`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/playbooks/oslo.messaging-telemetry-dsvm-integration-kafka/post.yaml` & `oslo.messaging-9.8.0/playbooks/oslo.messaging-telemetry-dsvm-integration-amqp1/post.yaml`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/playbooks/oslo.messaging-src-grenade-dsvm/run.yaml` & `oslo.messaging-9.8.0/playbooks/oslo.messaging-src-grenade-dsvm/run.yaml`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/playbooks/oslo.messaging-telemetry-dsvm-integration-amqp1/run.yaml` & `oslo.messaging-9.8.0/playbooks/oslo.messaging-telemetry-dsvm-integration-amqp1/run.yaml`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/playbooks/oslo.messaging-telemetry-dsvm-integration-amqp1/post.yaml` & `oslo.messaging-9.8.0/playbooks/oslo.messaging-telemetry-dsvm-integration-rabbit/post.yaml`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/playbooks/oslo.messaging-telemetry-dsvm-integration-rabbit/run.yaml` & `oslo.messaging-9.8.0/playbooks/oslo.messaging-telemetry-dsvm-integration-rabbit/run.yaml`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/playbooks/oslo.messaging-telemetry-dsvm-integration-rabbit/post.yaml` & `oslo.messaging-9.8.0/playbooks/oslo.messaging-telemetry-dsvm-integration-kafka/post.yaml`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/playbooks/oslo.messaging-src-grenade-dsvm-multinode/run.yaml` & `oslo.messaging-9.8.0/playbooks/oslo.messaging-src-grenade-dsvm-multinode/run.yaml`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/releasenotes/source/conf.py` & `oslo.messaging-9.8.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `oslo.messaging-9.8.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/releasenotes/notes/removal-deprecated-options-6d4c5db90525c52d.yaml` & `oslo.messaging-9.8.0/releasenotes/notes/removal-deprecated-options-6d4c5db90525c52d.yaml`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/releasenotes/notes/rabbit-no-wait-for-ack-9e5de3e1320d7660.yaml` & `oslo.messaging-9.8.0/releasenotes/notes/rabbit-no-wait-for-ack-9e5de3e1320d7660.yaml`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/releasenotes/notes/bump-amqp-version-due-to-tls-issue-e877b152eb101c15.yaml` & `oslo.messaging-9.8.0/releasenotes/notes/bump-amqp-version-due-to-tls-issue-e877b152eb101c15.yaml`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/test-requirements.txt` & `oslo.messaging-9.8.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/requirements.txt` & `oslo.messaging-9.8.0/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 
 # for the routing notifier
 PyYAML>=3.12 # MIT
 
 # rabbit driver is the default
 # we set the amqp version to ensure heartbeat works
 amqp>=2.4.1 # BSD
-kombu!=4.0.2,>=4.0.0 # BSD
+kombu!=4.0.2,>=4.6.1 # BSD
 
 # middleware
 oslo.middleware>=3.31.0 # Apache-2.0
```

### Comparing `oslo.messaging-9.7.2/oslo.messaging.egg-info/entry_points.txt` & `oslo.messaging-9.8.0/oslo.messaging.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo.messaging.egg-info/PKG-INFO` & `oslo.messaging-9.8.0/oslo.messaging.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslo.messaging
-Version: 9.7.2
+Version: 9.8.0
 Summary: Oslo Messaging API
 Home-page: https://docs.openstack.org/oslo.messaging/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -43,10 +43,11 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: kafka
-Provides-Extra: test
 Provides-Extra: amqp1
+Provides-Extra: test
```

### Comparing `oslo.messaging-9.7.2/oslo.messaging.egg-info/SOURCES.txt` & `oslo.messaging-9.8.0/oslo.messaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/oslo.messaging.egg-info/requires.txt` & `oslo.messaging-9.8.0/oslo.messaging.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 stevedore>=1.20.0
 debtcollector>=1.2.0
 six>=1.10.0
 cachetools>=2.0.0
 WebOb>=1.7.1
 PyYAML>=3.12
 amqp>=2.4.1
-kombu!=4.0.2,>=4.0.0
+kombu!=4.0.2,>=4.6.1
 oslo.middleware>=3.31.0
 
 [:(python_version<'3.3')]
 monotonic>=0.6
 
 [amqp1]
 pyngus>=2.2.0
```

### Comparing `oslo.messaging-9.7.2/doc/source/user/FAQ.rst` & `oslo.messaging-9.8.0/doc/source/user/FAQ.rst`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/doc/source/conf.py` & `oslo.messaging-9.8.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/doc/source/contributor/driver-dev-guide.rst` & `oslo.messaging-9.8.0/doc/source/contributor/driver-dev-guide.rst`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/doc/source/contributor/supported-messaging-drivers.rst` & `oslo.messaging-9.8.0/doc/source/contributor/supported-messaging-drivers.rst`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/doc/source/admin/kafka.rst` & `oslo.messaging-9.8.0/doc/source/admin/kafka.rst`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 
 Set the Kafka and Scala version and location variables if needed for
 the configuration
 
 ::
 
    KAFKA_VERSION=2.0.0
-   KAFKA_BASEURL=http://www.apache.org/dist/kafka
+   KAFKA_BASEURL=http://archive.apache.org/dist/kafka
    SCALA_VERSION=2.12
    SCALA_BASEURL=http://www.scala-lang.org/riles/archive
 
 The **RPC_** and **NOTIFY_** variables will define the message bus
 configuration that will be used. The hybrid configurations will allow
 for the *rabbit* and *amqp* drivers to be used for the RPC transports
 while the *kafka* driver will be used for the Notify transport. The
```

### Comparing `oslo.messaging-9.7.2/doc/source/admin/AMQP1.0.rst` & `oslo.messaging-9.8.0/doc/source/admin/AMQP1.0.rst`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/doc/source/reference/executors.rst` & `oslo.messaging-9.8.0/doc/source/reference/executors.rst`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/doc/source/reference/transport.rst` & `oslo.messaging-9.8.0/doc/source/reference/transport.rst`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/doc/source/reference/target.rst` & `oslo.messaging-9.8.0/doc/source/reference/target.rst`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/doc/source/reference/exceptions.rst` & `oslo.messaging-9.8.0/doc/source/reference/exceptions.rst`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/doc/requirements.txt` & `oslo.messaging-9.8.0/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `oslo.messaging-9.7.2/AUTHORS` & `oslo.messaging-9.8.0/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 Chet Burgess <cfb@metacloud.com>
 Chris Dent <chdent@redhat.com>
 Christian Berendt <berendt@b1-systems.de>
 Christian Strack <strack@mathematik.uni-marburg.de>
 Clark Boylan <clark.boylan@gmail.com>
 Claudiu Belu <cbelu@cloudbasesolutions.com>
 Clint Byrum <clint@fewbar.com>
+Corey Bryant <corey.bryant@canonical.com>
 Corey Wright <corey.wright@rackspace.com>
 Cyril Roelandt <cyril@redhat.com>
 Daisuke Fujita <fuzita.daisuke@jp.fujitsu.com>
 Dan Prince <dprince@redhat.com>
 Dan Smith <dansmith@redhat.com>
 Daniel Alvarez <dalvarez@redhat.com>
 Davanum Srinivas (dims) <davanum@gmail.com>
```

### Comparing `oslo.messaging-9.7.2/tox.ini` & `oslo.messaging-9.8.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 minversion = 2.0
-envlist = py37,py27,pep8
+envlist = py27,py37,pep8
 
 [testenv]
 setenv =
     VIRTUAL_ENV={envdir}
 passenv = OS_*
           ZUUL_CACHE_DIR
           REQUIREMENTS_PIP_LOCATION
```

