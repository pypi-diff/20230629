# Comparing `tmp/line-bot-sdk-2.4.2.tar.gz` & `tmp/line-bot-sdk-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "line-bot-sdk-2.4.2.tar", last modified: Mon Mar 13 02:21:26 2023, max compression
+gzip compressed data, was "line-bot-sdk-3.0.0.tar", last modified: Thu Jun 29 06:34:01 2023, max compression
```

## Comparing `line-bot-sdk-2.4.2.tar` & `line-bot-sdk-3.0.0.tar`

### file list

```diff
@@ -1,123 +1,32 @@
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.970447 line-bot-sdk-2.4.2/
--rw-r--r--   0 yutakasai   (503) staff       (20)    11347 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/LICENSE
--rw-r--r--   0 yutakasai   (503) staff       (20)      244 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/MANIFEST.in
--rw-r--r--   0 yutakasai   (503) staff       (20)    46240 2023-03-13 02:21:26.970625 line-bot-sdk-2.4.2/PKG-INFO
--rw-r--r--   0 yutakasai   (503) staff       (20)    45423 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/README.rst
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.934257 line-bot-sdk-2.4.2/docs/
--rw-r--r--   0 yutakasai   (503) staff       (20)     7667 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/docs/Makefile
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.935452 line-bot-sdk-2.4.2/docs/source/
--rw-r--r--   0 yutakasai   (503) staff       (20)    10166 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/docs/source/conf.py
--rw-r--r--   0 yutakasai   (503) staff       (20)      430 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/docs/source/index.rst
--rw-r--r--   0 yutakasai   (503) staff       (20)     1959 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/docs/source/linebot.models.rst
--rw-r--r--   0 yutakasai   (503) staff       (20)      457 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/docs/source/linebot.rst
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.937310 line-bot-sdk-2.4.2/line_bot_sdk.egg-info/
--rw-r--r--   0 yutakasai   (503) staff       (20)    46240 2023-03-13 02:21:26.000000 line-bot-sdk-2.4.2/line_bot_sdk.egg-info/PKG-INFO
--rw-r--r--   0 yutakasai   (503) staff       (20)     3287 2023-03-13 02:21:26.000000 line-bot-sdk-2.4.2/line_bot_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 yutakasai   (503) staff       (20)        1 2023-03-13 02:21:26.000000 line-bot-sdk-2.4.2/line_bot_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 yutakasai   (503) staff       (20)       39 2023-03-13 02:21:26.000000 line-bot-sdk-2.4.2/line_bot_sdk.egg-info/requires.txt
--rw-r--r--   0 yutakasai   (503) staff       (20)        8 2023-03-13 02:21:26.000000 line-bot-sdk-2.4.2/line_bot_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.942800 line-bot-sdk-2.4.2/linebot/
--rw-r--r--   0 yutakasai   (503) staff       (20)      781 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/__about__.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1056 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/__init__.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     5946 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/aiohttp_async_http_client.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    86776 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/api.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    88701 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/async_api.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     5099 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/async_http_client.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3198 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/exceptions.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    10498 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/http_client.py
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.950567 line-bot-sdk-2.4.2/linebot/models/
--rw-r--r--   0 yutakasai   (503) staff       (20)     4846 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/__init__.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     9405 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/actions.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1939 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/background.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3795 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/base.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1107 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/delivery_context.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1183 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/emojis.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1845 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/error.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    19053 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/events.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     4941 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/filter.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    26498 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/flex_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     7011 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/imagemap.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    10480 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/insight.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1132 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/limit.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1180 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/mention.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1351 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/mentionee.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     9111 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/messages.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2403 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/operator.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2083 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/recipient.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    38321 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/responses.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     5012 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/rich_menu.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     9375 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/send_messages.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3831 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/sources.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     9133 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/template.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     4718 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/things.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1065 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/unsend.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1210 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/video_play_complete.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1715 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/utils.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     9610 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/webhook.py
--rw-r--r--   0 yutakasai   (503) staff       (20)      111 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/requirements-dev.txt
--rw-r--r--   0 yutakasai   (503) staff       (20)       55 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/requirements-test.txt
--rw-r--r--   0 yutakasai   (503) staff       (20)       41 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/requirements.txt
--rw-r--r--   0 yutakasai   (503) staff       (20)       92 2023-03-13 02:21:26.971117 line-bot-sdk-2.4.2/setup.cfg
--rw-r--r--   0 yutakasai   (503) staff       (20)     7321 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/setup.py
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.952125 line-bot-sdk-2.4.2/tests/
--rw-r--r--   0 yutakasai   (503) staff       (20)      580 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/__init__.py
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.964887 line-bot-sdk-2.4.2/tests/api/
--rw-r--r--   0 yutakasai   (503) staff       (20)      580 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/__init__.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     6321 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_channel_access_token_v2_1.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     4433 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_error_handle.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2073 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_bot_info.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1132 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_content.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     4401 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_custom_aggregation_units.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3393 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_delivery.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2374 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_group.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    12659 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_insight.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     6651 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_member_ids.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2750 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_member_profile.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2333 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_message_quota.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1948 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_profile.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1470 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_room.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1649 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_webhook_endpoint.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2541 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_issue_channel_token.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1548 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_issue_link_token.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1836 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_leave.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    14943 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_narrowcast_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1565 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_revoke_channel_token.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    17746 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_rich_menu.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     6049 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_rich_menu_alias.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3497 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_audio_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3558 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_image_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     5876 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_imagemap_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3617 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_location_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3411 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_sticker_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    22270 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_template_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     8052 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_text_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     6111 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_text_message_with_quick_reply.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2476 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_text_message_with_sender.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     5440 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_text_message_with_statistics_per_aggregation_unit.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3631 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_video_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1456 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_set_webhook_endpoint.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1892 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_test_webhook_endpoint.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     5204 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_validate_message_objects.py
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.966024 line-bot-sdk-2.4.2/tests/async_api/
--rw-r--r--   0 yutakasai   (503) staff       (20)     1688 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/async_api/test_async_error_handle.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1357 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/async_api/test_get_message_content.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1518 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/async_api/test_get_profile.py
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.969396 line-bot-sdk-2.4.2/tests/models/
--rw-r--r--   0 yutakasai   (503) staff       (20)      580 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/__init__.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2551 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/serialize_test_case.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3203 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_actions.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1223 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_background.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2959 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_base.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2213 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_filter.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     9117 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_flex_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     4112 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_imagemap.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     4084 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_send_messages.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     6757 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_template.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2721 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_text_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3168 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/test_aiohttp_async_http_client.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2662 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/test_exceptions.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1820 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/test_utils.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    39339 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/test_webhook.py
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.969748 line-bot-sdk-2.4.2/tests/text/
--rw-r--r--   0 yutakasai   (503) staff       (20)    15137 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/text/webhook.json
--rw-r--r--   0 yutakasai   (503) staff       (20)      564 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tox.ini
+drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-06-29 06:34:01.115376 line-bot-sdk-3.0.0/
+-rw-r--r--   0 yutakasai   (503) staff       (20)    11347 2023-06-29 06:02:15.000000 line-bot-sdk-3.0.0/LICENSE
+-rw-r--r--   0 yutakasai   (503) staff       (20)      244 2023-06-29 06:02:15.000000 line-bot-sdk-3.0.0/MANIFEST.in
+-rw-r--r--   0 yutakasai   (503) staff       (20)     9754 2023-06-29 06:34:01.115484 line-bot-sdk-3.0.0/PKG-INFO
+-rw-r--r--   0 yutakasai   (503) staff       (20)     8906 2023-06-29 06:33:37.000000 line-bot-sdk-3.0.0/README.rst
+drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-06-29 06:34:01.110417 line-bot-sdk-3.0.0/line_bot_sdk.egg-info/
+-rw-r--r--   0 yutakasai   (503) staff       (20)     9754 2023-06-29 06:34:01.000000 line-bot-sdk-3.0.0/line_bot_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 yutakasai   (503) staff       (20)      531 2023-06-29 06:34:01.000000 line-bot-sdk-3.0.0/line_bot_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 yutakasai   (503) staff       (20)        1 2023-06-29 06:34:01.000000 line-bot-sdk-3.0.0/line_bot_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 yutakasai   (503) staff       (20)       96 2023-06-29 06:34:01.000000 line-bot-sdk-3.0.0/line_bot_sdk.egg-info/requires.txt
+-rw-r--r--   0 yutakasai   (503) staff       (20)        8 2023-06-29 06:34:01.000000 line-bot-sdk-3.0.0/line_bot_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-06-29 06:34:01.112384 line-bot-sdk-3.0.0/linebot/
+-rw-r--r--   0 yutakasai   (503) staff       (20)      781 2023-06-29 06:02:29.000000 line-bot-sdk-3.0.0/linebot/__about__.py
+-rw-r--r--   0 yutakasai   (503) staff       (20)      774 2023-06-29 06:02:29.000000 line-bot-sdk-3.0.0/linebot/__init__.py
+-rw-r--r--   0 yutakasai   (503) staff       (20)     1469 2023-06-29 06:02:29.000000 line-bot-sdk-3.0.0/linebot/exceptions.py
+drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-06-29 06:34:01.113143 line-bot-sdk-3.0.0/linebot/models/
+-rw-r--r--   0 yutakasai   (503) staff       (20)      662 2023-06-29 06:02:29.000000 line-bot-sdk-3.0.0/linebot/models/__init__.py
+-rw-r--r--   0 yutakasai   (503) staff       (20)     1099 2023-06-29 06:02:29.000000 line-bot-sdk-3.0.0/linebot/models/events.py
+-rw-r--r--   0 yutakasai   (503) staff       (20)     1715 2023-06-29 06:02:15.000000 line-bot-sdk-3.0.0/linebot/utils.py
+-rw-r--r--   0 yutakasai   (503) staff       (20)     8003 2023-06-29 06:02:29.000000 line-bot-sdk-3.0.0/linebot/webhook.py
+-rw-r--r--   0 yutakasai   (503) staff       (20)      111 2023-06-29 06:02:15.000000 line-bot-sdk-3.0.0/requirements-dev.txt
+-rw-r--r--   0 yutakasai   (503) staff       (20)       55 2023-06-29 06:02:15.000000 line-bot-sdk-3.0.0/requirements-test.txt
+-rw-r--r--   0 yutakasai   (503) staff       (20)      106 2023-06-29 06:02:29.000000 line-bot-sdk-3.0.0/requirements.txt
+-rw-r--r--   0 yutakasai   (503) staff       (20)       92 2023-06-29 06:34:01.115846 line-bot-sdk-3.0.0/setup.cfg
+-rw-r--r--   0 yutakasai   (503) staff       (20)     2730 2023-06-29 06:02:29.000000 line-bot-sdk-3.0.0/setup.py
+drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-06-29 06:34:01.114332 line-bot-sdk-3.0.0/tests/
+-rw-r--r--   0 yutakasai   (503) staff       (20)      580 2023-06-29 06:02:15.000000 line-bot-sdk-3.0.0/tests/__init__.py
+-rw-r--r--   0 yutakasai   (503) staff       (20)     1820 2023-06-29 06:02:15.000000 line-bot-sdk-3.0.0/tests/test_utils.py
+-rw-r--r--   0 yutakasai   (503) staff       (20)    39951 2023-06-29 06:02:29.000000 line-bot-sdk-3.0.0/tests/test_webhook.py
+drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-06-29 06:34:01.115157 line-bot-sdk-3.0.0/tests/text/
+-rw-r--r--   0 yutakasai   (503) staff       (20)    15209 2023-06-29 06:02:29.000000 line-bot-sdk-3.0.0/tests/text/webhook.json
+-rw-r--r--   0 yutakasai   (503) staff       (20)      614 2023-06-29 06:02:29.000000 line-bot-sdk-3.0.0/tox.ini
```

### Comparing `line-bot-sdk-2.4.2/LICENSE` & `line-bot-sdk-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/__about__.py` & `line-bot-sdk-3.0.0/linebot/__about__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations
 #  under the License.
 
 """Meta data of line-bot-sdk."""
 
 
