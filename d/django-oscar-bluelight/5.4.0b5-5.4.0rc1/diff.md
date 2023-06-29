# Comparing `tmp/django-oscar-bluelight-5.4.0b5.tar.gz` & `tmp/django-oscar-bluelight-5.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oscar-bluelight-5.4.0b5.tar", last modified: Tue Jun 27 19:55:25 2023, max compression
+gzip compressed data, was "django-oscar-bluelight-5.4.0rc1.tar", last modified: Thu Jun 29 20:46:37 2023, max compression
```

## Comparing `django-oscar-bluelight-5.4.0b5.tar` & `django-oscar-bluelight-5.4.0rc1.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.333107 django-oscar-bluelight-5.4.0b5/
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    15745 2023-06-27 19:55:25.333107 django-oscar-bluelight-5.4.0b5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    14997 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/README.md
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-27 19:55:25.333107 django-oscar-bluelight-5.4.0b5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2028 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.302081 django-oscar-bluelight-5.4.0b5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.305732 django-oscar-bluelight-5.4.0b5/src/django_oscar_bluelight.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15745 2023-06-27 19:55:25.000000 django-oscar-bluelight-5.4.0b5/src/django_oscar_bluelight.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8920 2023-06-27 19:55:25.000000 django-oscar-bluelight-5.4.0b5/src/django_oscar_bluelight.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 19:55:25.000000 django-oscar-bluelight-5.4.0b5/src/django_oscar_bluelight.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-27 19:55:25.000000 django-oscar-bluelight-5.4.0b5/src/django_oscar_bluelight.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-27 19:55:25.000000 django-oscar-bluelight-5.4.0b5/src/django_oscar_bluelight.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.306644 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3965 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/basket_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2923 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/caching.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.306644 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.307556 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/offers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/offers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/offers/api_views.py
--rw-rw-rw-   0 root         (0) root         (0)     4469 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/offers/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     8885 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/offers/forms.py
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/offers/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/offers/reports.py
--rw-rw-rw-   0 root         (0) root         (0)     2628 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/offers/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)    15037 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/offers/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.308469 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/ranges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/ranges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/ranges/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     3985 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/ranges/forms.py
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/ranges/models.py
--rw-rw-rw-   0 root         (0) root         (0)     5764 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/ranges/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.310294 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/vouchers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/vouchers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2867 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/vouchers/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     4450 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/vouchers/forms.py
--rw-rw-rw-   0 root         (0) root         (0)    15136 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/vouchers/views.py
--rw-rw-rw-   0 root         (0) root         (0)     3809 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/defaults.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.302081 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.302994 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.311207 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    37748 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/locale/es/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.mo
--rw-rw-rw-   0 root         (0) root         (0)     2145 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.po
--rw-rw-rw-   0 root         (0) root         (0)    12939 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.313032 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1984 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     9493 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/applicator.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    27667 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/benefits.py
--rw-rw-rw-   0 root         (0) root         (0)    15451 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/conditions.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4735 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/groups.py
--rw-rw-rw-   0 root         (0) root         (0)     3028 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.317594 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    25223 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0002_auto_20151210_1053.py
--rw-rw-rw-   0 root         (0) root         (0)     1538 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0002_compoundcondition.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0003_merge.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0004_conditionaloffer_groups.py
--rw-rw-rw-   0 root         (0) root         (0)     3547 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0005_auto_20160719_1238.py
--rw-rw-rw-   0 root         (0) root         (0)     8828 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0006_bluelightabsolutediscountbenefit_bluelightcountcondition_bluelightcoveragecondition_bluelightfixedpr.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0007_auto_20170417_1354.py
--rw-rw-rw-   0 root         (0) root         (0)     1708 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0008_auto_20170512_1049.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0009_auto_20170517_1605.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0009_auto_20200801_0817.py
--rw-rw-rw-   0 root         (0) root         (0)      989 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0010_auto_20170613_1245.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0010_conditionaloffer_combinations.py
--rw-rw-rw-   0 root         (0) root         (0)     1991 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0011_auto_20170710_1442.py
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0011_conditionaloffer_affects_cosmetic_pricing.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0012_auto_20180514_1142.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0012_auto_20211020_1037.py
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0013_alter_offergroup_slug.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0013_conditionaloffer_exclusive.py
--rw-rw-rw-   0 root         (0) root         (0)      879 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0014_auto_20181017_1151.py
--rw-rw-rw-   0 root         (0) root         (0)     3442 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0014_drop_triggers.py
--rw-rw-rw-   0 root         (0) root         (0)      903 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0015_auto_20181018_1220.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0016_remove_conditionaloffer_apply_to_displayed_prices.py
--rw-rw-rw-   0 root         (0) root         (0)     2921 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0017_auto_20190705_1245.py
--rw-rw-rw-   0 root         (0) root         (0)     1404 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0017_compoundbenefit.py
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0018_merge_20190705_1247.py
--rw-rw-rw-   0 root         (0) root         (0)      833 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0019_auto_20190926_1547.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0020_remove_range_cache_version.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0021_rangeproductset.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15503 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2400 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/reports.py
--rw-rw-rw-   0 root         (0) root         (0)     1984 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/results.py
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/signals.py
--rw-rw-rw-   0 root         (0) root         (0)     7204 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/sql.py
--rw-rw-rw-   0 root         (0) root         (0)     1817 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     3994 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/upsells.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.302994 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.319419 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/static/oscarbluelight/
--rw-rw-rw-   0 root         (0) root         (0)     1388 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/static/oscarbluelight/offergroups.css
--rw-rw-rw-   0 root         (0) root         (0)     1936 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/static/oscarbluelight/offergroups.css.map
--rw-rw-rw-   0 root         (0) root         (0)     6571 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/static/oscarbluelight/offergroups.js
--rw-rw-rw-   0 root         (0) root         (0)    24756 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/static/oscarbluelight/offergroups.js.map
--rw-rw-rw-   0 root         (0) root         (0)   210646 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/static/oscarbluelight/vendor.js
--rw-rw-rw-   0 root         (0) root         (0)   778250 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/static/oscarbluelight/vendor.js.map
--rw-rw-rw-   0 root         (0) root         (0)     1293 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/static/oscarbluelight/webpack-stats.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.302994 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.302994 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.302994 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/catalogue/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.319419 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/catalogue/partials/
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/catalogue/partials/stock_record.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.303907 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.323070 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/
--rw-rw-rw-   0 root         (0) root         (0)     1992 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_delete.html
--rw-rw-rw-   0 root         (0) root         (0)     5482 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit.html
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit_compound.html
--rw-rw-rw-   0 root         (0) root         (0)     5404 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_list.html
--rw-rw-rw-   0 root         (0) root         (0)      787 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_selection_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1997 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/condition_delete.html
--rw-rw-rw-   0 root         (0) root         (0)     5389 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit.html
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit_compound.html
--rw-rw-rw-   0 root         (0) root         (0)     5391 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/condition_list.html
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/condition_selection_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1959 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/image_form.html
--rw-rw-rw-   0 root         (0) root         (0)     9218 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/offer_detail.html
--rw-rw-rw-   0 root         (0) root         (0)     5691 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/offer_list.html
--rw-rw-rw-   0 root         (0) root         (0)     1924 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_delete.html
--rw-rw-rw-   0 root         (0) root         (0)     3944 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_edit.html
--rw-rw-rw-   0 root         (0) root         (0)     1547 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.323070 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/partials/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/partials/offer_thumbnail.html
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/restrictions_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.323070 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/ranges/
--rw-rw-rw-   0 root         (0) root         (0)     1793 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/ranges/range_excluded_products.html
--rw-rw-rw-   0 root         (0) root         (0)     5266 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/ranges/range_list.html
--rw-rw-rw-   0 root         (0) root         (0)     8583 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/ranges/range_price_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.324895 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/vouchers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.324895 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/vouchers/partials/
--rw-rw-rw-   0 root         (0) root         (0)     4162 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/vouchers/partials/voucher_details_table.html
--rw-rw-rw-   0 root         (0) root         (0)     2792 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_add_children.html
--rw-rw-rw-   0 root         (0) root         (0)     7389 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_detail.html
--rw-rw-rw-   0 root         (0) root         (0)     2773 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_export_children.html
--rw-rw-rw-   0 root         (0) root         (0)     2257 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_form.html
--rw-rw-rw-   0 root         (0) root         (0)     3599 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list.html
--rw-rw-rw-   0 root         (0) root         (0)     6453 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list_children.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.324895 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templatetags/oscarbluelight_tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.324895 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.327632 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/base.py
--rw-rw-rw-   0 root         (0) root         (0)    19887 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_benefit_absolute.py
--rw-rw-rw-   0 root         (0) root         (0)    11153 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_benefit_compound.py
--rw-rw-rw-   0 root         (0) root         (0)     8276 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_benefit_fixed_price.py
--rw-rw-rw-   0 root         (0) root         (0)     8234 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_benefit_fixed_price_per_item.py
--rw-rw-rw-   0 root         (0) root         (0)     6558 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_benefit_multibuy.py
--rw-rw-rw-   0 root         (0) root         (0)    15250 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_benefit_percentage.py
--rw-rw-rw-   0 root         (0) root         (0)    37853 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_conditions.py
--rw-rw-rw-   0 root         (0) root         (0)     2862 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_cosmetic_prices.py
--rw-rw-rw-   0 root         (0) root         (0)    54267 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_offer_groups.py
--rw-rw-rw-   0 root         (0) root         (0)    10397 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_range.py
--rw-rw-rw-   0 root         (0) root         (0)    12352 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_recalculate_offer_application_totals.py
--rw-rw-rw-   0 root         (0) root         (0)     6926 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_system_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.327632 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/voucher/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/voucher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7817 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/voucher/test_rules.py
--rw-rw-rw-   0 root         (0) root         (0)    17769 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/voucher/test_vouchers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.329457 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 19:55:25.333107 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     5397 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      729 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0002_auto_20160503_1138.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0003_voucher_parent.py
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0004_auto_20161115_1115.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0005_auto_20170613_1245.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0006_auto_20170710_1442.py
--rw-rw-rw-   0 root         (0) root         (0)     2850 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0007_auto_20180601_1348.py
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0008_auto_20190926_1547.py
--rw-rw-rw-   0 root         (0) root         (0)     1703 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0008_auto_20200801_0817.py
--rw-rw-rw-   0 root         (0) root         (0)      557 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0009_auto_20210216_1327.py
--rw-rw-rw-   0 root         (0) root         (0)     2620 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0010_auto_20210526_1410.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0011_auto_20220615_1024.py
--rw-rw-rw-   0 root         (0) root         (0)      455 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0012_voucher_status.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11548 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3017 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/reports.py
--rw-rw-rw-   0 root         (0) root         (0)     4250 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/rules.py
--rw-rw-rw-   0 root         (0) root         (0)     3229 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/sql.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-06-27 19:55:15.000000 django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/tasks.py
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-27 19:55:25.000000 django-oscar-bluelight-5.4.0b5/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.268343 django-oscar-bluelight-5.4.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    15962 2023-06-29 20:46:37.268343 django-oscar-bluelight-5.4.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    15213 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-29 20:46:37.268343 django-oscar-bluelight-5.4.0rc1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2028 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.236343 django-oscar-bluelight-5.4.0rc1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.241344 django-oscar-bluelight-5.4.0rc1/src/django_oscar_bluelight.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15962 2023-06-29 20:46:37.000000 django-oscar-bluelight-5.4.0rc1/src/django_oscar_bluelight.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8920 2023-06-29 20:46:37.000000 django-oscar-bluelight-5.4.0rc1/src/django_oscar_bluelight.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 20:46:37.000000 django-oscar-bluelight-5.4.0rc1/src/django_oscar_bluelight.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-29 20:46:37.000000 django-oscar-bluelight-5.4.0rc1/src/django_oscar_bluelight.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-29 20:46:37.000000 django-oscar-bluelight-5.4.0rc1/src/django_oscar_bluelight.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.242344 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3965 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/basket_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2923 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/caching.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.242344 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.243343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/offers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/offers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/offers/api_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     4469 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/offers/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     8885 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/offers/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/offers/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/offers/reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/offers/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)    15037 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/offers/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.244343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/ranges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/ranges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/ranges/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3985 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/ranges/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/ranges/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     5764 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/ranges/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.245344 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/vouchers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/vouchers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2867 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/vouchers/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/vouchers/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)    15136 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/vouchers/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     3809 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/defaults.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.237343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.237343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.246343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    37748 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/locale/es/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2145 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.po
+-rw-rw-rw-   0 root         (0) root         (0)    12939 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.248343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1984 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     9720 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/applicator.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    28056 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/benefits.py
+-rw-rw-rw-   0 root         (0) root         (0)    15451 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/conditions.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4735 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     3028 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.253343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    25223 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0002_auto_20151210_1053.py
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0002_compoundcondition.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0003_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0004_conditionaloffer_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     3547 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0005_auto_20160719_1238.py
+-rw-rw-rw-   0 root         (0) root         (0)     8828 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0006_bluelightabsolutediscountbenefit_bluelightcountcondition_bluelightcoveragecondition_bluelightfixedpr.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0007_auto_20170417_1354.py
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0008_auto_20170512_1049.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0009_auto_20170517_1605.py
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0009_auto_20200801_0817.py
+-rw-rw-rw-   0 root         (0) root         (0)      989 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0010_auto_20170613_1245.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0010_conditionaloffer_combinations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0011_auto_20170710_1442.py
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0011_conditionaloffer_affects_cosmetic_pricing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0012_auto_20180514_1142.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0012_auto_20211020_1037.py
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0013_alter_offergroup_slug.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0013_conditionaloffer_exclusive.py
+-rw-rw-rw-   0 root         (0) root         (0)      879 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0014_auto_20181017_1151.py
+-rw-rw-rw-   0 root         (0) root         (0)     3442 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0014_drop_triggers.py
+-rw-rw-rw-   0 root         (0) root         (0)      903 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0015_auto_20181018_1220.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0016_remove_conditionaloffer_apply_to_displayed_prices.py
+-rw-rw-rw-   0 root         (0) root         (0)     2921 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0017_auto_20190705_1245.py
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0017_compoundbenefit.py
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0018_merge_20190705_1247.py
+-rw-rw-rw-   0 root         (0) root         (0)      833 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0019_auto_20190926_1547.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0020_remove_range_cache_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0021_rangeproductset.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15503 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     1984 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/results.py
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)     7204 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3994 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/upsells.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.237343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.255343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/static/oscarbluelight/
+-rw-rw-rw-   0 root         (0) root         (0)     1388 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/static/oscarbluelight/offergroups.css
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/static/oscarbluelight/offergroups.css.map
+-rw-rw-rw-   0 root         (0) root         (0)     6571 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/static/oscarbluelight/offergroups.js
+-rw-rw-rw-   0 root         (0) root         (0)    24756 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/static/oscarbluelight/offergroups.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   210646 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/static/oscarbluelight/vendor.js
+-rw-rw-rw-   0 root         (0) root         (0)   778250 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/static/oscarbluelight/vendor.js.map
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/static/oscarbluelight/webpack-stats.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.237343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.238344 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.238344 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/catalogue/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.256343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/catalogue/partials/
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/catalogue/partials/stock_record.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.238344 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.259343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/
+-rw-rw-rw-   0 root         (0) root         (0)     1992 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_delete.html
+-rw-rw-rw-   0 root         (0) root         (0)     5482 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit.html
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit_compound.html
+-rw-rw-rw-   0 root         (0) root         (0)     5404 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_list.html
+-rw-rw-rw-   0 root         (0) root         (0)      787 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_selection_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1997 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/condition_delete.html
+-rw-rw-rw-   0 root         (0) root         (0)     5389 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit.html
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit_compound.html
+-rw-rw-rw-   0 root         (0) root         (0)     5391 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/condition_list.html
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/condition_selection_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1959 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/image_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     9218 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/offer_detail.html
+-rw-rw-rw-   0 root         (0) root         (0)     5691 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/offer_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     1924 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_delete.html
+-rw-rw-rw-   0 root         (0) root         (0)     3944 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_edit.html
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.259343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/partials/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/partials/offer_thumbnail.html
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/restrictions_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.259343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/ranges/
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/ranges/range_excluded_products.html
+-rw-rw-rw-   0 root         (0) root         (0)     5266 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/ranges/range_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     8583 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/ranges/range_price_list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.260343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/vouchers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.260343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/vouchers/partials/
+-rw-rw-rw-   0 root         (0) root         (0)     4162 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/vouchers/partials/voucher_details_table.html
+-rw-rw-rw-   0 root         (0) root         (0)     2792 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_add_children.html
+-rw-rw-rw-   0 root         (0) root         (0)     7389 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_detail.html
+-rw-rw-rw-   0 root         (0) root         (0)     2773 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_export_children.html
+-rw-rw-rw-   0 root         (0) root         (0)     2257 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     3599 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     6453 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list_children.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.261343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templatetags/oscarbluelight_tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.261343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.264343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    19887 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_benefit_absolute.py
+-rw-rw-rw-   0 root         (0) root         (0)    11153 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_benefit_compound.py
+-rw-rw-rw-   0 root         (0) root         (0)     8276 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_benefit_fixed_price.py
+-rw-rw-rw-   0 root         (0) root         (0)     8243 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_benefit_fixed_price_per_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     6558 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_benefit_multibuy.py
+-rw-rw-rw-   0 root         (0) root         (0)    15250 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_benefit_percentage.py
+-rw-rw-rw-   0 root         (0) root         (0)    37853 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_conditions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2862 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_cosmetic_prices.py
+-rw-rw-rw-   0 root         (0) root         (0)    54267 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_offer_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)    10397 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_range.py
+-rw-rw-rw-   0 root         (0) root         (0)    12352 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_recalculate_offer_application_totals.py
+-rw-rw-rw-   0 root         (0) root         (0)     6926 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_system_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.264343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/voucher/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/voucher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7817 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/voucher/test_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)    17769 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/voucher/test_vouchers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.265343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 20:46:37.267343 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     5397 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      729 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0002_auto_20160503_1138.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0003_voucher_parent.py
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0004_auto_20161115_1115.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0005_auto_20170613_1245.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0006_auto_20170710_1442.py
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0007_auto_20180601_1348.py
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0008_auto_20190926_1547.py
+-rw-rw-rw-   0 root         (0) root         (0)     1703 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0008_auto_20200801_0817.py
+-rw-rw-rw-   0 root         (0) root         (0)      557 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0009_auto_20210216_1327.py
+-rw-rw-rw-   0 root         (0) root         (0)     2620 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0010_auto_20210526_1410.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0011_auto_20220615_1024.py
+-rw-rw-rw-   0 root         (0) root         (0)      455 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0012_voucher_status.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     4250 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     3229 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-06-29 20:46:26.000000 django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/tasks.py
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-29 20:46:37.000000 django-oscar-bluelight-5.4.0rc1/version.txt
```

### Comparing `django-oscar-bluelight-5.4.0b5/LICENSE` & `django-oscar-bluelight-5.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/PKG-INFO` & `django-oscar-bluelight-5.4.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar-bluelight
-Version: 5.4.0b5
+Version: 5.4.0rc1
 Summary: Bluelight Specials - Enhancements to the offer and vouchers features for Django Oscar.
 Home-page: https://gitlab.com/thelabnyc/django-oscar-bluelight
 Author: thelabnyc
 Author-email: thelabdev@thelabnyc.com
 License: ISC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -137,14 +137,17 @@
 ## Changelog
 
 ### 5.4.0
 
 - Add rules framework to allow library consumers to change how vouchers are determined to be available or not.
 - Add functionality for recalculating offer application totals based on OrderDiscount models. This allows correcting voucher discount stats to account for canceled orders.
 - Redesign RangeProductSet view updating to improve web request performance (at the cost of allowing the view to be slightly out of date).
