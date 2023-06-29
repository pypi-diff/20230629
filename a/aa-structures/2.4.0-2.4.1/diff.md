# Comparing `tmp/aa_structures-2.4.0.tar.gz` & `tmp/aa_structures-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_structures-2.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_structures-2.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_structures-2.4.0.tar` & `aa_structures-2.4.1.tar`

### file list

```diff
@@ -1,174 +1,174 @@
--rw-r--r--   0        0        0     1070 2023-06-28 11:50:10.152553 aa_structures-2.4.0/LICENSE
--rw-r--r--   0        0        0     4406 2023-06-28 11:50:10.156553 aa_structures-2.4.0/README.md
--rw-r--r--   0        0        0     2069 2023-06-28 11:50:10.156553 aa_structures-2.4.0/pyproject.toml
--rw-r--r--   0        0        0      170 2023-06-28 11:58:29.139033 aa_structures-2.4.0/structures/__init__.py
--rw-r--r--   0        0        0    36110 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/admin.py
--rw-r--r--   0        0        0     6228 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/app_settings.py
--rw-r--r--   0        0        0      268 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/apps.py
--rw-r--r--   0        0        0      915 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/auth_hooks.py
--rw-r--r--   0        0        0     1232 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/checks.py
--rw-r--r--   0        0        0      741 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/constants.py
--rw-r--r--   0        0        0        0 2023-06-28 12:18:16.631954 aa_structures-2.4.0/structures/core/__init__.py
--rw-r--r--   0        0        0    71519 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/core/notification_embeds.py
--rw-r--r--   0        0        0    16436 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/core/notification_timers.py
--rw-r--r--   0        0        0    19834 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/core/serializers.py
--rw-r--r--   0        0        0      623 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/core/sovereignty.py
--rw-r--r--   0        0        0     1613 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/core/starbases.py
--rw-r--r--   0        0        0      382 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/forms.py
--rw-r--r--   0        0        0        0 2023-06-28 12:18:16.631954 aa_structures-2.4.0/structures/helpers/__init__.py
--rw-r--r--   0        0        0      830 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/helpers/general.py
--rw-r--r--   0        0        0    13634 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    61204 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47227 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/locale/django.pot
--rw-r--r--   0        0        0      380 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47274 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5784 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    55691 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47227 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47227 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47267 2023-06-28 11:50:10.160553 aa_structures-2.4.0/structures/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      391 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47024 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/locale/ko/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47227 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      538 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47437 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47505 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11588 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    58962 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-06-28 12:18:16.631954 aa_structures-2.4.0/structures/management/commands/__init__.py
--rw-r--r--   0        0        0     1443 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/management/commands/structures_load_eve.py
--rw-r--r--   0        0        0     2398 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/management/commands/structures_preload_eveuniverse.py
--rw-r--r--   0        0        0    18949 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/managers.py
--rw-r--r--   0        0        0    59315 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/migrations/0001_initial_new.py
--rw-r--r--   0        0        0     2274 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/migrations/0002_remove_eveuniverse_relation_names.py
--rw-r--r--   0        0        0    44042 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/migrations/0003_add_localization_and_unique_key.py
--rw-r--r--   0        0        0        0 2023-06-28 12:18:16.631954 aa_structures-2.4.0/structures/migrations/__init__.py
--rw-r--r--   0        0        0      505 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/models/__init__.py
--rw-r--r--   0        0        0     2073 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/models/eveuniverse.py
--rw-r--r--   0        0        0    42745 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/models/notifications.py
--rw-r--r--   0        0        0    53967 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/models/owners.py
--rw-r--r--   0        0        0    37256 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/models/structures.py
--rw-r--r--   0        0        0      274 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/providers.py
--rw-r--r--   0        0        0     1165 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/static/structures/css/global.css
--rw-r--r--   0        0        0     1186 2023-06-28 11:50:10.164553 aa_structures-2.4.0/structures/static/structures/css/main.css
--rw-r--r--   0        0        0    43262 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0      908 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/eve_symbol_128.png
--rw-r--r--   0        0        0      805 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/0h.png
--rw-r--r--   0        0        0      805 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/0l.png
--rw-r--r--   0        0        0      805 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/0m.png
--rw-r--r--   0        0        0      805 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/0r.png
--rw-r--r--   0        0        0      805 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/0s.png
--rw-r--r--   0        0        0     2590 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/1h.png
--rw-r--r--   0        0        0     1976 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/1l.png
--rw-r--r--   0        0        0     2025 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/1m.png
--rw-r--r--   0        0        0     2512 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/1r.png
--rw-r--r--   0        0        0     3541 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/2h.png
--rw-r--r--   0        0        0     2570 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/2l.png
--rw-r--r--   0        0        0     2766 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/2m.png
--rw-r--r--   0        0        0     3497 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/2r.png
--rw-r--r--   0        0        0     4607 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/3h.png
--rw-r--r--   0        0        0     3523 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/3l.png
--rw-r--r--   0        0        0     3720 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/3m.png
--rw-r--r--   0        0        0     4886 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/3r.png
--rw-r--r--   0        0        0     5309 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/4h.png
--rw-r--r--   0        0        0     4628 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/4l.png
--rw-r--r--   0        0        0     4956 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/4m.png
--rw-r--r--   0        0        0     9490 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/4s.png
--rw-r--r--   0        0        0     6109 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/5h.png
--rw-r--r--   0        0        0     5888 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/5l.png
--rw-r--r--   0        0        0     6270 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/5m.png
--rw-r--r--   0        0        0     7399 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/5s.png
--rw-r--r--   0        0        0     7203 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/6h.png
--rw-r--r--   0        0        0     7014 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/6l.png
--rw-r--r--   0        0        0     7439 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/6m.png
--rw-r--r--   0        0        0     8288 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/7h.png
--rw-r--r--   0        0        0     8067 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/7l.png
--rw-r--r--   0        0        0     8580 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/7m.png
--rw-r--r--   0        0        0     9276 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/8h.png
--rw-r--r--   0        0        0     8972 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/8l.png
--rw-r--r--   0        0        0     9541 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/8m.png
--rw-r--r--   0        0        0      195 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/blank.png
--rw-r--r--   0        0        0    16840 2023-06-28 11:50:10.168552 aa_structures-2.4.0/structures/static/structures/img/panel/circle.png
--rw-r--r--   0        0        0    33523 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/static/structures/img/panel/dustwheel.png
--rw-r--r--   0        0        0     1480 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/static/structures/img/panel/h.png
--rw-r--r--   0        0        0     1480 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/static/structures/img/panel/l.png
--rw-r--r--   0        0        0     1480 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/static/structures/img/panel/m.png
--rw-r--r--   0        0        0     8879 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/static/structures/img/panel/noship.png
--rw-r--r--   0        0        0     1480 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/static/structures/img/panel/r.png
--rw-r--r--   0        0        0    43642 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/static/structures/img/panel/tyrannis.png
--rw-r--r--   0        0        0    43560 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/static/structures/img/panel/tyrannis_blue.png
--rw-r--r--   0        0        0    42833 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/static/structures/img/panel/tyrannis_darkred.png
--rw-r--r--   0        0        0    38343 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/static/structures/img/panel/tyrannis_default.png
--rw-r--r--   0        0        0    42868 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/static/structures/img/panel/tyrannis_revelations.png
--rw-r--r--   0        0        0      496 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/static/structures/img/structures_logo.png
--rw-r--r--   0        0        0     8806 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/tasks.py
--rw-r--r--   0        0        0      298 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/base.html
--rw-r--r--   0        0        0    21200 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/main.html
--rw-r--r--   0        0        0      264 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/modals/fitting_assets.html
--rw-r--r--   0        0        0     9530 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/modals/fitting_gfx.html
--rw-r--r--   0        0        0     2705 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/modals/poco_details.html
--rw-r--r--   0        0        0     4133 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/modals/starbase_detail.html
--rw-r--r--   0        0        0     4070 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/modals/structure_details.html
--rw-r--r--   0        0        0      998 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/modals/tab_general_detail.html
--rw-r--r--   0        0        0     1501 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/partials/jump_gates_list.html
--rw-r--r--   0        0        0     1034 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/partials/poco_list.html
--rw-r--r--   0        0        0     5947 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/partials/structure_list.html
--rw-r--r--   0        0        0     1586 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/partials/structure_summary.html
--rw-r--r--   0        0        0      117 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/templatetags/detail_title.html
--rw-r--r--   0        0        0      375 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/templatetags/list_asset.html
--rw-r--r--   0        0        0      706 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/templatetags/list_item.html
--rw-r--r--   0        0        0      505 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/templatetags/list_tax_item.html
--rw-r--r--   0        0        0       68 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templates/structures/templatetags/list_title.html
--rw-r--r--   0        0        0        0 2023-06-28 12:18:16.639953 aa_structures-2.4.0/structures/templatetags/__init__.py
--rw-r--r--   0        0        0     1601 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/templatetags/structures.py
--rw-r--r--   0        0        0       75 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 12:18:16.639953 aa_structures-2.4.0/structures/tests/core/__init__.py
--rw-r--r--   0        0        0    13532 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/tests/core/test_notification_embeds.py
--rw-r--r--   0        0        0    10435 2023-06-28 11:50:10.172552 aa_structures-2.4.0/structures/tests/core/test_notification_structuretimers.py
--rw-r--r--   0        0        0     5515 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/core/test_notifications_timerboard.py
--rw-r--r--   0        0        0     3385 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/core/test_serializers.py
--rw-r--r--   0        0        0      825 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/core/test_sovereignty.py
--rw-r--r--   0        0        0     3163 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/core/test_starbases.py
--rw-r--r--   0        0        0        0 2023-06-28 12:18:16.639953 aa_structures-2.4.0/structures/tests/models/__init__.py
--rw-r--r--   0        0        0     1600 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/models/test_eveuniverse.py
--rw-r--r--   0        0        0    39346 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/models/test_notifications_1.py
--rw-r--r--   0        0        0    31553 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/models/test_notifications_2.py
--rw-r--r--   0        0        0     6004 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/models/test_notifications_3.py
--rw-r--r--   0        0        0     5318 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/models/test_notifications_discord.py
--rw-r--r--   0        0        0    26807 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/models/test_owners_1.py
--rw-r--r--   0        0        0    54158 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/models/test_owners_2.py
--rw-r--r--   0        0        0    37407 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/models/test_owners_3.py
--rw-r--r--   0        0        0    37744 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/models/test_structures.py
--rw-r--r--   0        0        0    21127 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/test_admin.py
--rw-r--r--   0        0        0     1242 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/test_checks.py
--rw-r--r--   0        0        0     1861 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/test_helpers.py
--rw-r--r--   0        0        0    23524 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/test_integration.py
--rw-r--r--   0        0        0    26102 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/test_managers_1.py
--rw-r--r--   0        0        0     1567 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/test_managers_3.py
--rw-r--r--   0        0        0    18409 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/test_tasks.py
--rw-r--r--   0        0        0    36695 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/test_views.py
--rw-r--r--   0        0        0        0 2023-06-28 12:18:16.639953 aa_structures-2.4.0/structures/tests/testdata/__init__.py
--rw-r--r--   0        0        0     2601 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/testdata/create_eveuniverse.py
--rw-r--r--   0        0        0    33188 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/testdata/entities.json
--rw-r--r--   0        0        0    13864 2023-06-28 11:50:10.176552 aa_structures-2.4.0/structures/tests/testdata/esi_data.json
--rw-r--r--   0        0        0   979813 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/tests/testdata/eveuniverse.json
--rw-r--r--   0        0        0     7827 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/tests/testdata/factories.py
--rw-r--r--   0        0        0    10857 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/tests/testdata/factories_2.py
--rw-r--r--   0        0        0     5746 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/tests/testdata/generate_notifications.py
--rw-r--r--   0        0        0     1415 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/tests/testdata/generate_notifications_2.py
--rw-r--r--   0        0        0     6238 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/tests/testdata/generate_structures.py
--rw-r--r--   0        0        0    26820 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/tests/testdata/helpers.py
--rw-r--r--   0        0        0      395 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/tests/testdata/load_eveuniverse.py
--rw-r--r--   0        0        0      963 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/tests/testdata/tasks_loadtest.py
--rw-r--r--   0        0        0      414 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/tests/testdata/test_generate_structures.py
--rw-r--r--   0        0        0     1057 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/urls.py
--rw-r--r--   0        0        0    21820 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/views.py
--rw-r--r--   0        0        0        0 2023-06-28 12:18:16.639953 aa_structures-2.4.0/structures/webhooks/__init__.py
--rw-r--r--   0        0        0     6587 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/webhooks/core.py
--rw-r--r--   0        0        0     1036 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/webhooks/managers.py
--rw-r--r--   0        0        0     1641 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/webhooks/models.py
--rw-r--r--   0        0        0        0 2023-06-28 12:18:16.639953 aa_structures-2.4.0/structures/webhooks/tests/__init__.py
--rw-r--r--   0        0        0     6395 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/webhooks/tests/test_core.py
--rw-r--r--   0        0        0      459 2023-06-28 11:50:10.180552 aa_structures-2.4.0/structures/webhooks/tests/test_utils.py
--rw-r--r--   0        0        0     5933 1970-01-01 00:00:00.000000 aa_structures-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-28 11:50:10.152553 aa_structures-2.4.1/LICENSE
+-rw-r--r--   0        0        0     4406 2023-06-28 11:50:10.156553 aa_structures-2.4.1/README.md
+-rw-r--r--   0        0        0     2069 2023-06-28 11:50:10.156553 aa_structures-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-06-29 12:35:51.837332 aa_structures-2.4.1/structures/__init__.py
+-rw-r--r--   0        0        0    36110 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/admin.py
+-rw-r--r--   0        0        0     6228 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/app_settings.py
+-rw-r--r--   0        0        0      268 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/apps.py
+-rw-r--r--   0        0        0      915 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/auth_hooks.py
+-rw-r--r--   0        0        0     1232 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/checks.py
+-rw-r--r--   0        0        0      741 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/constants.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:58:08.028016 aa_structures-2.4.1/structures/core/__init__.py
+-rw-r--r--   0        0        0    71519 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/core/notification_embeds.py
+-rw-r--r--   0        0        0    16436 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/core/notification_timers.py
+-rw-r--r--   0        0        0    19834 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/core/serializers.py
+-rw-r--r--   0        0        0      623 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/core/sovereignty.py
+-rw-r--r--   0        0        0     1613 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/core/starbases.py
+-rw-r--r--   0        0        0      382 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/forms.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:58:08.028016 aa_structures-2.4.1/structures/helpers/__init__.py
+-rw-r--r--   0        0        0      830 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/helpers/general.py
+-rw-r--r--   0        0        0    13634 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    61204 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/django.pot
+-rw-r--r--   0        0        0      380 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47274 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5784 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    55691 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47267 2023-06-28 11:50:10.160553 aa_structures-2.4.1/structures/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      391 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47024 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/locale/ko/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      538 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47437 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47505 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11588 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    58962 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-06-29 12:58:08.028016 aa_structures-2.4.1/structures/management/commands/__init__.py
+-rw-r--r--   0        0        0     1443 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/management/commands/structures_load_eve.py
+-rw-r--r--   0        0        0     2398 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/management/commands/structures_preload_eveuniverse.py
+-rw-r--r--   0        0        0    18114 2023-06-29 12:35:51.837332 aa_structures-2.4.1/structures/managers.py
+-rw-r--r--   0        0        0    59315 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/migrations/0001_initial_new.py
+-rw-r--r--   0        0        0     2274 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/migrations/0002_remove_eveuniverse_relation_names.py
+-rw-r--r--   0        0        0    44042 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/migrations/0003_add_localization_and_unique_key.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:58:08.028016 aa_structures-2.4.1/structures/migrations/__init__.py
+-rw-r--r--   0        0        0      505 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/models/__init__.py
+-rw-r--r--   0        0        0     2073 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/models/eveuniverse.py
+-rw-r--r--   0        0        0    42745 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/models/notifications.py
+-rw-r--r--   0        0        0    53967 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/models/owners.py
+-rw-r--r--   0        0        0    37256 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/models/structures.py
+-rw-r--r--   0        0        0      274 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/providers.py
+-rw-r--r--   0        0        0     1165 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/static/structures/css/global.css
+-rw-r--r--   0        0        0     1186 2023-06-28 11:50:10.164553 aa_structures-2.4.1/structures/static/structures/css/main.css
+-rw-r--r--   0        0        0    43262 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0      908 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/eve_symbol_128.png
+-rw-r--r--   0        0        0      805 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/0h.png
+-rw-r--r--   0        0        0      805 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/0l.png
+-rw-r--r--   0        0        0      805 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/0m.png
+-rw-r--r--   0        0        0      805 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/0r.png
+-rw-r--r--   0        0        0      805 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/0s.png
+-rw-r--r--   0        0        0     2590 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/1h.png
+-rw-r--r--   0        0        0     1976 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/1l.png
+-rw-r--r--   0        0        0     2025 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/1m.png
+-rw-r--r--   0        0        0     2512 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/1r.png
+-rw-r--r--   0        0        0     3541 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/2h.png
+-rw-r--r--   0        0        0     2570 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/2l.png
+-rw-r--r--   0        0        0     2766 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/2m.png
+-rw-r--r--   0        0        0     3497 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/2r.png
+-rw-r--r--   0        0        0     4607 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/3h.png
+-rw-r--r--   0        0        0     3523 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/3l.png
+-rw-r--r--   0        0        0     3720 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/3m.png
+-rw-r--r--   0        0        0     4886 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/3r.png
+-rw-r--r--   0        0        0     5309 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/4h.png
+-rw-r--r--   0        0        0     4628 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/4l.png
+-rw-r--r--   0        0        0     4956 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/4m.png
+-rw-r--r--   0        0        0     9490 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/4s.png
+-rw-r--r--   0        0        0     6109 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/5h.png
+-rw-r--r--   0        0        0     5888 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/5l.png
+-rw-r--r--   0        0        0     6270 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/5m.png
+-rw-r--r--   0        0        0     7399 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/5s.png
+-rw-r--r--   0        0        0     7203 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/6h.png
+-rw-r--r--   0        0        0     7014 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/6l.png
+-rw-r--r--   0        0        0     7439 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/6m.png
+-rw-r--r--   0        0        0     8288 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/7h.png
+-rw-r--r--   0        0        0     8067 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/7l.png
+-rw-r--r--   0        0        0     8580 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/7m.png
+-rw-r--r--   0        0        0     9276 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/8h.png
+-rw-r--r--   0        0        0     8972 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/8l.png
+-rw-r--r--   0        0        0     9541 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/8m.png
+-rw-r--r--   0        0        0      195 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/blank.png
+-rw-r--r--   0        0        0    16840 2023-06-28 11:50:10.168552 aa_structures-2.4.1/structures/static/structures/img/panel/circle.png
+-rw-r--r--   0        0        0    33523 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/dustwheel.png
+-rw-r--r--   0        0        0     1480 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/h.png
+-rw-r--r--   0        0        0     1480 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/l.png
+-rw-r--r--   0        0        0     1480 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/m.png
+-rw-r--r--   0        0        0     8879 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/noship.png
+-rw-r--r--   0        0        0     1480 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/r.png
+-rw-r--r--   0        0        0    43642 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis.png
+-rw-r--r--   0        0        0    43560 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis_blue.png
+-rw-r--r--   0        0        0    42833 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis_darkred.png
+-rw-r--r--   0        0        0    38343 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis_default.png
+-rw-r--r--   0        0        0    42868 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis_revelations.png
+-rw-r--r--   0        0        0      496 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/static/structures/img/structures_logo.png
+-rw-r--r--   0        0        0     8806 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/tasks.py
+-rw-r--r--   0        0        0      298 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/base.html
+-rw-r--r--   0        0        0    21200 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/main.html
+-rw-r--r--   0        0        0      264 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/modals/fitting_assets.html
+-rw-r--r--   0        0        0     9530 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/modals/fitting_gfx.html
+-rw-r--r--   0        0        0     2705 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/modals/poco_details.html
+-rw-r--r--   0        0        0     4133 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/modals/starbase_detail.html
+-rw-r--r--   0        0        0     4070 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/modals/structure_details.html
+-rw-r--r--   0        0        0      998 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/modals/tab_general_detail.html
+-rw-r--r--   0        0        0     1501 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/partials/jump_gates_list.html
+-rw-r--r--   0        0        0     1034 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/partials/poco_list.html
+-rw-r--r--   0        0        0     5947 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/partials/structure_list.html
+-rw-r--r--   0        0        0     1586 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/partials/structure_summary.html
+-rw-r--r--   0        0        0      117 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/templatetags/detail_title.html
+-rw-r--r--   0        0        0      375 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/templatetags/list_asset.html
+-rw-r--r--   0        0        0      706 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/templatetags/list_item.html
+-rw-r--r--   0        0        0      505 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/templatetags/list_tax_item.html
+-rw-r--r--   0        0        0       68 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templates/structures/templatetags/list_title.html
+-rw-r--r--   0        0        0        0 2023-06-29 12:58:08.036016 aa_structures-2.4.1/structures/templatetags/__init__.py
+-rw-r--r--   0        0        0     1601 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/templatetags/structures.py
+-rw-r--r--   0        0        0       75 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:58:08.036016 aa_structures-2.4.1/structures/tests/core/__init__.py
+-rw-r--r--   0        0        0    13532 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/tests/core/test_notification_embeds.py
+-rw-r--r--   0        0        0    10435 2023-06-28 11:50:10.172552 aa_structures-2.4.1/structures/tests/core/test_notification_structuretimers.py
+-rw-r--r--   0        0        0     5515 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/core/test_notifications_timerboard.py
+-rw-r--r--   0        0        0     3385 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/core/test_serializers.py
+-rw-r--r--   0        0        0      825 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/core/test_sovereignty.py
+-rw-r--r--   0        0        0     3163 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/core/test_starbases.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:58:08.036016 aa_structures-2.4.1/structures/tests/models/__init__.py
+-rw-r--r--   0        0        0     1600 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_eveuniverse.py
+-rw-r--r--   0        0        0    39346 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_notifications_1.py
+-rw-r--r--   0        0        0    31553 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_notifications_2.py
+-rw-r--r--   0        0        0     6004 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_notifications_3.py
+-rw-r--r--   0        0        0     5318 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_notifications_discord.py
+-rw-r--r--   0        0        0    26807 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_owners_1.py
+-rw-r--r--   0        0        0    54158 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_owners_2.py
+-rw-r--r--   0        0        0    37407 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_owners_3.py
+-rw-r--r--   0        0        0    37744 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/models/test_structures.py
+-rw-r--r--   0        0        0    21127 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/test_admin.py
+-rw-r--r--   0        0        0     1242 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/test_checks.py
+-rw-r--r--   0        0        0     1861 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/test_helpers.py
+-rw-r--r--   0        0        0    23524 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/test_integration.py
+-rw-r--r--   0        0        0    27217 2023-06-29 12:35:51.837332 aa_structures-2.4.1/structures/tests/test_managers_1.py
+-rw-r--r--   0        0        0     1567 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/test_managers_3.py
+-rw-r--r--   0        0        0    18409 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/test_tasks.py
+-rw-r--r--   0        0        0    36695 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/test_views.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:58:08.036016 aa_structures-2.4.1/structures/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     2601 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0    33188 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/testdata/entities.json
+-rw-r--r--   0        0        0    13864 2023-06-28 11:50:10.176552 aa_structures-2.4.1/structures/tests/testdata/esi_data.json
+-rw-r--r--   0        0        0   979813 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0     7827 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/factories.py
+-rw-r--r--   0        0        0    10857 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/factories_2.py
+-rw-r--r--   0        0        0     5746 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/generate_notifications.py
+-rw-r--r--   0        0        0     1415 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/generate_notifications_2.py
+-rw-r--r--   0        0        0     6238 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/generate_structures.py
+-rw-r--r--   0        0        0    26820 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/helpers.py
+-rw-r--r--   0        0        0      395 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0      963 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/tasks_loadtest.py
+-rw-r--r--   0        0        0      414 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/tests/testdata/test_generate_structures.py
+-rw-r--r--   0        0        0     1057 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/urls.py
+-rw-r--r--   0        0        0    21820 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/views.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:58:08.036016 aa_structures-2.4.1/structures/webhooks/__init__.py
+-rw-r--r--   0        0        0     6587 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/webhooks/core.py
+-rw-r--r--   0        0        0     1036 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/webhooks/managers.py
+-rw-r--r--   0        0        0     1641 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/webhooks/models.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:58:08.036016 aa_structures-2.4.1/structures/webhooks/tests/__init__.py
+-rw-r--r--   0        0        0     6395 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/webhooks/tests/test_core.py
+-rw-r--r--   0        0        0      459 2023-06-28 11:50:10.180552 aa_structures-2.4.1/structures/webhooks/tests/test_utils.py
+-rw-r--r--   0        0        0     5933 1970-01-01 00:00:00.000000 aa_structures-2.4.1/PKG-INFO
```