-__version__ = '2.4.2'
+__version__ = '3.0.0'
 __author__ = 'LINE Corporation'
 __copyright__ = 'Copyright 2016, LINE Corporation'
 __license__ = 'Apache 2.0'
 
 __all__ = (
     '__version__'
 )
```

### Comparing `line-bot-sdk-2.4.2/linebot/__init__.py` & `line-bot-sdk-3.0.0/linebot/models/events.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,34 +8,28 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations
 #  under the License.
 
-"""linebot package."""
+"""linebot.models.events module."""
 
+from linebot.webhooks.models.event import Event
+from linebot.utils import to_snake_case
 
-from .__about__ import (  # noqa
-    __version__
-)
-from .api import (  # noqa
-    LineBotApi,
-)
-from .async_api import (  # noqa
-    AsyncLineBotApi,
-)
-from .http_client import (  # noqa
-    HttpClient,
-    RequestsHttpClient,
-    HttpResponse,
-)
-from .async_http_client import (  # noqa
-    AsyncHttpClient,
-    AsyncHttpResponse,
-)
-from .webhook import (  # noqa
-    SignatureValidator,
-    WebhookParser,
-    WebhookHandler,
-    WebhookPayload,
-)
+class UnknownEvent(Event):
+    """Unknown event.
+
+    We welcome your contribution to line-bot-sdk-python!
+    """
+
+    @classmethod
+    def new_from_json_dict(cls, data):
+        """Create a new instance from a dict.
+
+        :param data: JSON dict
+        """
+        new_data = {to_snake_case(key): value
+                    for key, value in data.items()}
+
+        return cls(**new_data)
```

### Comparing `line-bot-sdk-2.4.2/linebot/models/background.py` & `line-bot-sdk-3.0.0/linebot/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,52 +8,47 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations
 #  under the License.
 