+- Fix issue where a voucher is applied multiple times when it contains multiple offers.
+- Allow HiddenPostOrderAction benefits to be combined with other benefit types.
+- Improve descriptions of fixed price benefits.
 
 ### 5.3.0
 
 - Add new system for obtaining structured data regarding offer upsell messages
 - Add `BLUELIGHT_IGNORED_ORDER_STATUSES`, ignore voucher usage on orders with those statuses
 
 ### 5.2.4
```

### Comparing `django-oscar-bluelight-5.4.0b5/README.md` & `django-oscar-bluelight-5.4.0rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,17 @@
 ## Changelog
 
 ### 5.4.0
 
 - Add rules framework to allow library consumers to change how vouchers are determined to be available or not.
 - Add functionality for recalculating offer application totals based on OrderDiscount models. This allows correcting voucher discount stats to account for canceled orders.
 - Redesign RangeProductSet view updating to improve web request performance (at the cost of allowing the view to be slightly out of date).
+- Fix issue where a voucher is applied multiple times when it contains multiple offers.
+- Allow HiddenPostOrderAction benefits to be combined with other benefit types.
+- Improve descriptions of fixed price benefits.
 
 ### 5.3.0
 
 - Add new system for obtaining structured data regarding offer upsell messages
 - Add `BLUELIGHT_IGNORED_ORDER_STATUSES`, ignore voucher usage on orders with those statuses
 
 ### 5.2.4