### Comparing `aa_structures-2.4.0/LICENSE` & `aa_structures-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/README.md` & `aa_structures-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/pyproject.toml` & `aa_structures-2.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/admin.py` & `aa_structures-2.4.1/structures/admin.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/app_settings.py` & `aa_structures-2.4.1/structures/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/auth_hooks.py` & `aa_structures-2.4.1/structures/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/checks.py` & `aa_structures-2.4.1/structures/checks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/constants.py` & `aa_structures-2.4.1/structures/constants.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/core/notification_embeds.py` & `aa_structures-2.4.1/structures/core/notification_embeds.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/core/notification_timers.py` & `aa_structures-2.4.1/structures/core/notification_timers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/core/serializers.py` & `aa_structures-2.4.1/structures/core/serializers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/core/sovereignty.py` & `aa_structures-2.4.1/structures/core/sovereignty.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/core/starbases.py` & `aa_structures-2.4.1/structures/core/starbases.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/helpers/general.py` & `aa_structures-2.4.1/structures/helpers/general.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/locale/de/LC_MESSAGES/django.mo` & `aa_structures-2.4.1/structures/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/locale/de/LC_MESSAGES/django.po` & `aa_structures-2.4.1/structures/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/locale/django.pot` & `aa_structures-2.4.1/structures/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/locale/en/LC_MESSAGES/django.po` & `aa_structures-2.4.1/structures/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/locale/es/LC_MESSAGES/django.mo` & `aa_structures-2.4.1/structures/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/locale/es/LC_MESSAGES/django.po` & `aa_structures-2.4.1/structures/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/locale/fr_FR/LC_MESSAGES/django.po` & `aa_structures-2.4.1/structures/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/locale/it_IT/LC_MESSAGES/django.po` & `aa_structures-2.4.1/structures/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/locale/ja/LC_MESSAGES/django.po` & `aa_structures-2.4.1/structures/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/locale/ko/LC_MESSAGES/django.po` & `aa_structures-2.4.1/structures/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/locale/ko_KR/LC_MESSAGES/django.po` & `aa_structures-2.4.1/structures/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/locale/ru/LC_MESSAGES/django.mo` & `aa_structures-2.4.1/structures/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/locale/ru/LC_MESSAGES/django.po` & `aa_structures-2.4.1/structures/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/locale/uk/LC_MESSAGES/django.po` & `aa_structures-2.4.1/structures/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_structures-2.4.1/structures/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_structures-2.4.1/structures/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/management/commands/structures_load_eve.py` & `aa_structures-2.4.1/structures/management/commands/structures_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/management/commands/structures_preload_eveuniverse.py` & `aa_structures-2.4.1/structures/management/commands/structures_preload_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/managers.py` & `aa_structures-2.4.1/structures/managers.py`

 * *Files 3% similar despite different names*