-"""linebot.models.emojis module."""
+"""linebot.exceptions module."""
 
 
 from abc import ABCMeta
 
 from future.utils import with_metaclass
 
-from .base import Base
 
+class BaseError(with_metaclass(ABCMeta, Exception)):
+    """Base Exception class."""
 
-class Background(with_metaclass(ABCMeta, Base)):
-    """Background."""
-
-    def __init__(self, **kwargs):
+    def __init__(self, message='-'):
         """__init__ method.
 
-        :param kwargs:
+        :param str message: Human readable message
         """
-        super(Background, self).__init__(**kwargs)
+        self.message = message
+
+    def __repr__(self):
+        """repr."""
+        return str(self)
 
-        self.type = None
+    def __str__(self):
+        """str.
+
+        :rtype: str
+        """
+        return '<{0} [{1}]>'.format(
+            self.__class__.__name__, self.message)
 
 
-class LinearGradientBackground(Background):
-    """LinearGradientBackground."""
+class InvalidSignatureError(BaseError):
+    """When Webhook signature does NOT match, this error will be raised."""
 
-    def __init__(self, angle, start_color, end_color,
-                 center_color=None, center_position=None, **kwargs):
+    def __init__(self, message='-'):
         """__init__ method.
 
-        :param str type: The type of background used
-        :param str angle: The angle at which a linear gradient moves
-        :param str start_color: The color at the gradient's starting point
-        :param str end_color: The color at the gradient's ending point
-        :param str center_color: The color in the middle of the gradient
-        :param str center_position: The position of the intermediate color stop
-        :param kwargs:
+        :param str message: Human readable message
         """
-        super(LinearGradientBackground, self).__init__(**kwargs)
-        self.type = 'linearGradient'
-        self.angle = angle
-        self.start_color = start_color
-        self.end_color = end_color
-        self.center_color = center_color
-        self.center_position = center_position
+        super(InvalidSignatureError, self).__init__(message)
```

### Comparing `line-bot-sdk-2.4.2/linebot/utils.py` & `line-bot-sdk-3.0.0/linebot/utils.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/webhook.py` & `line-bot-sdk-3.0.0/linebot/webhook.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,32 +16,22 @@
 
 
 import base64
 import hashlib
 import hmac
 import inspect
 import json
+import pprint
 
 from .exceptions import InvalidSignatureError