```

### Comparing `django-oscar-bluelight-5.4.0b5/setup.py` & `django-oscar-bluelight-5.4.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/django_oscar_bluelight.egg-info/PKG-INFO` & `django-oscar-bluelight-5.4.0rc1/src/django_oscar_bluelight.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar-bluelight
-Version: 5.4.0b5
+Version: 5.4.0rc1
 Summary: Bluelight Specials - Enhancements to the offer and vouchers features for Django Oscar.
 Home-page: https://gitlab.com/thelabnyc/django-oscar-bluelight
 Author: thelabnyc
 Author-email: thelabdev@thelabnyc.com
 License: ISC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -137,14 +137,17 @@
 ## Changelog
 
 ### 5.4.0
 
 - Add rules framework to allow library consumers to change how vouchers are determined to be available or not.
 - Add functionality for recalculating offer application totals based on OrderDiscount models. This allows correcting voucher discount stats to account for canceled orders.
 - Redesign RangeProductSet view updating to improve web request performance (at the cost of allowing the view to be slightly out of date).
+- Fix issue where a voucher is applied multiple times when it contains multiple offers.
+- Allow HiddenPostOrderAction benefits to be combined with other benefit types.
+- Improve descriptions of fixed price benefits.
 
 ### 5.3.0
 
 - Add new system for obtaining structured data regarding offer upsell messages
 - Add `BLUELIGHT_IGNORED_ORDER_STATUSES`, ignore voucher usage on orders with those statuses
 
 ### 5.2.4