```diff
@@ -341,105 +341,86 @@
         }
         owner = Owner.objects.get(
             corporation__corporation_id=structure_info["corporation_id"]
         )
         obj, created = self.update_or_create_from_dict(structure=structure, owner=owner)
         return obj, created
 
-    def update_or_create_from_dict(self, structure: dict, owner: object) -> tuple:
+    def update_or_create_from_dict(self, structure: dict, owner) -> tuple:
         """update or create structure from given dict"""
 
         from .models import StructureService
 
         eve_type, _ = EveType.objects.get_or_create_esi(id=structure["type_id"])
         eve_solar_system, _ = EveSolarSystem.objects.get_or_create_esi(
             id=structure["system_id"]
         )
-        fuel_expires_at = (
-            structure["fuel_expires"] if "fuel_expires" in structure else None
-        )
-        next_reinforce_hour = (
-            structure["next_reinforce_hour"]
-            if "next_reinforce_hour" in structure
-            else None
-        )
-        next_reinforce_apply = (
-            structure["next_reinforce_apply"]
-            if "next_reinforce_apply" in structure
-            else None
-        )
-        reinforce_hour = (
-            structure["reinforce_hour"] if "reinforce_hour" in structure else None
-        )
-        state = (
-            self.model.State.from_esi_name(structure["state"])
-            if "state" in structure
-            else self.model.State.UNKNOWN
-        )
-        state_timer_start = (
-            structure["state_timer_start"] if "state_timer_start" in structure else None
-        )
-        state_timer_end = (
-            structure["state_timer_end"] if "state_timer_end" in structure else None
-        )
-        unanchors_at = (
-            structure["unanchors_at"] if "unanchors_at" in structure else None
-        )
-        position_x = structure["position"]["x"] if "position" in structure else None
-        position_y = structure["position"]["y"] if "position" in structure else None
-        position_z = structure["position"]["z"] if "position" in structure else None
-        if "planet_id" in structure:
-            eve_planet, _ = EvePlanet.objects.get_or_create_esi(
-                id=structure["planet_id"]
-            )
+        if position := structure.get("position"):
+            position_x = position.get("x")
+            position_y = position.get("y")
+            position_z = position.get("z")
+        else:
+            position_x = position_y = position_z = None
+        if planet_id := structure.get("planet_id"):
+            eve_planet, _ = EvePlanet.objects.get_or_create_esi(id=planet_id)
         else:
             eve_planet = None
-        if "moon_id" in structure:
-            eve_moon, _ = EveMoon.objects.get_or_create_esi(id=structure["moon_id"])
+        if moon_id := structure.get("moon_id"):
+            eve_moon, _ = EveMoon.objects.get_or_create_esi(id=moon_id)
         else:
             eve_moon = None
+
+        structure_id = structure["structure_id"]
         try:
-            old_obj = self.get(id=structure["structure_id"])
+            old_obj = self.get(id=structure_id)
         except self.model.DoesNotExist:
             old_obj = None
+
         obj, created = self.update_or_create(
-            id=structure["structure_id"],
+            id=structure_id,
             defaults={
                 "owner": owner,
                 "eve_type": eve_type,
-                "name": structure["name"],
+                "name": structure.get("name", ""),
                 "eve_solar_system": eve_solar_system,
                 "eve_planet": eve_planet,
                 "eve_moon": eve_moon,
                 "position_x": position_x,
                 "position_y": position_y,
                 "position_z": position_z,
-                "fuel_expires_at": fuel_expires_at,
-                "next_reinforce_hour": next_reinforce_hour,
-                "next_reinforce_apply": next_reinforce_apply,
-                "reinforce_hour": reinforce_hour,
-                "state": state,
-                "state_timer_start": state_timer_start,
-                "state_timer_end": state_timer_end,
-                "unanchors_at": unanchors_at,
+                "fuel_expires_at": structure.get("fuel_expires"),
+                "next_reinforce_hour": structure.get("next_reinforce_hour"),
+                "next_reinforce_apply": structure.get("next_reinforce_apply"),
+                "reinforce_hour": structure.get("reinforce_hour"),
+                "state": self.model.State.from_esi_name(structure.get("state", "")),
+                "state_timer_start": structure.get("state_timer_start"),
+                "state_timer_end": structure.get("state_timer_end"),
+                "unanchors_at": structure.get("unanchors_at"),
                 "last_updated_at": now(),
             },
         )
+
         if old_obj:
             obj.handle_fuel_notifications(old_obj)
+
         # Make sure we have dogmas loaded for this type for fittings
         EveType.objects.get_or_create_esi(
             id=structure["type_id"], enabled_sections=[EveType.Section.DOGMAS]
         )
+
         # save related structure services
         StructureService.objects.filter(structure=obj).delete()
         if "services" in structure and structure["services"]:
             for service in structure["services"]:
-                state = StructureService.State.from_esi_name(service["state"])
-                args = {"structure": obj, "name": service["name"], "state": state}
+                service_state = StructureService.State.from_esi_name(service["state"])
+                args = {
+                    "structure": obj,
+                    "name": service["name"],
+                    "state": service_state,
+                }
                 StructureService.objects.create(**args)
 
         if obj.services.filter(state=StructureService.State.ONLINE).exists():
             obj.last_online_at = now()
             obj.save()
 
         return obj, created
```