-from .models.events import (
+from linebot.webhooks import (
+    Event,
     MessageEvent,
-    FollowEvent,
-    UnfollowEvent,
-    JoinEvent,
-    LeaveEvent,
-    PostbackEvent,
-    BeaconEvent,
-    AccountLinkEvent,
-    MemberJoinedEvent,
-    MemberLeftEvent,
-    ThingsEvent,
-    UnsendEvent,
-    VideoPlayCompleteEvent,
-    UnknownEvent,
 )
+from .models.events import UnknownEvent ## Special
 from .utils import LOGGER, PY3, safe_compare_digest
 
 if hasattr(hmac, "compare_digest"):
     def compare_digest(val1, val2):
         """compare_digest function.
 
         If hmac module has compare_digest function, use it.
@@ -143,43 +133,18 @@
         if not self.signature_validator.validate(body, signature):
             raise InvalidSignatureError(
                 'Invalid signature. signature=' + signature)
 
         body_json = json.loads(body)
         events = []
         for event in body_json['events']:
-            event_type = event['type']
-            if event_type == 'message':
-                events.append(MessageEvent.new_from_json_dict(event))
-            elif event_type == 'follow':
-                events.append(FollowEvent.new_from_json_dict(event))
-            elif event_type == 'unfollow':
-                events.append(UnfollowEvent.new_from_json_dict(event))
-            elif event_type == 'join':
-                events.append(JoinEvent.new_from_json_dict(event))
-            elif event_type == 'leave':
-                events.append(LeaveEvent.new_from_json_dict(event))
-            elif event_type == 'postback':
-                events.append(PostbackEvent.new_from_json_dict(event))
-            elif event_type == 'beacon':
-                events.append(BeaconEvent.new_from_json_dict(event))
-            elif event_type == 'accountLink':
-                events.append(AccountLinkEvent.new_from_json_dict(event))
-            elif event_type == 'memberJoined':
-                events.append(MemberJoinedEvent.new_from_json_dict(event))
-            elif event_type == 'memberLeft':
-                events.append(MemberLeftEvent.new_from_json_dict(event))
-            elif event_type == 'things':
-                events.append(ThingsEvent.new_from_json_dict(event))
-            elif event_type == 'unsend':
-                events.append(UnsendEvent.new_from_json_dict(event))
-            elif event_type == 'videoPlayComplete':
-                events.append(VideoPlayCompleteEvent.new_from_json_dict(event))
-            else:
-                LOGGER.info('Unknown event type. type=' + event_type)
+            try:
+                events.append(Event.from_dict(event))
+            except ValueError:
+                LOGGER.info('Unknown event type. type=' + event['type'])
                 events.append(UnknownEvent.new_from_json_dict(event))
 
         if as_payload:
             return WebhookPayload(events=events, destination=body_json.get('destination'))
         else:
             return events
```

### Comparing `line-bot-sdk-2.4.2/tests/__init__.py` & `line-bot-sdk-3.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/test_utils.py` & `line-bot-sdk-3.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/test_webhook.py` & `line-bot-sdk-3.0.0/tests/test_webhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,29 @@
 import unittest
 from builtins import open
 import inspect
 
 from linebot import (
     SignatureValidator, WebhookParser, WebhookHandler
 )
-from linebot.models import (
+from linebot.webhooks.models import (
     MessageEvent, FollowEvent, UnfollowEvent, JoinEvent,
     LeaveEvent, PostbackEvent, BeaconEvent, AccountLinkEvent,
     MemberJoinedEvent, MemberLeftEvent, ThingsEvent,
+    VideoPlayCompleteEvent, VideoPlayComplete, UnsendEvent, UnsendDetail,
+    TextMessageContent, ImageMessageContent, VideoMessageContent, AudioMessageContent,
+    LocationMessageContent, StickerMessageContent, FileMessageContent,
+    UserSource, RoomSource, GroupSource,
+    LinkThingsContent, UnlinkThingsContent, ActionResult,
+    ScenarioResultThingsContent,
+    DeliveryContext
+)
+from linebot.models import (
     UnknownEvent,
-    TextMessage, ImageMessage, VideoMessage, AudioMessage,
-    LocationMessage, StickerMessage, FileMessage,
-    SourceUser, SourceRoom, SourceGroup,
-    DeviceLink, DeviceUnlink, ScenarioResult, ActionResult)
-from linebot.models.delivery_context import DeliveryContext
-from linebot.models.events import UnsendEvent, VideoPlayCompleteEvent
-from linebot.models.unsend import Unsend
-from linebot.models.video_play_complete import VideoPlayComplete
+)
 from linebot.utils import PY3
 
 
 class TestSignatureValidator(unittest.TestCase):
     def test_validate(self):
         signature_validator = SignatureValidator('channel_secret')
 
@@ -68,430 +70,428 @@
             body = fp.read()
 
         events = self.parser.parse(body, 'channel_secret')
 
         # events count
         self.assertEqual(len(events), 30)
 
-        # MessageEvent, SourceUser, TextMessage
+        # MessageEvent, UserSource, TextMessageContent
         self.assertIsInstance(events[0], MessageEvent)
         self.assertEqual(events[0].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[0].type, 'message')
         self.assertEqual(events[0].mode, 'active')
         self.assertEqual(events[0].timestamp, 1462629479859)
-        self.assertIsInstance(events[0].source, SourceUser)
+        self.assertIsInstance(events[0].source, UserSource)
         self.assertEqual(events[0].source.type, 'user')
         self.assertEqual(events[0].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[0].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[0].delivery_context, DeliveryContext)
         self.assertFalse(events[0].delivery_context.is_redelivery)
-        self.assertIsInstance(events[0].message, TextMessage)
+        self.assertIsInstance(events[0].message, TextMessageContent)
         self.assertEqual(events[0].message.id, '325708')
         self.assertEqual(events[0].message.type, 'text')
         self.assertEqual(events[0].message.text, 'Hello, world')
 
-        # MessageEvent, SourceRoom, ImageMessage
+        # MessageEvent, RoomSource, ImageMessageContent
         self.assertIsInstance(events[1], MessageEvent)
         self.assertEqual(events[1].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[1].type, 'message')
         self.assertEqual(events[1].mode, 'active')
         self.assertEqual(events[1].timestamp, 1462629479859)
-        self.assertIsInstance(events[1].source, SourceRoom)
+        self.assertIsInstance(events[1].source, RoomSource)
         self.assertEqual(events[1].source.type, 'room')
         self.assertEqual(events[1].source.room_id, 'Ra8dbf4673c4c812cd491258042226c99')
         self.assertEqual(events[1].source.user_id, None)
         self.assertEqual(events[1].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[1].delivery_context, DeliveryContext)
         self.assertFalse(events[1].delivery_context.is_redelivery)
-        self.assertIsInstance(events[1].message, ImageMessage)
+        self.assertIsInstance(events[1].message, ImageMessageContent)
         self.assertEqual(events[1].message.id, '325708')
         self.assertEqual(events[1].message.type, 'image')
         self.assertEqual(events[1].message.content_provider.type, 'external')
         self.assertEqual(events[1].message.content_provider.original_content_url,
                          "https://example.com")
         self.assertEqual(events[1].message.content_provider.preview_image_url,
                          "https://example.com")
 
-        # MessageEvent, SourceUser, VideoMessage
+        # MessageEvent, UserSource, VideoMessageContent
         self.assertIsInstance(events[2], MessageEvent)
         self.assertEqual(events[2].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[2].type, 'message')
         self.assertEqual(events[2].mode, 'active')
         self.assertEqual(events[2].timestamp, 1462629479859)
-        self.assertIsInstance(events[2].source, SourceUser)
+        self.assertIsInstance(events[2].source, UserSource)
         self.assertEqual(events[2].source.type, 'user')
         self.assertEqual(events[2].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[2].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[2].delivery_context, DeliveryContext)
         self.assertFalse(events[2].delivery_context.is_redelivery)
-        self.assertIsInstance(events[2].message, VideoMessage)
+        self.assertIsInstance(events[2].message, VideoMessageContent)
         self.assertEqual(events[2].message.id, '325708')
         self.assertEqual(events[2].message.type, 'video')
         self.assertEqual(events[2].message.duration, 60000)
         self.assertEqual(events[2].message.content_provider.type, 'external')
         self.assertEqual(events[2].message.content_provider.original_content_url,
                          "https://example.com")
         self.assertEqual(events[2].message.content_provider.preview_image_url,
                          "https://example.com")
 
-        # MessageEvent, SourceUser, AudioMessage
+        # MessageEvent, UserSource, AudioMessageContent
         self.assertIsInstance(events[3], MessageEvent)
         self.assertEqual(events[3].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[3].type, 'message')
         self.assertEqual(events[3].mode, 'active')
         self.assertEqual(events[3].timestamp, 1462629479859)
-        self.assertIsInstance(events[3].source, SourceUser)
+        self.assertIsInstance(events[3].source, UserSource)
         self.assertEqual(events[3].source.type, 'user')
         self.assertEqual(events[3].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[3].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[3].delivery_context, DeliveryContext)
         self.assertFalse(events[3].delivery_context.is_redelivery)
-        self.assertIsInstance(events[3].message, AudioMessage)
+        self.assertIsInstance(events[3].message, AudioMessageContent)
         self.assertEqual(events[3].message.id, '325708')
         self.assertEqual(events[3].message.type, 'audio')
         self.assertEqual(events[3].message.duration, 60000)
         self.assertEqual(events[3].message.content_provider.type, 'external')
         self.assertEqual(events[3].message.content_provider.original_content_url,
                          "https://example.com")
 
-        # MessageEvent, SourceUser, LocationMessage
+        # MessageEvent, UserSource, LocationMessageContent
         self.assertIsInstance(events[4], MessageEvent)
         self.assertEqual(events[4].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[4].type, 'message')
         self.assertEqual(events[4].mode, 'active')
         self.assertEqual(events[4].timestamp, 1462629479859)
-        self.assertIsInstance(events[4].source, SourceUser)
+        self.assertIsInstance(events[4].source, UserSource)
         self.assertEqual(events[4].source.type, 'user')
         self.assertEqual(events[4].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[4].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[4].delivery_context, DeliveryContext)
         self.assertFalse(events[4].delivery_context.is_redelivery)
-        self.assertIsInstance(events[4].message, LocationMessage)
+        self.assertIsInstance(events[4].message, LocationMessageContent)
         self.assertEqual(events[4].message.id, '325708')
         self.assertEqual(events[4].message.type, 'location')
         self.assertEqual(events[4].message.title, 'my location')
         self.assertEqual(events[4].message.address, 'Tokyo')
         self.assertEqual(events[4].message.latitude, 35.65910807942215)
         self.assertEqual(events[4].message.longitude, 139.70372892916203)
 
-        # MessageEvent, SourceUser, StickerMessage
+        # MessageEvent, UserSource, StickerMessageContent
         self.assertIsInstance(events[5], MessageEvent)
         self.assertEqual(events[5].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[5].type, 'message')
         self.assertEqual(events[5].mode, 'active')
         self.assertEqual(events[5].timestamp, 1462629479859)
-        self.assertIsInstance(events[5].source, SourceUser)
+        self.assertIsInstance(events[5].source, UserSource)
         self.assertEqual(events[5].source.type, 'user')
         self.assertEqual(events[5].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[5].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[5].delivery_context, DeliveryContext)
         self.assertFalse(events[5].delivery_context.is_redelivery)
-        self.assertIsInstance(events[5].message, StickerMessage)
+        self.assertIsInstance(events[5].message, StickerMessageContent)
         self.assertEqual(events[5].message.id, '325708')
         self.assertEqual(events[5].message.type, 'sticker')
         self.assertEqual(events[5].message.package_id, '1')
         self.assertEqual(events[5].message.sticker_id, '1')
         self.assertEqual(events[5].message.sticker_resource_type, 'STATIC')
         self.assertEqual(events[5].message.keywords[0], 'Love You')
         self.assertEqual(events[5].message.keywords[1], 'Love')
         self.assertEqual(events[5].message.text, 'Just sticker')
 
-        # FollowEvent, SourceUser
+        # FollowEvent, User
         self.assertIsInstance(events[6], FollowEvent)
         self.assertEqual(events[6].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[6].type, 'follow')
         self.assertEqual(events[6].mode, 'active')
         self.assertEqual(events[6].timestamp, 1462629479859)
-        self.assertIsInstance(events[6].source, SourceUser)
+        self.assertIsInstance(events[6].source, UserSource)
         self.assertEqual(events[6].source.type, 'user')
         self.assertEqual(events[6].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[6].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[6].delivery_context, DeliveryContext)
         self.assertFalse(events[6].delivery_context.is_redelivery)
 
-        # UnfollowEvent, SourceUser
+        # UnfollowEvent, User
         self.assertIsInstance(events[7], UnfollowEvent)
         self.assertEqual(events[7].type, 'unfollow')
         self.assertEqual(events[7].mode, 'active')
         self.assertEqual(events[7].timestamp, 1462629479859)
-        self.assertIsInstance(events[7].source, SourceUser)
+        self.assertIsInstance(events[7].source, UserSource)
         self.assertEqual(events[7].source.type, 'user')
         self.assertEqual(events[7].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[7].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[7].delivery_context, DeliveryContext)
         self.assertFalse(events[7].delivery_context.is_redelivery)
 
-        # JoinEvent, SourceGroup
+        # JoinEvent, GroupSource
         self.assertIsInstance(events[8], JoinEvent)
         self.assertEqual(events[8].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[8].type, 'join')
         self.assertEqual(events[8].mode, 'active')
         self.assertEqual(events[8].timestamp, 1462629479859)
-        self.assertIsInstance(events[8].source, SourceGroup)
+        self.assertIsInstance(events[8].source, GroupSource)
         self.assertEqual(events[8].source.type, 'group')
         self.assertEqual(events[8].source.group_id, 'Ca56f94637cc4347f90a25382909b24b9')
         self.assertEqual(events[8].source.user_id, None)
         self.assertEqual(events[8].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[8].delivery_context, DeliveryContext)
         self.assertFalse(events[8].delivery_context.is_redelivery)
 
-        # LeaveEvent, SourceGroup
+        # LeaveEvent, GroupSource
         self.assertIsInstance(events[9], LeaveEvent)
         self.assertEqual(events[9].type, 'leave')
         self.assertEqual(events[9].mode, 'active')
         self.assertEqual(events[9].timestamp, 1462629479859)
-        self.assertIsInstance(events[9].source, SourceGroup)
+        self.assertIsInstance(events[9].source, GroupSource)
         self.assertEqual(events[9].source.type, 'group')
         self.assertEqual(events[9].source.group_id, 'Ca56f94637cc4347f90a25382909b24b9')
         self.assertEqual(events[9].source.user_id, None)
         self.assertEqual(events[9].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[9].delivery_context, DeliveryContext)
         self.assertFalse(events[9].delivery_context.is_redelivery)
 
-        # PostbackEvent, SourceUser
+        # PostbackEvent, UserSource
         self.assertIsInstance(events[10], PostbackEvent)
         self.assertEqual(events[10].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[10].type, 'postback')
         self.assertEqual(events[10].mode, 'active')
         self.assertEqual(events[10].timestamp, 1462629479859)
-        self.assertIsInstance(events[10].source, SourceUser)
+        self.assertIsInstance(events[10].source, UserSource)
         self.assertEqual(events[10].source.type, 'user')
         self.assertEqual(events[10].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[10].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[10].delivery_context, DeliveryContext)
         self.assertFalse(events[10].delivery_context.is_redelivery)
         self.assertEqual(events[10].postback.data, 'action=buyItem&itemId=123123&color=red')
-        self.assertEqual(events[10].postback.params, None)
+        self.assertEqual(events[10].postback.params, {'datetime': '2017-12-25T01:00'})
 
-        # BeaconEvent, SourceUser
+        # BeaconEvent, UserSource
         self.assertIsInstance(events[11], BeaconEvent)
         self.assertEqual(events[11].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[11].type, 'beacon')
         self.assertEqual(events[11].mode, 'active')
         self.assertEqual(events[11].timestamp, 1462629479859)
-        self.assertIsInstance(events[11].source, SourceUser)
+        self.assertIsInstance(events[11].source, UserSource)
         self.assertEqual(events[11].source.type, 'user')
         self.assertEqual(events[11].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[11].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[11].delivery_context, DeliveryContext)
         self.assertFalse(events[11].delivery_context.is_redelivery)
         self.assertEqual(events[11].beacon.hwid, 'd41d8cd98f')
         self.assertEqual(events[11].beacon.type, 'enter')
         self.assertEqual(events[11].beacon.dm, None)
-        self.assertEqual(events[11].beacon.device_message, None)
 
-        # BeaconEvent, SourceUser (with device message)
+        # BeaconEvent, UserSource (with device message)
         self.assertIsInstance(events[12], BeaconEvent)
         self.assertEqual(events[12].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[12].type, 'beacon')
         self.assertEqual(events[12].mode, 'active')
         self.assertEqual(events[12].timestamp, 1462629479859)
-        self.assertIsInstance(events[12].source, SourceUser)
+        self.assertIsInstance(events[12].source, UserSource)
         self.assertEqual(events[12].source.type, 'user')
         self.assertEqual(events[12].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[12].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[12].delivery_context, DeliveryContext)
         self.assertFalse(events[12].delivery_context.is_redelivery)
         self.assertEqual(events[12].beacon.hwid, 'd41d8cd98f')
         self.assertEqual(events[12].beacon.type, 'enter')
         self.assertEqual(events[12].beacon.dm, '1234567890abcdef')
-        self.assertEqual(events[12].beacon.device_message, bytearray(b'\x124Vx\x90\xab\xcd\xef'))
 
-        # AccountEvent, SourceUser
+        # AccountEvent, UserSource
         self.assertIsInstance(events[13], AccountLinkEvent)
         self.assertEqual(events[13].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[13].type, 'accountLink')
         self.assertEqual(events[13].mode, 'active')
         self.assertEqual(events[13].timestamp, 1462629479859)
-        self.assertIsInstance(events[13].source, SourceUser)
+        self.assertIsInstance(events[13].source, UserSource)
         self.assertEqual(events[13].source.type, 'user')
         self.assertEqual(events[13].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[13].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[13].delivery_context, DeliveryContext)
         self.assertFalse(events[13].delivery_context.is_redelivery)
         self.assertEqual(events[13].link.result, 'ok')
         self.assertEqual(events[13].link.nonce, 'Vb771wDYtXuammLszK6h9A')
 
-        # MessageEvent, SourceGroup with userId, TextMessage
+        # MessageEvent, GroupSource with userId, TextMessageContent
         self.assertIsInstance(events[14], MessageEvent)
         self.assertEqual(events[14].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[14].type, 'message')
         self.assertEqual(events[14].mode, 'active')
         self.assertEqual(events[14].timestamp, 1462629479859)
-        self.assertIsInstance(events[14].source, SourceGroup)
+        self.assertIsInstance(events[14].source, GroupSource)
         self.assertEqual(events[14].source.type, 'group')
         self.assertEqual(events[14].source.group_id, 'Ca56f94637cc4347f90a25382909b24b9')
         self.assertEqual(events[14].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[14].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[14].delivery_context, DeliveryContext)
         self.assertFalse(events[14].delivery_context.is_redelivery)
-        self.assertIsInstance(events[14].message, TextMessage)
+        self.assertIsInstance(events[14].message, TextMessageContent)
         self.assertEqual(events[14].message.id, '325708')
         self.assertEqual(events[14].message.type, 'text')
         self.assertEqual(events[14].message.text, 'Hello, world')
 
-        # MessageEvent, SourceRoom with userId, TextMessage
+        # MessageEvent, RoomSource with userId, TextMessageContent
         self.assertIsInstance(events[15], MessageEvent)
         self.assertEqual(events[15].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[15].type, 'message')
         self.assertEqual(events[15].mode, 'active')
         self.assertEqual(events[15].timestamp, 1462629479859)
-        self.assertIsInstance(events[15].source, SourceRoom)
+        self.assertIsInstance(events[15].source, RoomSource)
         self.assertEqual(events[15].source.type, 'room')
         self.assertEqual(events[15].source.room_id, 'Ra8dbf4673c4c812cd491258042226c99')
         self.assertEqual(events[15].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[15].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[15].delivery_context, DeliveryContext)
         self.assertFalse(events[15].delivery_context.is_redelivery)
-        self.assertIsInstance(events[15].message, TextMessage)
+        self.assertIsInstance(events[15].message, TextMessageContent)
         self.assertEqual(events[15].message.id, '325708')
         self.assertEqual(events[15].message.type, 'text')
         self.assertEqual(events[15].message.text, 'Hello, world')
 
-        # PostbackEvent, SourceUser, with date params
+        # PostbackEvent, UserSource, with date params
         self.assertIsInstance(events[16], PostbackEvent)
         self.assertEqual(events[16].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[16].type, 'postback')
         self.assertEqual(events[16].mode, 'active')
         self.assertEqual(events[16].timestamp, 1462629479859)
-        self.assertIsInstance(events[16].source, SourceUser)
+        self.assertIsInstance(events[16].source, UserSource)
         self.assertEqual(events[16].source.type, 'user')
         self.assertEqual(events[16].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[16].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[16].delivery_context, DeliveryContext)
         self.assertFalse(events[16].delivery_context.is_redelivery)
         self.assertEqual(events[16].postback.data, 'action=buyItem&itemId=123123&color=red')
         self.assertEqual(events[16].postback.params['date'], '2013-04-01')
 
-        # PostbackEvent, SourceUser, with date params
+        # PostbackEvent, UserSource, with date params
         self.assertIsInstance(events[17], PostbackEvent)
         self.assertEqual(events[17].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[17].type, 'postback')
         self.assertEqual(events[17].mode, 'active')
         self.assertEqual(events[17].timestamp, 1462629479859)
-        self.assertIsInstance(events[17].source, SourceUser)
+        self.assertIsInstance(events[17].source, UserSource)
         self.assertEqual(events[17].source.type, 'user')
         self.assertEqual(events[17].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[17].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[17].delivery_context, DeliveryContext)
         self.assertFalse(events[17].delivery_context.is_redelivery)
         self.assertEqual(events[17].postback.data, 'action=buyItem&itemId=123123&color=red')
         self.assertEqual(events[17].postback.params['time'], '10:00')
 
-        # PostbackEvent, SourceUser, with date params
+        # PostbackEvent, UserSource, with date params
         self.assertIsInstance(events[18], PostbackEvent)
         self.assertEqual(events[18].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[18].type, 'postback')
         self.assertEqual(events[18].mode, 'active')
         self.assertEqual(events[18].timestamp, 1462629479859)
-        self.assertIsInstance(events[18].source, SourceUser)
+        self.assertIsInstance(events[18].source, UserSource)
         self.assertEqual(events[18].source.type, 'user')
         self.assertEqual(events[18].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[18].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[18].delivery_context, DeliveryContext)
         self.assertFalse(events[18].delivery_context.is_redelivery)
         self.assertEqual(events[18].postback.data, 'action=buyItem&itemId=123123&color=red')
         self.assertEqual(events[18].postback.params['datetime'], '2013-04-01T10:00')
 
-        # ThingsEvent, SourceUser, link
+        # ThingsEvent, UserSource, link
         self.assertIsInstance(events[19], ThingsEvent)
         self.assertEqual(events[19].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[19].type, 'things')
         self.assertEqual(events[19].mode, 'active')
         self.assertEqual(events[19].timestamp, 1462629479859)
-        self.assertIsInstance(events[19].source, SourceUser)
+        self.assertIsInstance(events[19].source, UserSource)
         self.assertEqual(events[19].source.type, 'user')
         self.assertEqual(events[19].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[19].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[19].delivery_context, DeliveryContext)
         self.assertFalse(events[19].delivery_context.is_redelivery)
-        self.assertIsInstance(events[19].things, DeviceLink)
+        self.assertIsInstance(events[19].things, LinkThingsContent)
         self.assertEqual(events[19].things.type, 'link')
         self.assertEqual(events[19].things.device_id, 't2c449c9d1')
 
         # MemberJoinedEvent
         self.assertIsInstance(events[20], MemberJoinedEvent)
         self.assertEqual(events[20].reply_token, '0f3779fba3b349968c5d07db31eabf65')
         self.assertEqual(events[20].type, 'memberJoined')
         self.assertEqual(events[20].mode, 'active')
         self.assertEqual(events[20].timestamp, 1462629479859)
-        self.assertIsInstance(events[20].source, SourceGroup)
+        self.assertIsInstance(events[20].source, GroupSource)
         self.assertEqual(events[20].source.type, 'group')
         self.assertEqual(events[20].source.group_id, 'C4af4980629...')
         self.assertEqual(events[20].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[20].delivery_context, DeliveryContext)
         self.assertFalse(events[20].delivery_context.is_redelivery)
         self.assertEqual(len(events[20].joined.members), 2)
-        self.assertIsInstance(events[20].joined.members[0], SourceUser)
+        self.assertIsInstance(events[20].joined.members[0], UserSource)
         self.assertEqual(events[20].joined.members[0].user_id, 'U4af4980629...')
         self.assertEqual(events[20].joined.members[1].user_id, 'U91eeaf62d9...')
 
         # MemberLeftEvent
         self.assertIsInstance(events[21], MemberLeftEvent)
         self.assertEqual(events[21].type, 'memberLeft')
         self.assertEqual(events[21].mode, 'active')
         self.assertEqual(events[21].timestamp, 1462629479960)
-        self.assertIsInstance(events[21].source, SourceGroup)
+        self.assertIsInstance(events[21].source, GroupSource)
         self.assertEqual(events[21].source.type, 'group')
         self.assertEqual(events[21].source.group_id, 'C4af4980629...')
         self.assertEqual(events[21].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[21].delivery_context, DeliveryContext)
         self.assertFalse(events[21].delivery_context.is_redelivery)
         self.assertEqual(len(events[21].left.members), 2)
-        self.assertIsInstance(events[21].left.members[0], SourceUser)
+        self.assertIsInstance(events[21].left.members[0], UserSource)
         self.assertEqual(events[21].left.members[0].user_id, 'U4af4980629...')
         self.assertEqual(events[21].left.members[1].user_id, 'U91eeaf62d9...')
 
-        # ThingsEvent, SourceUser, unlink
+        # ThingsEvent, UserSource, unlink
         self.assertIsInstance(events[22], ThingsEvent)
         self.assertEqual(events[22].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[22].type, 'things')
         self.assertEqual(events[22].mode, 'active')
         self.assertEqual(events[22].timestamp, 1462629479859)
-        self.assertIsInstance(events[22].source, SourceUser)
+        self.assertIsInstance(events[22].source, UserSource)
         self.assertEqual(events[22].source.type, 'user')
         self.assertEqual(events[22].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[22].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[22].delivery_context, DeliveryContext)
         self.assertFalse(events[22].delivery_context.is_redelivery)
-        self.assertIsInstance(events[22].things, DeviceUnlink)
+        self.assertIsInstance(events[22].things, UnlinkThingsContent)
         self.assertEqual(events[22].things.type, 'unlink')
         self.assertEqual(events[22].things.device_id, 't2c449c9d1')
 
-        # MessageEvent, SourceUser, FileMessage
+        # MessageEvent, UserSource, UserSource
         self.assertIsInstance(events[23], MessageEvent)
         self.assertEqual(events[23].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[23].type, 'message')
         self.assertEqual(events[23].mode, 'active')
         self.assertEqual(events[23].timestamp, 1462629479859)
-        self.assertIsInstance(events[23].source, SourceUser)
+        self.assertIsInstance(events[23].source, UserSource)
         self.assertEqual(events[23].source.type, 'user')
         self.assertEqual(events[23].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[23].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[23].delivery_context, DeliveryContext)
         self.assertFalse(events[23].delivery_context.is_redelivery)
-        self.assertIsInstance(events[23].message, FileMessage)
+        self.assertIsInstance(events[23].message, FileMessageContent)
         self.assertEqual(events[23].message.id, '325708')
         self.assertEqual(events[23].message.type, 'file')
         self.assertEqual(events[23].message.file_name, "file.txt")
         self.assertEqual(events[23].message.file_size, 2138)
 
-        # ThingsEvent, SourceUser, scenarioResult
+        # ThingsEvent, UserSource, scenarioResult
         self.assertIsInstance(events[24], ThingsEvent)
         self.assertEqual(events[24].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[24].type, 'things')
         self.assertEqual(events[24].mode, 'active')
         self.assertEqual(events[24].timestamp, 1547817848122)
-        self.assertIsInstance(events[24].source, SourceUser)
+        self.assertIsInstance(events[24].source, UserSource)
         self.assertEqual(events[24].source.type, 'user')
         self.assertEqual(events[24].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[24].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[24].delivery_context, DeliveryContext)
         self.assertFalse(events[24].delivery_context.is_redelivery)
-        self.assertIsInstance(events[24].things, ScenarioResult)
+        self.assertIsInstance(events[24].things, ScenarioResultThingsContent)
         self.assertEqual(events[24].things.type, 'scenarioResult')
         self.assertEqual(events[24].things.device_id, 't2c449c9d1')
         self.assertEqual(events[24].things.result.scenario_id, 'XXX')
         self.assertEqual(events[24].things.result.revision, 2)
         self.assertEqual(events[24].things.result.start_time, 1547817845950)
         self.assertEqual(events[24].things.result.end_time, 1547817845952)
         self.assertEqual(events[24].things.result.result_code, 'success')
@@ -503,138 +503,153 @@
         self.assertEqual(events[24].things.result.action_results[1].type, 'void')
 
         # UnsendEvent
         self.assertIsInstance(events[25], UnsendEvent)
         self.assertEqual(events[25].type, 'unsend')
         self.assertEqual(events[25].mode, 'active')
         self.assertEqual(events[25].timestamp, 1547817848122)
-        self.assertIsInstance(events[25].source, SourceGroup)
+        self.assertIsInstance(events[25].source, GroupSource)
         self.assertEqual(events[25].source.type, 'group')
         self.assertEqual(events[25].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[25].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[25].delivery_context, DeliveryContext)
         self.assertFalse(events[25].delivery_context.is_redelivery)
-        self.assertIsInstance(events[25].unsend, Unsend)
+        self.assertIsInstance(events[25].unsend, UnsendDetail)
         self.assertEqual(events[25].unsend.message_id, '325708')
 
         # VideoPlayCompleteEvent
         self.assertIsInstance(events[26], VideoPlayCompleteEvent)
         self.assertEqual(events[26].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[26].type, 'videoPlayComplete')
         self.assertEqual(events[26].mode, 'active')
         self.assertEqual(events[26].timestamp, 1462629479859)
-        self.assertIsInstance(events[26].source, SourceUser)
+        self.assertIsInstance(events[26].source, UserSource)
         self.assertEqual(events[26].source.type, 'user')
         self.assertEqual(events[26].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[26].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[26].delivery_context, DeliveryContext)
         self.assertFalse(events[26].delivery_context.is_redelivery)
         self.assertIsInstance(events[26].video_play_complete, VideoPlayComplete)
         self.assertEqual(events[26].video_play_complete.tracking_id, 'track_id')
 
-        # MessageEvent, SourceUser, ImageMessage with ImageSet
+        # MessageEvent, UserSource, ImageMessage with ImageSet
         self.assertIsInstance(events[1], MessageEvent)
         self.assertEqual(events[27].reply_token, 'fbf94e269485410da6b7e3a5e33283e8')
         self.assertEqual(events[27].type, 'message')
         self.assertEqual(events[27].mode, 'active')
         self.assertEqual(events[27].timestamp, 1627356924722)
-        self.assertIsInstance(events[27].source, SourceUser)
+        self.assertIsInstance(events[27].source, UserSource)
         self.assertEqual(events[27].source.type, 'user')
         self.assertEqual(events[27].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[27].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[27].delivery_context, DeliveryContext)
         self.assertFalse(events[27].delivery_context.is_redelivery)
-        self.assertIsInstance(events[27].message, ImageMessage)
+        self.assertIsInstance(events[27].message, ImageMessageContent)
         self.assertEqual(events[27].message.id, '354718705033693861')
         self.assertEqual(events[27].message.type, 'image')
         self.assertEqual(events[27].message.content_provider.type, 'line')
         self.assertEqual(events[27].message.image_set.id, 'E005D41A7288F41B655')
         self.assertEqual(events[27].message.image_set.index, 2)
         self.assertEqual(events[27].message.image_set.total, 2)
 
-        # MessageEvent, SourceUser, TextMessage (Redeliveried)
+        # MessageEvent, UserSource, TextMessage (Redeliveried)
         self.assertIsInstance(events[28], MessageEvent)
         self.assertEqual(events[28].reply_token, 'nHuyWiB7yP5Zw52FIkcQobQuGDXCTA')
         self.assertEqual(events[28].type, 'message')
         self.assertEqual(events[28].mode, 'active')
         self.assertEqual(events[28].timestamp, 1462629479859)
-        self.assertIsInstance(events[28].source, SourceUser)
+        self.assertIsInstance(events[28].source, UserSource)
         self.assertEqual(events[28].source.type, 'user')
         self.assertEqual(events[28].source.user_id, 'U206d25c2ea6bd87c17655609a1c37cb8')
         self.assertEqual(events[28].webhook_event_id, 'testwebhookeventid')
         self.assertIsInstance(events[28].delivery_context, DeliveryContext)
         self.assertTrue(events[28].delivery_context.is_redelivery)
-        self.assertIsInstance(events[28].message, TextMessage)
+        self.assertIsInstance(events[28].message, TextMessageContent)
         self.assertEqual(events[28].message.id, '325708')
         self.assertEqual(events[28].message.type, 'text')
         self.assertEqual(events[28].message.text, 'Hello, world')
 
         # UnknownEvent
         self.assertIsInstance(events[29], UnknownEvent)
 
+        # TODO: richmenu switch
+
     def test_parse_webhook_req_without_destination(self):
         body = """
         {
             "events": [
                 {
                     "replyToken": "00000000000000000000000000000000",
                     "type": "message",
+                    "mode": "active",
                     "timestamp": 1561099010135,
                     "source": {
                         "type": "user",
                         "userId": "Udeadbeefdeadbeefdeadbeefdeadbeef"
                     },
                     "message": {
                         "id": "100001",
                         "type": "text",
                         "text": "Hello, world"
+                    },
+                    "webhookEventId": "testwebhookeventid",
+                    "deliveryContext": {
+                        "isRedelivery": false
                     }
                 },
                 {
                     "replyToken": "ffffffffffffffffffffffffffffffff",
                     "type": "message",
+                    "mode": "active",
                     "timestamp": 1561099010135,
                     "source": {
                         "type": "user",
                         "userId": "Udeadbeefdeadbeefdeadbeefdeadbeef"
                     },
                     "message": {
                         "id": "100002",
                         "type": "sticker",
                         "packageId": "1",
-                        "stickerId": "1"
+                        "stickerId": "1",
+                        "stickerResourceType": "ANIMATION"
+                    },
+                    "webhookEventId": "testwebhookeventid",
+                    "deliveryContext": {
+                        "isRedelivery": false
                     }
                 }
             ]
         }
         """
         payload = self.parser.parse(body=body, signature='channel_secret', as_payload=True)
         self.assertEqual(None, payload.destination)
 
 
 class TestWebhookHandler(unittest.TestCase):
     def setUp(self):
         self.handler = WebhookHandler('channel_secret')
 
-        @self.handler.add(MessageEvent, message=TextMessage)
+        @self.handler.add(MessageEvent, message=TextMessageContent)
         def message_text(event, destination):
             self.assertEqual('message', event.type)
             self.assertEqual('text', event.message.type)
             self.assertEqual('U123', destination)
 
         @self.handler.add(MessageEvent,
-                          message=(ImageMessage, VideoMessage, AudioMessage))
+                          message=(ImageMessageContent,
+                                   VideoMessageContent,
+                                   AudioMessageContent))
         def message_content(event):
             self.assertEqual('message', event.type)
             self.assertIn(
                 event.message.type,
                 ['image', 'video', 'audio']
             )
 
-        @self.handler.add(MessageEvent, message=StickerMessage)
+        @self.handler.add(MessageEvent, message=StickerMessageContent)
         def message_sticker(event):
             self.assertEqual('message', event.type)
             self.assertEqual('sticker', event.message.type)
 
         @self.handler.add(MessageEvent)
         def message(event):
             self.assertEqual('message', event.type)
```

### Comparing `line-bot-sdk-2.4.2/tests/text/webhook.json` & `line-bot-sdk-3.0.0/tests/text/webhook.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997395833333333%*

 * *Differences: {"'events'": "{10: {'postback': {'params': OrderedDict([('datetime', '2017-12-25T01:00')])}}}"}*

```diff
@@ -194,15 +194,18 @@
         },
         {
             "deliveryContext": {
                 "isRedelivery": false
             },
             "mode": "active",
             "postback": {
-                "data": "action=buyItem&itemId=123123&color=red"
+                "data": "action=buyItem&itemId=123123&color=red",
+                "params": {
+                    "datetime": "2017-12-25T01:00"
+                }
             },
             "replyToken": "nHuyWiB7yP5Zw52FIkcQobQuGDXCTA",
             "source": {
                 "type": "user",
                 "userId": "U206d25c2ea6bd87c17655609a1c37cb8"
             },
             "timestamp": 1462629479859,
```

### Comparing `line-bot-sdk-2.4.2/tox.ini` & `line-bot-sdk-3.0.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py3.7, py3.8, py3.9, py3.10, py3-flake8-src, py3-flake8-other
+envlist = py3.7, py3.8, py3.9, py3.10, py3.11, py3-flake8-src, py3-flake8-other
 
 [testenv]
 deps =
     six
     -r{toxinidir}/requirements.txt
     -r{toxinidir}/requirements-test.txt
 commands = py.test -v tests/
@@ -15,15 +15,16 @@
 
 [testenv:py3-flake8-src]
 basepython = python3
 deps =
     six
     flake8
     flake8-docstrings
-commands = flake8 linebot/
+# Ignores generated files.
+commands = flake8 --filename=linebot/*.py
 
 [testenv:py3-flake8-other]
 basepython = python3
 deps =
     six
     flake8
 commands = flake8 tests/ examples/ --max-line-length=120
```