```

### Comparing `django-oscar-bluelight-5.4.0b5/src/django_oscar_bluelight.egg-info/SOURCES.txt` & `django-oscar-bluelight-5.4.0rc1/src/django_oscar_bluelight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/basket_utils.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/basket_utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/caching.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/caching.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/offers/apps.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/offers/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/offers/forms.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/offers/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/offers/reports.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/offers/reports.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/offers/serializers.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/offers/serializers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/offers/views.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/offers/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/ranges/apps.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/ranges/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/ranges/forms.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/ranges/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/ranges/views.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/ranges/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/vouchers/apps.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/vouchers/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/vouchers/forms.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/vouchers/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/dashboard/vouchers/views.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/dashboard/vouchers/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/defaults.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/defaults.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/locale/es/LC_MESSAGES/django.po` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.po` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/mixins.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/mixins.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/admin.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/admin.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/applicator.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/applicator.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,19 @@
         return qs.select_related(*self._offer_select_related_fields)
 
     def get_basket_offers(self, basket, user):
         offers = []
         if not basket.id or not user:
             return offers
 
-        for voucher in basket.vouchers.all():
+        # Ordering by PK / Distinct is necessary here to avoid selecting
+        # duplicate rows when a voucher has more than one offer associated with
+        # it.
+        vouchers = basket.vouchers.all().order_by("pk").distinct()
+        for voucher in vouchers.all():
             available_to_user, __ = voucher.is_available_to_user(user=user)
             if voucher.is_active() and available_to_user:
                 basket_offers = voucher.offers.select_related(
                     *self._offer_select_related_fields
                 ).all()
                 for offer in basket_offers:
                     offer.set_voucher(voucher)