### Comparing `aa_structures-2.4.0/structures/migrations/0001_initial_new.py` & `aa_structures-2.4.1/structures/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/migrations/0002_remove_eveuniverse_relation_names.py` & `aa_structures-2.4.1/structures/migrations/0002_remove_eveuniverse_relation_names.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/migrations/0003_add_localization_and_unique_key.py` & `aa_structures-2.4.1/structures/migrations/0003_add_localization_and_unique_key.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/models/eveuniverse.py` & `aa_structures-2.4.1/structures/models/eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/models/notifications.py` & `aa_structures-2.4.1/structures/models/notifications.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/models/owners.py` & `aa_structures-2.4.1/structures/models/owners.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/models/structures.py` & `aa_structures-2.4.1/structures/models/structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/css/global.css` & `aa_structures-2.4.1/structures/static/structures/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/css/main.css` & `aa_structures-2.4.1/structures/static/structures/css/main.css`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/Spinner-1s-64px-dark.gif` & `aa_structures-2.4.1/structures/static/structures/img/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/Spinner-1s-64px-light.gif` & `aa_structures-2.4.1/structures/static/structures/img/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/eve_symbol_128.png` & `aa_structures-2.4.1/structures/static/structures/img/eve_symbol_128.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/0h.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/0h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/0l.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/0l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/0m.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/0m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/0r.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/0r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/0s.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/0s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/1h.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/1h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/1l.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/1l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/1m.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/1m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/1r.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/1r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/2h.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/2h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/2l.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/2l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/2m.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/2m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/2r.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/2r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/3h.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/3h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/3l.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/3l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/3m.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/3m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/3r.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/3r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/4h.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/4h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/4l.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/4l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/4m.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/4m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/4s.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/4s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/5h.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/5h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/5l.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/5l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/5m.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/5m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/5s.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/5s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/6h.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/6h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/6l.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/6l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/6m.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/6m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/7h.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/7h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/7l.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/7l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/7m.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/7m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/8h.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/8h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/8l.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/8l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/8m.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/8m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/circle.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/circle.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/dustwheel.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/dustwheel.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/h.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/l.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/m.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/noship.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/noship.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/r.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/tyrannis.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/tyrannis_blue.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis_blue.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/tyrannis_darkred.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis_darkred.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/tyrannis_default.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis_default.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/static/structures/img/panel/tyrannis_revelations.png` & `aa_structures-2.4.1/structures/static/structures/img/panel/tyrannis_revelations.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tasks.py` & `aa_structures-2.4.1/structures/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/templates/structures/main.html` & `aa_structures-2.4.1/structures/templates/structures/main.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/templates/structures/modals/fitting_gfx.html` & `aa_structures-2.4.1/structures/templates/structures/modals/fitting_gfx.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/templates/structures/modals/poco_details.html` & `aa_structures-2.4.1/structures/templates/structures/modals/poco_details.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/templates/structures/modals/starbase_detail.html` & `aa_structures-2.4.1/structures/templates/structures/modals/starbase_detail.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/templates/structures/modals/structure_details.html` & `aa_structures-2.4.1/structures/templates/structures/modals/structure_details.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/templates/structures/modals/tab_general_detail.html` & `aa_structures-2.4.1/structures/templates/structures/modals/tab_general_detail.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/templates/structures/partials/jump_gates_list.html` & `aa_structures-2.4.1/structures/templates/structures/partials/jump_gates_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/templates/structures/partials/poco_list.html` & `aa_structures-2.4.1/structures/templates/structures/partials/poco_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/templates/structures/partials/structure_list.html` & `aa_structures-2.4.1/structures/templates/structures/partials/structure_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/templates/structures/partials/structure_summary.html` & `aa_structures-2.4.1/structures/templates/structures/partials/structure_summary.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/templates/structures/templatetags/list_item.html` & `aa_structures-2.4.1/structures/templates/structures/templatetags/list_item.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/templatetags/structures.py` & `aa_structures-2.4.1/structures/templatetags/structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/core/test_notification_embeds.py` & `aa_structures-2.4.1/structures/tests/core/test_notification_embeds.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/core/test_notification_structuretimers.py` & `aa_structures-2.4.1/structures/tests/core/test_notification_structuretimers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/core/test_notifications_timerboard.py` & `aa_structures-2.4.1/structures/tests/core/test_notifications_timerboard.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/core/test_serializers.py` & `aa_structures-2.4.1/structures/tests/core/test_serializers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/core/test_sovereignty.py` & `aa_structures-2.4.1/structures/tests/core/test_sovereignty.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/core/test_starbases.py` & `aa_structures-2.4.1/structures/tests/core/test_starbases.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/models/test_eveuniverse.py` & `aa_structures-2.4.1/structures/tests/models/test_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/models/test_notifications_1.py` & `aa_structures-2.4.1/structures/tests/models/test_notifications_1.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/models/test_notifications_2.py` & `aa_structures-2.4.1/structures/tests/models/test_notifications_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/models/test_notifications_3.py` & `aa_structures-2.4.1/structures/tests/models/test_notifications_3.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/models/test_notifications_discord.py` & `aa_structures-2.4.1/structures/tests/models/test_notifications_discord.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/models/test_owners_1.py` & `aa_structures-2.4.1/structures/tests/models/test_owners_1.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/models/test_owners_2.py` & `aa_structures-2.4.1/structures/tests/models/test_owners_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/models/test_owners_3.py` & `aa_structures-2.4.1/structures/tests/models/test_owners_3.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/models/test_structures.py` & `aa_structures-2.4.1/structures/tests/models/test_structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/test_admin.py` & `aa_structures-2.4.1/structures/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/test_checks.py` & `aa_structures-2.4.1/structures/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/test_helpers.py` & `aa_structures-2.4.1/structures/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/test_integration.py` & `aa_structures-2.4.1/structures/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/test_managers_1.py` & `aa_structures-2.4.1/structures/tests/test_managers_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 from django.utils.timezone import now
 from eveuniverse.models import EveSolarSystem
 
 from allianceauth.eveonline.models import EveCharacter, EveCorporationInfo
 from app_utils.esi_testing import EsiClientStub, EsiEndpoint
 from app_utils.testing import NoSocketsTestCase, create_user_from_evecharacter
 
-from ..models import (
+from structures.models import (
     EveSovereigntyMap,
     NotificationType,
     Owner,
     Structure,
     StructureService,
     StructureTag,
     Webhook,
 )
+
 from .testdata.factories import (
     create_eve_sovereignty_map,
     create_owner_from_user,
     create_upwell_structure,
 )
+from .testdata.factories_2 import OwnerFactory
 from .testdata.helpers import create_structures, load_entities
 from .testdata.load_eveuniverse import load_eveuniverse
 
 MODULE_PATH = "structures.managers"
 MODULE_PATH_ESI_FETCH = "structures.helpers.esi_fetch"
 
 
@@ -499,14 +501,40 @@
             structure, owner
         )
 
         # check structure
         self.assertFalse(created)
         self.assertIsNone(structure.last_online_at)
 
+    def test_can_create_starbase_without_moon(self):
+        owner = OwnerFactory()
+        structure = {
+            "structure_id": 1300000000099,
+            "name": "Hidden place",
+            "system_id": 30002537,
+            "type_id": 16213,
+            "moon_id": None,
+            "position": {"x": 55028384780.0, "y": 7310316270.0, "z": -163686684205.0},
+        }
+        structure, created = Structure.objects.update_or_create_from_dict(
+            structure, owner
+        )
+
+        # check structure
+        structure: Structure
+        self.assertTrue(created)
+        self.assertEqual(structure.id, 1300000000099)
+        self.assertEqual(structure.eve_type_id, 16213)
+        self.assertEqual(structure.eve_solar_system_id, 30002537)
+        self.assertEqual(structure.owner, owner)
+        self.assertEqual(structure.position_x, 55028384780.0)
+        self.assertEqual(structure.position_y, 7310316270.0)
+        self.assertEqual(structure.position_z, -163686684205.0)
+        self.assertEqual(structure.state, Structure.State.UNKNOWN)
+
 
 class TestStructureTagManager(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         load_eveuniverse()
         load_entities([EveSovereigntyMap])
```

### Comparing `aa_structures-2.4.0/structures/tests/test_managers_3.py` & `aa_structures-2.4.1/structures/tests/test_managers_3.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/test_tasks.py` & `aa_structures-2.4.1/structures/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/test_views.py` & `aa_structures-2.4.1/structures/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/testdata/create_eveuniverse.py` & `aa_structures-2.4.1/structures/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/testdata/entities.json` & `aa_structures-2.4.1/structures/tests/testdata/entities.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/testdata/esi_data.json` & `aa_structures-2.4.1/structures/tests/testdata/esi_data.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/testdata/eveuniverse.json` & `aa_structures-2.4.1/structures/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/testdata/factories.py` & `aa_structures-2.4.1/structures/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/testdata/factories_2.py` & `aa_structures-2.4.1/structures/tests/testdata/factories_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/testdata/generate_notifications.py` & `aa_structures-2.4.1/structures/tests/testdata/generate_notifications.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/testdata/generate_notifications_2.py` & `aa_structures-2.4.1/structures/tests/testdata/generate_notifications_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/testdata/generate_structures.py` & `aa_structures-2.4.1/structures/tests/testdata/generate_structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/testdata/helpers.py` & `aa_structures-2.4.1/structures/tests/testdata/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/tests/testdata/tasks_loadtest.py` & `aa_structures-2.4.1/structures/tests/testdata/tasks_loadtest.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/urls.py` & `aa_structures-2.4.1/structures/urls.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/views.py` & `aa_structures-2.4.1/structures/views.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/webhooks/core.py` & `aa_structures-2.4.1/structures/webhooks/core.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/webhooks/managers.py` & `aa_structures-2.4.1/structures/webhooks/managers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/webhooks/models.py` & `aa_structures-2.4.1/structures/webhooks/models.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/structures/webhooks/tests/test_core.py` & `aa_structures-2.4.1/structures/webhooks/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.4.0/PKG-INFO` & `aa_structures-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-structures
-Version: 2.4.0
+Version: 2.4.1
 Summary: App for managing Eve Online structures with Alliance Auth.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
```