```

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/benefits.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/benefits.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from oscar.templatetags.currency_filters import currency
 import copy
 
 Benefit = get_model("offer", "Benefit")
 
 BasketDiscount = get_class("offer.results", "BasketDiscount")
 PostOrderAction = get_class("offer.results", "PostOrderAction")
+HiddenPostOrderAction = get_class("offer.results", "HiddenPostOrderAction")
 ZERO_DISCOUNT = get_class("offer.results", "ZERO_DISCOUNT")
 
 
 class BluelightPercentageDiscountBenefit(PercentageDiscountBenefit):
     """
     An offer benefit that gives a percentage discount
     """
@@ -272,28 +273,29 @@
     the max_affected_items and uses the products affected by the condition instead. This
     changes the behavior to more closely follow how other benefits work. It applied, it
     gives the basket items in the benefit range for a fixed price, not the basket items
     in the condition range. It also respects the max_affected_items setting.
     """
 
     _description = _(
-        "The products in the range are sold for %(amount)s, %(max_affected_items)s"
+        "The products in %(range)s are sold for %(amount)s, %(max_affected_items)s"
     )
 
     class Meta:
         app_label = "offer"
         proxy = True
         verbose_name = _("Fixed price benefit")
         verbose_name_plural = _("Fixed price benefits")
 
     @property
     def name(self):
         return self._append_max_discount_to_text(
             self._description
             % {
+                "range": self.range,
                 "amount": currency(self.value),
                 "max_affected_items": (
                     _("maximum %s item(s)") % self.max_affected_items
                 )
                 if self.max_affected_items
                 else _("no maximum"),
             }
@@ -366,28 +368,29 @@
     the max_affected_items and uses the products affected by the condition instead. This
     changes the behavior to more closely follow how other benefits work. It applied, it
     gives the basket items in the benefit range for a fixed price, not the basket items
     in the condition range. It also respects the max_affected_items setting.
     """
 
     _description = _(
-        "The products in the range are sold for %(amount)s each; %(max_affected_items)s"
+        "The products in %(range)s are sold for %(amount)s each; %(max_affected_items)s"
     )
 
     class Meta:
         app_label = "offer"
         proxy = True
         verbose_name = _("Fixed price per item benefit")
         verbose_name_plural = _("Fixed price per item benefits")
 
     @property
     def name(self):
         return self._append_max_discount_to_text(
             self._description
             % {
+                "range": self.range,
                 "amount": currency(self.value),
                 "max_affected_items": (
                     _("maximum %s item(s)") % self.max_affected_items
                 )
                 if self.max_affected_items
                 else _("no maximum"),
             }
@@ -722,15 +725,19 @@
             result = child.apply(
                 basket,
                 condition,
                 offer,
                 max_total_discount=max(discount_amount_available, D("0.00")),
                 consume_items=_consume_items,
             )
-            if combined_result is None:
+            if isinstance(result, HiddenPostOrderAction):
+                # Explicitly ignore HiddenPostOrderAction so that they're the
+                # one exception to the to "can't combine differing types rule".
+                pass
+            elif combined_result is None:
                 combined_result = copy.deepcopy(result)
                 discount_amount_available -= result.discount
             elif combined_result.affects == result.affects:
                 combined_result.discount += result.discount
                 discount_amount_available -= result.discount
             else:
                 raise ValueError(_("Can not combine offer benefits of differing types"))
```

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/conditions.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/conditions.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/groups.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/groups.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/handlers.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/handlers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0001_initial.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0002_auto_20151210_1053.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0002_auto_20151210_1053.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0002_compoundcondition.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0002_compoundcondition.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0004_conditionaloffer_groups.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0004_conditionaloffer_groups.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0005_auto_20160719_1238.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0005_auto_20160719_1238.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0006_bluelightabsolutediscountbenefit_bluelightcountcondition_bluelightcoveragecondition_bluelightfixedpr.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0006_bluelightabsolutediscountbenefit_bluelightcountcondition_bluelightcoveragecondition_bluelightfixedpr.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0007_auto_20170417_1354.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0007_auto_20170417_1354.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0008_auto_20170512_1049.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0008_auto_20170512_1049.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0009_auto_20170517_1605.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0009_auto_20170517_1605.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0010_auto_20170613_1245.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0010_auto_20170613_1245.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0010_conditionaloffer_combinations.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0010_conditionaloffer_combinations.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0011_auto_20170710_1442.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0011_auto_20170710_1442.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0011_conditionaloffer_affects_cosmetic_pricing.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0011_conditionaloffer_affects_cosmetic_pricing.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0012_auto_20180514_1142.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0012_auto_20180514_1142.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0012_auto_20211020_1037.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0012_auto_20211020_1037.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0013_alter_offergroup_slug.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0013_alter_offergroup_slug.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0013_conditionaloffer_exclusive.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0013_conditionaloffer_exclusive.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0014_auto_20181017_1151.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0014_auto_20181017_1151.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0014_drop_triggers.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0014_drop_triggers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0015_auto_20181018_1220.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0015_auto_20181018_1220.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0017_auto_20190705_1245.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0017_auto_20190705_1245.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0017_compoundbenefit.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0017_compoundbenefit.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0019_auto_20190926_1547.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0019_auto_20190926_1547.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/migrations/0021_rangeproductset.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/migrations/0021_rangeproductset.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/models.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/reports.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/reports.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/results.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/results.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/signals.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/signals.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/sql.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/sql.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/tasks.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/tasks.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/offer/upsells.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/offer/upsells.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/static/oscarbluelight/offergroups.css` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/static/oscarbluelight/offergroups.css`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/static/oscarbluelight/offergroups.css.map` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/static/oscarbluelight/offergroups.css.map`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/static/oscarbluelight/offergroups.js` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/static/oscarbluelight/offergroups.js`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/static/oscarbluelight/offergroups.js.map` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/static/oscarbluelight/offergroups.js.map`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/static/oscarbluelight/vendor.js` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/static/oscarbluelight/vendor.js`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/static/oscarbluelight/vendor.js.map` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/static/oscarbluelight/vendor.js.map`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/static/oscarbluelight/webpack-stats.json` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/static/oscarbluelight/webpack-stats.json`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/catalogue/partials/stock_record.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/catalogue/partials/stock_record.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_delete.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_list.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_selection_form.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_selection_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/condition_delete.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/condition_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit_compound.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit_compound.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/condition_list.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/condition_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/condition_selection_form.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/condition_selection_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/image_form.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/image_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/offer_detail.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/offer_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/offer_list.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/offer_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_delete.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_edit.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_edit.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_list.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/ranges/range_excluded_products.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/ranges/range_excluded_products.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/ranges/range_list.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/ranges/range_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/ranges/range_price_list.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/ranges/range_price_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/vouchers/partials/voucher_details_table.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/vouchers/partials/voucher_details_table.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_add_children.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_add_children.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_detail.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_export_children.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_export_children.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_form.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list_children.html` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list_children.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/base.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/base.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_benefit_absolute.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_benefit_absolute.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_benefit_compound.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_benefit_compound.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_benefit_fixed_price.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_benefit_fixed_price.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_benefit_fixed_price_per_item.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_benefit_fixed_price_per_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,28 +36,28 @@
         )
         self.offer = mock.Mock()
         self.basket = factories.create_basket(empty=True)
 
     def test_name(self):
         self.assertEqual(
             self.benefit.name,
-            "The products in the range are sold for $20.00 each; no maximum",
+            "The products in All products are sold for $20.00 each; no maximum",
         )
 
     def test_description(self):
         self.assertEqual(
             self.benefit.description,
-            "The products in the range are sold for $20.00 each; no maximum",
+            "The products in All products are sold for $20.00 each; no maximum",
         )
 
     def test_description_with_max_items(self):
         self.benefit.max_affected_items = 1
         self.assertEqual(
             self.benefit.description,
-            "The products in the range are sold for $20.00 each; maximum 1 item(s)",
+            "The products in All products are sold for $20.00 each; maximum 1 item(s)",
         )
 
     def test_applies_correctly_to_empty_basket(self):
         result = self.benefit.apply(self.basket, self.condition, self.offer)
         self.assertEqual(D("0.00"), result.discount)
         self.assertEqual(0, self.basket.num_items_with_discount)
         self.assertEqual(0, self.basket.num_items_without_discount)
```

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_benefit_multibuy.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_benefit_multibuy.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_benefit_percentage.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_benefit_percentage.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_conditions.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_conditions.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_cosmetic_prices.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_cosmetic_prices.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_offer_groups.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_offer_groups.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_range.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_range.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_recalculate_offer_application_totals.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_recalculate_offer_application_totals.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/offer/test_system_groups.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/offer/test_system_groups.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/voucher/test_rules.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/voucher/test_rules.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/tests/voucher/test_vouchers.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/tests/voucher/test_vouchers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/admin.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/admin.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0001_initial.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0002_auto_20160503_1138.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0002_auto_20160503_1138.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0003_voucher_parent.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0003_voucher_parent.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0004_auto_20161115_1115.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0004_auto_20161115_1115.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0005_auto_20170613_1245.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0005_auto_20170613_1245.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0006_auto_20170710_1442.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0006_auto_20170710_1442.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0007_auto_20180601_1348.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0007_auto_20180601_1348.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0008_auto_20190926_1547.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0008_auto_20190926_1547.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0008_auto_20200801_0817.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0008_auto_20200801_0817.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0009_auto_20210216_1327.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0009_auto_20210216_1327.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0010_auto_20210526_1410.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0010_auto_20210526_1410.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/migrations/0011_auto_20220615_1024.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/migrations/0011_auto_20220615_1024.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/models.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/reports.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/reports.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/rules.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/rules.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/sql.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/sql.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b5/src/oscarbluelight/voucher/tasks.py` & `django-oscar-bluelight-5.4.0rc1/src/oscarbluelight/voucher/tasks.py`

 * *Files identical despite different names*

